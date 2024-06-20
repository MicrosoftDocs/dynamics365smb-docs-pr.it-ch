---
title: 'Gestione fatture QR [CH]'
description: 'Questo articolo descrive i miglioramenti per l''estensione Gestione fatture QR e come è possibile utilizzare Business Central per generare, inviare e importare facilmente le fatture QR.'
author: sorenfriisalexandersen
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'QR-bill, invoice, incoming documents, payment reference'
ms.search.form: '11502, 11510, 11511, 11512, 11513, 11514, 11515, 11516, 11517, 11518'
ms.date: 04/05/2023
ms.author: soalex
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---
# <a name="qr-bill-management-in-the-swiss-version-of-business-central"></a>Gestione fatture QR nella versione svizzera di Business Central

Dal 1° luglio 2020, le società svizzere devono essere in grado di ricevere le fatture QR. Le fatture QR sono distinte di pagamento che seguono le fatture e fanno parte di un'iniziativa a livello nazionale per semplificare i processi di pagamento. Le fatture QR sostituiscono tutte le distinte di pagamento esistenti e le funzionalità relative a PVR. Contengono tutte le informazioni necessarie per effettuare i pagamenti e un codice QR sulla distinta di pagamento semplifica l'importazione delle informazioni [!INCLUDE[prod_short](../../includes/prod_short.md)]. Tutte le informazioni rilevanti vengono importate e utilizzate per generare pagamenti per il fornitore che ha inviato la fattura QR, incluso il riferimento di pagamento, che viene automaticamente incluso nelle voci dei movimenti contabili fornitori ed esportato nei file di pagamento alla banca.

## <a name="get-started-with-the-qr-bill-management-extension"></a><a name="get-started"></a>Inizia con l'estensione Gestione fattura QR

L'estensione Gestione fattura QR è inclusa e installata automaticamente in [!INCLUDE[prod_short](../../includes/prod_short.md)]. Per iniziare con l'estensione, è necessario apportare alcune modifiche alla configurazione [!INCLUDE[prod_short](../../includes/prod_short.md)]. Un modo semplice per eseguire questa operazione è scegliere l'![icona a forma di lampadina che consente di aprire la funzionalità delle informazioni.](../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immetti **Setup fattura QR**, quindi seleziona il collegamento correlato. La guida ti aiuta a inserire informazioni, come:

* Specifica se utilizzare il tuo IBAN o QR-IBAN. Il QR-IBAN è un IBAN che contiene un numero compreso tra 30000 e 31999 sulle posizioni da 5 a 9, ad esempio *CH55 30024 123456789012*.
* Definisci come visualizzare nomi e indirizzi sulle fatture QR e utilizzare la codifica dei caratteri Umlaut tedeschi. Ti consigliamo di utilizzare i valori predefiniti.
* Seleziona il **Layout fattura QR predefinito**. Il layout determina se utilizzare IBAN o QR-IBAN, se il tipo di riferimento è creditore o riferimento QR e se includere le informazioni di fatturazione nel formato SWICO.
* Abilita le fatture di vendita e assistenza e i metodi di pagamento per le fatture QR.
* Specificare la definizione registrazioni e il batch registrazioni da utilizzare per la generazione di registro acquisti da fatture QR scansionate o importate.

Se necessario, è possibile modificare le impostazioni di layout nella pagina **Layout fattura QR**.

## <a name="issuing-qr-bills"></a>Emissione di fatture QR

È possibile abilitare le fatture QR per le fatture di vendita e assistenza. Questa opzione aggiunge una voce alla pagina **Selezione report - Vendite** che genera un PDF aggiuntivo con la fattura QR quando vengono generate le fatture. Per abilitare la funzione scegli il campo **Tipi di documento abilitati per le fatture QR** nella pagina **Setup fattura QR** e attiva i tipi di documento desiderati selezionando la casella appropriata nella colonna **Abilitato**.

## <a name="adding-billing-information-to-qr-bills"></a>Aggiunta di informazioni di fatturazione a fatture QR

Quando si crea una fattura QR, è possibile includere le informazioni di fatturazione nel formato SWICO, come richiesto da SIX, il fornitore svizzero di infrastrutture di pagamento. Idealmente, anche le applicazioni aziendali che producono o importano fatture QR dovrebbero essere in grado di elaborare informazioni quali l'importo dell'IVA, il numero di fattura del fornitore e così via, poiché possono essere utili per le fatture esigibili. In [!INCLUDE[prod_short](../../includes/prod_short.md)],importiamo queste informazioni ma utilizziamo solo il numero di fattura del fornitore. È necessario personalizzare se vuoi includere altre informazioni.

## <a name="understanding-the-payment-reference"></a>Metodi del riferimento del pagamento

I processi di pagamento consistono nel pagare l'importo giusto alla parte giusta e semplificare la riconciliazione dei pagamenti con la chiusura dei conti in sospeso. L'estensione gestione fatture QR gestisce questi processi generando un riferimento di pagamento per le fatture emesse in una società specifica, il che significa che lo stesso riferimento di pagamento non può essere emesso più di una volta.  

Se anche il cliente sta usando [!INCLUDE[prod_short](../../includes/prod_short.md)], il riferimento di pagamento viene importato quando si ricevono fatture QR, trasferite alla pagina **Voci di contabilità fornitori** e utilizzate come riferimento durante la creazione di pagamenti fornitore. Per ulteriori informazioni, vedi [Ricevere Fatture QR](ui-extensions-qr-bill-management.md#receiving-qr-bills).

Il flusso è simile alla precedente funzionalità di riferimento ESR che le fatture QR stanno sostituendo. Infine, il file di pagamento (pain.001) viene inviato dall'app aziendale del cliente alla sua banca con il messaggio di trasferire gli importi sul conto del fornitore. La banca produce un file di estratto conto cliente (camt.054) che il fornitore può importare per riconciliare i conti. Questo file include il riferimento di pagamento e viene importato tramite il Framework di scambio dati che viene aggiornato dall'estensione Gestione fatture QR per importare i file camt.054.

Per i riferimenti ESR è possibile configurare informazioni, ad esempio, in modo che includano il numero cliente e il numero di fattura. Non è possibile configurare il riferimento di pagamento nelle fatture QR. Ci sarà sempre una relazione 1: 1 tra una fattura QR emessa e un pagamento, il che semplifica la riconciliazione ed elimina la necessità di configurare il riferimento di pagamento sulle fatture QR. Pertanto, [!INCLUDE[prod_short](../../includes/prod_short.md)] utilizza un contatore univoco per il riferimento di pagamento.  Inoltre, è in atto la logica per bloccare due volte l'importazione o la scansione dello stesso riferimento di pagamento.

### <a name="formats-for-qr-references-and-creditor-references"></a><a name="formats"></a>Formati per riferimenti QR e riferimenti creditori

Il riferimento QR è composto da 26 posizioni numeriche più una cifra di controllo.  

Il riferimento creditore ISO (ISO 11649) consente al creditore di effettuare confronti automatici tra le proprie fatture e i pagamenti in entrata. Deve includere il valore *SC* in posizione 1-2 e un carattere di test corretto in posizione 3-4 e può includere fino a un massimo di 25 caratteri.  

## <a name="using-multiple-bank-accounts-as-issuers-of-qr-bills"></a><a name="multiplebankaccounts"></a>Utilizzo di più conti bancari per emettere fatture QR

Coloro che emettono fatture QR possono utilizzare più conti bancari per instradare i pagamenti su conti bancari diversi. Questo è legato al metodo di pagamento in cui specifichi il **Nr. conto bancario fattura QR** Quando specificato, le informazioni IBAN/QR-IBAN di questo conto bancario verranno utilizzate sulle fatture QR che utilizzano il metodo di pagamento indicato. In questo modo puoi indirizzare i pagamenti in entrata sul conto bancario desiderato. Se non utilizzi più conti bancari e specifichi il **numero di conto bancario fattura QR** sulla scheda **Metodi di pagamento**, le informazioni QR-IBAN/IBAN dalla pagina **Informazioni società** vengono utilizzate sulle fatture QR. Assicurati di aver impostato almeno le informazioni del tuo conto bancario principale. Per ulteriori informazion, vedi [Impostare i conti correnti bancari](../../bank-how-setup-bank-accounts.md).

> [!NOTE]
> Se emetti fatture QR, imposta i conti bancari in modo che i conti giusti vengano visualizzati ai clienti, a seconda che utilizzi il QR-IBAN o l'IBAN regolare. Se sei il destinatario e il pagante di fatture QR, ti consigliamo di impostare correttamente i conti bancari dei fornitori per il pagamento e il trasferimento nei conti con IBAN regolare o QR-IBAN.

### <a name="adding-a-qr-iban-to-a-new-or-existing-bank-account"></a>Aggiunta di un QR-IBAN a un conto bancario nuovo o esistente

Per utilizzare un QR-IBAN diverso da quello impostato nella pagina **Informazioni società**, specifica i dati del conto bancario nella **Scheda conto bancario**:

1. Scegliere la ![lampadina che apre la funzionalità delle informazioni.](../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immetti **Conti bancari**, quindi seleziona il collegamento correlato.
2. Nell'elenco **Metodi di pagamento** scegli l'azione **Nuovo** o **Modifica**.
3. Nella Scheda dettaglio **Trasferimento**, immetti il conto bancario nel campo **QR-IBAN**.

## <a name="scanning-and-importing-qr-bills"></a>Scansione ed importazione di fatture QR

Per analizzare o importare una fattura QR, è necessario utilizzare uno dei seguenti tipi di dispositivi di scansione:

* Uno scanner input che decodifica il codice QR e simula la tastiera per incollare il valore decodificato direttamente in un campo[!INCLUDE[prod_short](../../includes/prod_short.md)]. 
* Uno scanner in grado di decodificare il codice QR e salvarlo in un file .txt che importi in [!INCLUDE[prod_short](../../includes/prod_short.md)]. 

> [!NOTE]
> Non è possibile importare direttamente le fatture QR ricevute come file PDF [!INCLUDE[prod_short](../../includes/prod_short.md)] poiché [!INCLUDE[prod_short](../../includes/prod_short.md)] non può interpretare i codici QR. È necessario utilizzare uno dei metodi di scansione precedenti.

## <a name="receiving-qr-bills"></a>Ricezione di fatture QR

Puoi ricevere le fatture QR in diversi luoghi in [!INCLUDE[prod_short](../../includes/prod_short.md)]:

* **Documenti in arrivo**, quando si desidera una fattura QR per avviare la creazione di un nuovo documento di acquisto o giornale di acquisto.
* **Ordini di acquisto e fatture di acquisto**, quando si desidera importare informazioni da una fattura QR a un documento di acquisto esistente e utilizzarlo per convalidare l'importo e la valuta e per memorizzare il riferimento di pagamento.
* **giornale di registrazione acquisti**, quando si desidera creare nuove righe giornale di registrazione acquisti acquisti in base a fatture QR. 

### <a name="receiving-a-qr-bill-through-an-incoming-document"></a>Ricezione di una fattura QR tramite un documento in arrivo

La ricezione di una fattura QR tramite documenti in arrivo è particolarmente utile quando il processo è automatizzato, ma è anche possibile ricevere manualmente una fattura QR tramite documenti in arrivo.

1. Scegli la ![lampadina che apre la funzionalità delle informazioni.](../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immettere **Documenti in arrivo**, quindi selezionare il collegamento correlato.
2. Nella casella **Documenti in arrivo** creare una nuova voce selezionando **Nuovo**, quindi **Nuovo**.
3. Nella casella **Documenti in Arrivo** inserisci una descrizione nel campo **Descrizione** .
4. Per importare la fattura QR, scegli una delle seguenti azioni:
   * **Esegui scansione fattura QR** per eseguire la scansione di una fattura QR nel documento in entrata.
   * **Importa file di fattura QR sottoposta a scansione** per utilizzare un file generato dal secondo tipo di scanner descritto nella sezione [Scansione ed importazione di fatture QR](#scanning-and-importing-qr-bills).

> [!TIP]
> Dopo aver importato la fattura QR, è possibile verificare la presenza di errori nella scheda dettaglio **Dettagli Corrispondenti**.

Dal documento in arrivo è possibile creare un giornale acquisti o una fattura acquisti e il riferimento di pagamento dalla fattura QR viene assegnato a entrambi. Per ulteriori informazioni, vedi [Utilizzo dei documenti in entrata](../../across-income-documents.md).

> [!NOTE]
> Quando si importano fatture QR, [!INCLUDE[prod_short](../../includes/prod_short.md)] cerca un conto bancario del fornitore con un IBAN o QR-IBAN corrispondente. Quando importi le fatture QR in documenti in arrivo, un documento o un giornale di registrazione di acquisto viene creato e il conto bancario del fornitore determina il fornitore da utilizzare. L'approccio del documento in arrivo aiuta a garantire l'assegnazione del fornitore corretto. 

#### <a name="receiving-through-the-kofax-ocr-service"></a>Ricezione tramite il servizio Kofax OCR

> [!NOTE]
> Se le aziende esistenti in [!INCLUDE[prod_short](../../includes/prod_short.md)] desiderano che venga restituito un riferimento QR quando utilizzano il servizio Kofax OCR, devono aggiornare la definizione di scambio di dati esistente utilizzata come **Tipo scambio dati** per l'elaborazione delle fatture nei documenti in entrata.  

Completa i passaggi seguenti per aggiornare una definizione di scambio di dati esistente. 

1. Seleziona la ![lampadina che apre la funzionalità delle informazioni.](../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immetti **definizioni di scambio dati**, quindi seleziona il collegamento correlato. 
2. Nella lista **definizioni di scambio dati**, trova la riga che desideri aggiornare e apri la scheda. 
3. Nella Scheda dettaglio **Definizioni righe** seleziona **OCRINVHEADER**.  
4. Nella scheda dettaglio **Definizioni colonne** crea una nuova riga e immetti i seguenti valori.

    | Campo | Valore |
    |-------|-------|
    | **Nr. colonna** | 11513 |
    | **Nome** | Nr. riferimento fattura QR Svizzera |
    | **Descrizione** | Nr. riferimento fattura QR Svizzera |
    | **Percorso** | /Document/HeaderFields/HeaderField\[Type\[text()='qrreference'\]\]/Text |
    
5. Nella Scheda dettaglio **Definizioni righe** seleziona **Mapping dei campi**.  
6. Nella pagina **Mapping dei campi** crea una nuova riga e immetti i seguenti valori.

    | Campo | Valore |
    |-------|-------|
    | **Nr. colonna** | 11513 |
    | **ID tabella di destinazione** | 38 |
    | **ID campo di destinazione** | 171 |
    | **Solo convalida** | False |

7. Chiudi le pagine.  

### <a name="receiving-a-qr-bill-through-purchase-orders-or-purchase-invoices"></a>Ricezione di una fattura QR con ordini di acquisto o fatture di acquisto

La ricezione di una fattura QR tramite un ordine di acquisto o una fattura di acquisto convalida l'importo della fattura e aggiunge il riferimento di pagamento ai movimenti contabili. Come i documenti in arrivo, è possibile acquisire o importare una fattura QR in un ordine di acquisto o in una fattura esistente. Questo processo utilizza il QR-IBAN o l'IBAN della fattura QR per trovare il fornitore con un numero corrispondente. Se non viene trovata alcuna corrispondenza, non puoi eseguire la scansione o importare la fattura QR, quindi dovrai creare il conto bancario del fornitore e quindi consentire che la fattura QR sia allegata al documento di acquisto.

* Per aggiungere una fattura QR a un documento di acquisto esistente, seleziona il documento di destinazione e quindi scegli l'azione **Esegui scansione fattura QR** o **Importa file di fattura QR sottoposta a scansione** nella pagina **Ordini di acquisto** o **Fatture di acquisto**.

Quando la fattura QR viene scansionata o importata nel documento di acquisto, viene aggiunto l'importo, il riferimento di pagamento e altre informazioni dalla fattura QR. Questi dati sono utilizzati per convalidare il documento di acquisto prima della pubblicazione. La registrazione è bloccata se l'importo dell'ordine o della fattura non corrisponde all'importo della fattura QR. La convalida avviene anche quando si esegue la scansione o l'importazione della fattura QR. Se si carica una fattura QR non contenente l'**importo**, per esempio una fattura QR decodificata che ha una riga vuota dove dovrebbe comparire l'importo, dopo il caricamento la sezione **fattura QR** viene indicata sulla pagina **fattura acquisto**. Il campo **importo** della sezione **fattura QR** può essere modificato ed è possibile aggiungervi l'importo appropriato. Se una fattura QR caricata ha un valore nel campo **importo**, questo viene automaticamente impostato in base al campo **importo** della sezione **fattura QR**, ma il campo può ancora essere modificato.  

Se il riferimento di pagamento è già utilizzato in un movimento contabile per un fornitore, si verifica un errore. I fornitori non possono emettere più fatture QR con lo stesso riferimento di pagamento. Allo stesso modo, si verifica un errore se la fattura QR e il riferimento di pagamento sono già stati importati in un documento di acquisto aperto.

### <a name="receiving-a-qr-bill-through-a-purchase-journal"></a>Ricezione di una fattura QR con una giornale di registrazione acquisti

Puoi scansionare o importare fatture QR direttamente in una giornale di registrazione acquisti. Questa opzione è utile quando si desidera creare nuove righe di giornale di registrazione basate su una fattura QR. La scansione o l'importazione direttamente in una giornale di registrazione acquisti crea una nuova **riga giornale di registrazione acquisti acquisti** utilizzando il fornitore e l'importo dalla fattura QR e cerca di identificare il fornitore trovando un **Conto corrente fornitori** con un corrispondente IBAN o QR-IBAN. Ad esempio, l'utilizzo dei giornali di giornale di registrazione acquisti è utile se non vuoi utilizzare ordini di acquisto o fatture.

1. Scegli la ![lampadina che apre la funzionalità delle informazioni.](../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immetti **Registrazioni acquisti**, quindi seleziona il collegamento correlato.
2. Nell'elenco **Registrazioni acquisti**, crea una nuova voce scegliendo una delle seguenti azioni:
   * **Esegui scansione fattura QR** per eseguire la scansione di una fattura QR nel documento in entrata.
   * **Importa file di fattura QR sottoposta a scansione** per utilizzare il file generato dal secondo tipo di scanner descritto nella sezione [Scansione ed importazione di fatture QR](#scanning-and-importing-qr-bills).

## <a name="reconciliation"></a>Riconciliazione

Quando si importano transazioni bancarie (camt) nella pagina **Registrazioni riconciliazione pagamenti**, si presume che il file includa il riferimento di pagamento e che troverà automaticamente i corrispondenti **Movimenti contabili clienti** per liquidare la transazione.

## <a name="see-also"></a>Vedere anche

[Pagamenti elettronici svizzeri](swiss-electronic-payments.md)  
[Funzionalità locale per la Svizzera](switzerland-local-functionality.md)  

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
