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
ms.date: 04/01/2020
ms.author: soalex
ms.openlocfilehash: 6cf85170efe4f2d415adc1b1db83699730a6ea60
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 04/01/2020
ms.locfileid: "3196420"
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
* **Ordini di acquisto e fatture di acquisto**, quando si desidera importare informazioni da una fattura QR a un documento di acquisto esistente e utilizzarlo per convalidare l'importo e la valuta e per memorizzare il riferimento di pagamento (questa funzionalità è prevista per l'aggiornamento di maggio 2020 di [!INCLUDE[d365fin](../../includes/d365fin_md.md)]).
* **Registrazione acquisti**, quando si desidera creare nuove righe giornale di registrazione acquisti in base a fatture QR (questa funzionalità è prevista per l'aggiornamento di maggio 2020 di [!INCLUDE[d365fin](../../includes/d365fin_md.md)]). 

### <a name="to-receive-a-qr-bill-through-an-incoming-documents"></a>Per ricevere una fattura QR tramite documenti in arrivo
La ricezione di una fattura QR tramite documenti in arrivo è particolarmente utile quando il processo è automatizzato, ma è anche possibile ricevere manualmente una fattura QR tramite documenti in arrivo.

1. Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "Icona della funzionalità Cerca pagina o report"), immettere **Documenti in entrata**, quindi scegliere il collegamento correlato.
2. Nella casella **Documenti in arrivo** creare una nuova voce selezionando **Nuovo**, quindi **Nuovo**. 
3. Nella casella **Documenti in Arrivo** inserisci una descrizione nel campo **Descrizione** .
4. Per importare la fattura QR selezionare**Azioni**, quindi **Fatture QR**, e **Scannerizza fattura QR** per scannerizzare una fattura QR nei documenti in entrata.
 
> [!TIP]
> Dopo aver importato la fattura QR, è possibile verificare la presenza di errori nella scheda dettaglio **Dettagli Corrispondenti**.

Dal documento in arrivo è possibile creare un giornale acquisti o una fattura acquisti e il riferimento di pagamento dalla fattura QR verrà assegnato a entrambi.

> [!Note]
> Quando si importano fatture QR, [!INCLUDE[d365fin](../../includes/d365fin_md.md)] proverà a trovare un conto bancario del fornitore con un IBAN o QR-IBAN corrispondente. Quando si importano fatture QR su documenti in arrivo e si crea in tal modo un documento o un registro di acquisto, il conto bancario del fornitore determinerà il fornitore da utilizzare. L'approccio del documento in arrivo aiuta a garantire l'assegnazione del fornitore corretto.

<!--

### Receiving a QR-Bill through Purchase Order or Purchase Invoice (Planned for May, 2020)
Receiving a QR-bill through a purchase order or purchase invoice validates the invoice amount and adds the payment reference to the ledgers. Like incoming documents, you can scan or import a QR-bill to an existing purchase order or invoice. This process uses the QR-IBAN or IBAN from the QR-bill to find the vendor with a matching number. If no match is found you cannot scan or import the QR-bill. If that happens, you can create the vendor bank account and then allow the QR-bill to be attached to the purchase document. When the QR-bill is scanned or imported to the purchase document it will add the amount, payment reference, and other information from the QR-bill. This is used for validation before posting the purchase document. Posting will be blocked if the amount of the order or invoice does not match the amount from the QR-bill. Validation also happens when you scan or import the QR-bill. If the payment reference is already used on a vendor ledger entry for a vendor, an error will display. Vendors cannot issue multiple QR-bills with the same payment reference. Similarly, an error will display if the QR-bill and payment reference has already been imported to an open purchase document. 

### Receiving a QR-Bill through a Purchase Journal (Planned for May, 2020)
You can scan or import QR-bills directly into a **Purchase Journal**. This is useful when you want to create new journal lines based on a QR-bill. Scanning or importing directly into a purchase journal creates a new **Purchase Journal Line** using the vendor and amount from the QR-bill, and tries to identify the vendor by finding a **Vendor Bank Account** that has a matching IBAN or QR-IBAN. For example, using purchase journals is useful if you do not want to use purchase orders or invoices.  -->

## <a name="reconciliation"></a>Riconciliazione
Quando si importano transazioni bancarie (camt) nella pagina Registrazione e riconciliazione pagamenti, si presume che il file includa <!--not sure what "assumed to include" means--> il riferimento di pagamento, che troverà automaticamente il corrispondente **Movimenti contabili clienti** per la liquidazione.    

## <a name="upcoming-capabilities-for-qr-bills"></a>Funzionalità in arrivo per fatture QR
Stiamo pianificando di aggiungere funzionalità all'estensione di gestione di fatture QR nei prossimi aggiornamenti alla versione 1 del 2020. Ad esempio, sarai in grado di ricevere fatture QR tramite documenti di acquisto e registro di acquisto. Ciò fornirà ulteriori convalide e consentirà di automatizzare e semplificare i processi di ricezione. Per informazioni su quando ciò accadrà, tieni d'occhio il nostro [Release Plan](https://docs.microsoft.com/dynamics365-release-plan/2020wave1/dynamics365-business-central/qr-bill-management-switzerland).

## <a name="see-also"></a>Vedere anche
[Funzionalità locale per la Svizzera](switzerland-local-functionality.md)  
