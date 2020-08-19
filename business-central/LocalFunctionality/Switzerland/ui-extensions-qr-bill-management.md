---
title: Gestione fatture QR | Microsoft Docs
description: Impostare l'estensione Gestione fattura QR e generare, inviare e importare facilmente fatture QR.
author: sorenfriisalexandersen
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: QR-bill, invoice, incoming documents, payment reference
ms.date: 05/05/2020
ms.author: soalex
ms.openlocfilehash: 6c3f1a2209db2ff3e1f82e0b24d44281c661a9f5
ms.sourcegitcommit: 007b331b6974983ee614db0406f00777da359ecb
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 08/10/2020
ms.locfileid: "3676843"
---
# <a name="qr-bill-management-in-d365fin"></a>Gestione fatture QR in [!INCLUDE[d365fin](../../includes/d365fin_md.md)]
Dal 1° luglio 2020, le società svizzere devono essere in grado di ricevere le fatture QR. Le fatture QR sono distinte di pagamento che seguono le fatture e rappresentano un'iniziativa a livello nazionale per semplificare i processi di pagamento. Le fatture QR sostituiscono tutte le distinte di pagamento esistenti e le funzionalità relative a PVR. Contengono tutte le informazioni necessarie per effettuare i pagamenti e un codice QR sulla distinta di pagamento semplifica l'importazione delle informazioni [!INCLUDE[d365fin](../../includes/d365fin_md.md)]. Tutte le informazioni rilevanti vengono importate e utilizzate per generare pagamenti per il fornitore che ha inviato la fattura QR, incluso il riferimento di pagamento, che viene automaticamente incluso nelle voci dei movimenti contabili fornitori ed esportato nei file di pagamento alla banca.

## <a name="get-started-with-the-qr-bill-management-extension"></a>Inizia con l'estensione Gestione fattura QR
L'estensione Gestione fattura QR è inclusa e installata automaticamente in [!INCLUDE[d365fin](../../includes/d365fin_md.md)]. Per iniziare con l'estensione, è necessario apportare alcune modifiche alla configurazione [!INCLUDE[d365fin](../../includes/d365fin_md.md)]. Un modo semplice è quello di utilizzare la guida all'installazione assistita per la fattura QR. La guida ti aiuterà a inserire informazioni, come:

* Specifica se utilizzare il tuo IBAN o QR-IBAN.
* Definire come visualizzare nomi e indirizzi sulle fatture QR e utilizzare la codifica dei caratteri Umlaut tedeschi. Si consiglia di utilizzare i valori predefiniti.
* Seleziona il layout predefinito da utilizzare per le fatture QR. Il layout determina se utilizzare IBAN o QR-IBAN, se il tipo di riferimento è creditore o riferimento QR e se includere le informazioni di fatturazione nel formato SWICO.
* Abilita le fatture di vendita e assistenza e i metodi di pagamento per le fatture QR.
* Specificare la definizione registrazioni e il batch registrazioni da utilizzare per la generazione di registro acquisti da fatture QR scansionate o importate.

Se necessario, è possibile modificare queste impostazioni nelle seguenti pagine: 

* **Impostazione della fattura QR** per modificare le impostazioni generali. 
* **Layout della fattura QR** per modificare le impostazioni del layout.

## <a name="issuing-qr-bills"></a>Emissione di fatture QR
È possibile abilitare le fatture QR per le fatture di vendita e assistenza. Questo aggiunge una voce a **Selezione report - Vendite** che genera un PDF aggiuntivo con la fattura QR quando vengono generate le fatture.  

## <a name="adding-billing-information-to-qr-bills"></a>Aggiunta di informazioni di fatturazione a fatture QR
Quando si crea una fattura QR, è possibile includere le informazioni di fatturazione nel formato SWICO, come richiesto da SIX, il fornitore svizzero di infrastrutture di pagamento. Idealmente, anche le applicazioni aziendali che producono o importano fatture QR dovrebbero essere in grado di elaborare informazioni quali l'importo dell'IVA, il numero di fattura del fornitore e così via, poiché possono essere utili per le fatture esigibili. In [!INCLUDE[d365fin](../../includes/d365fin_md.md)],importiamo queste informazioni ma utilizziamo solo il numero di fattura del fornitore. Se si desidera utilizzare le altre informazioni, è possibile creare la propria personalizzazione.

## <a name="understanding-the-payment-reference"></a>Metodi del riferimento del pagamento
I processi di pagamento consistono nel pagare l'importo giusto alla parte giusta e semplificare la riconciliazione dei pagamenti con la chiusura dei conti in sospeso. L'estensione gestione fatture QR genera un riferimento di pagamento per le fatture emesse in una società specifica, il che significa che lo stesso riferimento di pagamento non può essere emesso più di una volta. Se anche il cliente sta usando [!INCLUDE[d365fin](../../includes/d365fin_md.md)], il riferimento di pagamento viene importato quando si ricevono fatture QR, trasferite alla pagina Voci di contabilità fornitori e utilizzate come riferimento durante la creazione di pagamenti fornitore. Per ulteriori informazioni, vedere [Ricevere Fatture QR](ui-extensions-qr-bill-management.md#receiving-qr-bills). Il flusso è simile alla precedente funzionalità di riferimento ESR che le fatture QR stanno sostituendo. Infine, il file di pagamento (pain.001) verrà inviato dall'app aziendale del cliente alla sua banca con il messaggio di trasferire gli importi sul conto del fornitore.  La banca produrrà un file di estratto conto cliente (camt.054) che il fornitore può importare per riconciliare i conti. Questo file includerà il riferimento di pagamento e viene importato tramite il Framework di scambio dati che viene aggiornato dall'estensione Gestione fatture QR per importare i file camt.054.  
Per i riferimenti ESR è possibile configurare informazioni, ad esempio, in modo che contengano il numero cliente e il numero di fattura. Non è possibile configurare il riferimento di pagamento nelle fatture QR. Ci sarà sempre una relazione 1: 1 tra una fattura QR emessa e un pagamento, il che semplifica la riconciliazione ed elimina la necessità di configurare il riferimento di pagamento sulle fatture QR. Pertanto, [!INCLUDE[d365fin](../../includes/d365fin_md.md)] utilizza un contatore univoco per il riferimento di pagamento.  Inoltre, è in atto la logica per bloccare due volte l'importazione o la scansione dello stesso riferimento di pagamento.

## <a name="scanning-and-importing-qr-bills"></a>Scansione ed importazione di fatture QR
Per analizzare o importare una fattura QR, è necessario utilizzare uno dei seguenti tipi di dispositivi di scansione:

* Uno scanner input che decodifica il codice QR e simula la tastiera per incollare il valore decodificato direttamente in un campo[!INCLUDE[d365fin](../../includes/d365fin_md.md)]. 
* Uno scanner in grado di decodificare il codice QR e salvarlo in un file .txt in cui si importa [!INCLUDE[d365fin](../../includes/d365fin_md.md)].  

> [!Note]
> Non è possibile importare direttamente le fatture QR ricevute come file PDF [!INCLUDE[d365fin](../../includes/d365fin_md.md)] poiché [!INCLUDE[d365fin](../../includes/d365fin_md.md)] non può interpretare i codici QR. È necessario utilizzare uno dei metodi di scansione.

## <a name="receiving-qr-bills"></a>Ricezione di fatture QR
Puoi ricevere le fatture QR in diversi luoghi in [!INCLUDE[d365fin](../../includes/d365fin_md.md)]:

* **Documenti in arrivo**, quando si desidera una fattura QR per avviare la creazione di un nuovo documento di acquisto o giornale di acquisto.
* **Ordini di acquisto e fatture di acquisto**, quando si desidera importare informazioni da una fattura QR a un documento di acquisto esistente e utilizzarlo per convalidare l'importo e la valuta e per memorizzare il riferimento di pagamento.
* **giornale di registrazione acquisti**, quando si desidera creare nuove righe giornale di registrazione acquisti acquisti in base a fatture QR. 

### <a name="to-receive-a-qr-bill-through-an-incoming-documents"></a>Per ricevere una fattura QR tramite documenti in arrivo
La ricezione di una fattura QR tramite documenti in arrivo è particolarmente utile quando il processo è automatizzato, ma è anche possibile ricevere manualmente una fattura QR tramite documenti in arrivo.

1. Scegliere l'![icona a forma di lampadina che consente di aprire la funzionalità delle informazioni](../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Documenti in entrata** e quindi scegliere il collegamento correlato.
2. Nella casella **Documenti in arrivo** creare una nuova voce selezionando **Nuovo**, quindi **Nuovo**. 
3. Nella casella **Documenti in Arrivo** inserisci una descrizione nel campo **Descrizione** .
4. Per importare la fattura QR selezionare**Azioni**, quindi **Fatture QR**, e **Scannerizza fattura QR** per scannerizzare una fattura QR nei documenti in entrata.
 
> [!TIP]
> Dopo aver importato la fattura QR, è possibile verificare la presenza di errori nella scheda dettaglio **Dettagli Corrispondenti**.

Dal documento in arrivo è possibile creare un giornale acquisti o una fattura acquisti e il riferimento di pagamento dalla fattura QR verrà assegnato a entrambi.

> [!Note]
> Quando si importano fatture QR, [!INCLUDE[d365fin](../../includes/d365fin_md.md)] proverà a trovare un conto bancario del fornitore con un IBAN o QR-IBAN corrispondente. Quando si importano fatture QR su documenti in arrivo e si crea in tal modo un documento o un registro di acquisto, il conto bancario del fornitore determinerà il fornitore da utilizzare. L'approccio del documento in arrivo aiuta a garantire l'assegnazione del fornitore corretto.

### <a name="receiving-a-qr-bill-through-purchase-order-or-purchase-invoice"></a>Ricezione di una fattura QR con un ordine di acquisto o fattura di acquisto
La ricezione di una fattura QR tramite un ordine di acquisto o una fattura di acquisto convalida l'importo della fattura e aggiunge il riferimento di pagamento ai movimenti contabili. Come i documenti in arrivo, è possibile acquisire o importare una fattura QR in un ordine di acquisto o in una fattura esistente. Questo processo utilizza il QR-IBAN o l'IBAN della fattura QR per trovare il fornitore con un numero corrispondente. Se non viene trovata alcuna corrispondenza, non è possibile acquisire o importare la fattura QR. In tal caso, è possibile creare il conto bancario del fornitore e quindi allegare la fattura QR al documento di acquisto. Quando la fattura QR viene scansionata o importata nel documento di acquisto, viene aggiunto l'importo, il riferimento di pagamento e altre informazioni dalla fattura QR. Viene utilizzato per la convalida prima di pubblicare il documento di acquisto. La registrazione verrà bloccata se l'importo dell'ordine o della fattura non corrisponde all'importo della fattura QR. La convalida avviene anche quando si esegue la scansione o l'importazione della fattura QR. Se il riferimento di pagamento è già utilizzato in un movimento contabile per un fornitore, verrà visualizzato un errore. I fornitori non possono emettere più fatture QR con lo stesso riferimento di pagamento. Allo stesso modo, verrà visualizzato un errore se la fattura QR e il riferimento di pagamento sono già stati importati in un documento di acquisto aperto. 

### <a name="receiving-a-qr-bill-through-a-purchase-journal"></a>Ricezione di una fattura QR con una giornale di registrazione acquisti
Puoi scansionare o importare fatture QR direttamente in una **giornale di registrazione acquisti**. Ciò è utile quando si desidera creare nuove righe di giornale di registrazione basate su una fattura QR. La scansione o l'importazione direttamente in una giornale di registrazione acquisti crea una nuova **riga giornale di registrazione acquisti acquisti** utilizzando il fornitore e l'importo dalla fattura QR e cerca di identificare il fornitore trovando un **Conto corrente fornitori** che ha un corrispondente IBAN o QR-IBAN. Ad esempio, l'utilizzo dei giornali di giornale di registrazione acquisti è utile se non si desidera utilizzare ordini di acquisto o fatture.

## <a name="reconciliation"></a>Riconciliazione
Quando si importano transazioni bancarie (camt) nella pagina Registrazione riconciliazione pagamenti, si presume che il file includa il riferimento di pagamento, che troverà automaticamente i corrispondenti **movimenti contabili clienti** da liquidare.    

## <a name="upcoming-capabilities-for-qr-bills"></a>Funzionalità in arrivo per fatture QR
Stiamo pianificando di aggiungere funzionalità all'estensione di gestione di fatture QR nei prossimi aggiornamenti alla versione 1 del 2020. Ad esempio, sarai in grado di ricevere fatture QR tramite documenti di acquisto e registro di acquisto. Ciò fornirà ulteriori convalide e consentirà di automatizzare e semplificare i processi di ricezione. Per informazioni su quando ciò accadrà, tieni d'occhio il nostro [Release Plan](https://docs.microsoft.com/dynamics365-release-plan/2020wave1/dynamics365-business-central/qr-bill-management-switzerland).

## <a name="see-also"></a>Vedere anche
[Funzionalità locale per la Svizzera](switzerland-local-functionality.md)  
