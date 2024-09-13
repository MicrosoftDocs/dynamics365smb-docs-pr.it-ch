---
title: Effettua pagamenti con AMC banking (USA) o bonifico SEPA (UE)
description: Elaborare i pagamenti ai fornitori esportando un file (EFT) con le informazioni di pagamento dalle righe registrazioni.
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: null
ms.search.form: '256, 1205, 1206, 1209, 10810, 10811'
ms.date: 08/26/2024
ms.author: bholtorf
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---
# Effettua pagamenti con l'estensione fondamentale AMC banking 365 o bonifico SEPA

Nella pagina  **Giornali di pagamento**, puoi elaborare i pagamenti ai tuoi fornitori esportando un file insieme alle informazioni di pagamento dalle righe del giornale. È quindi possibile caricare il file sul sito elettronico della banca dove vengono elaborati i trasferimenti di denaro correlati. [!INCLUDE[prod_short](includes/prod_short.md)] supporta il formato SEPA Credit Transfer, ma nel tuo paese/regione potrebbero essere disponibili altri formati per i pagamenti elettronici.

> [!NOTE]
> Nella versione generica di [!INCLUDE[prod_short](includes/prod_short.md)], viene installato e connesso un provider di servizi globale per convertire i dati bancari in qualsiasi formato di file richiesto dalla banca. Nelle versioni per il Nord America, lo stesso servizio può essere utilizzato per inviare file di pagamento come trasferimento elettronico di fondi (EFT), ad esempio la rete ACH (Automated Clearing House) comunemente utilizzata, tuttavia con un processo leggermente diverso. Vedere la sezione 6 [Per esportare pagamenti in un file della banca](finance-make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer.md#to-export-payments-to-a-bank-file).  

 Per abilitare i bonifici SEPA, è necessario innanzitutto impostare un conto corrente bancario, un fornitore e il batch registrazioni COGE su cui si basano le registrazioni pagamenti. Si preparano quindi i pagamenti ai fornitori compilando automaticamente la pagina  **Giornali di pagamento** con i pagamenti in scadenza con date di registrazione specificate.  

Dopo aver verificato che la banca ha elaborato i pagamenti, è possibile registrare le righe del giornale di pagamento.  

## Impostazione dell'estensione AMC Banking 365 Fundamentals 

Attiva l' AMC Banking 365 Fundamentals estensione per:

* Converti i file dell'estratto conto bancario in un formato che puoi importare.
* Converti i file di pagamento esportati nel formato richiesto dalla tua banca.

Per ulteriori informazioni, vedi [Usare l'estensione AMC Banking 365 Fundamentals](ui-extensions-amc-banking.md).

## Impostazione del bonifico SEPA

Dalla pagina  **Giornali di pagamento**, puoi esportare i pagamenti in un file da caricare sulla tua banca elettronica per l'elaborazione dei relativi trasferimenti di denaro. [!INCLUDE[prod_short](includes/prod_short.md)] supporta il formato SEPA Credit Transfer, ma nel tuo paese/regione potrebbero essere disponibili altri formati per i pagamenti elettronici.  

Per poter esportare un formato di file bancario non supportato di default in [!INCLUDE[prod_short](includes/prod_short.md)], è possibile impostare una definizione di scambio dati. Per ulteriori informazioni, vedere [Impostare le definizioni di scambio di dati](across-how-to-set-up-data-exchange-definitions.md).  

Prima di elaborare elettronicamente il pagamento esportando i file di pagamento in formato di bonifico SEPA, è necessario effettuare le seguenti operazioni di setup:  

* Impostare il conto corrente bancario in questione per gestire il formato del bonifico SEPA.  
* Impostare le schede fornitori per elaborare i pagamenti esportando i file nel formato di bonifico SEPA.  
* Impostare il batch di giornale generale correlato per abilitare l'esportazione dei pagamenti dalla pagina  **Giornali di pagamento**   
* Connettere la definizione di scambio dati per uno o più tipi di pagamento con uno o più metodi di pagamento rilevanti  

> [!NOTE]
> Business Central supporta sia il formato SEPA CT pain.001.001.03 che CT pain.001.001.09. Puoi scegliere qualsiasi formato nella pagina  **Conto bancario scheda** .  

> [!TIP]
> Questo articolo si applica alla versione generica di [!INCLUDE [prod_short](includes/prod_short.md)]. Nel tuo paese o regione, potrebbero essere stati aggiunti ulteriori campi obbligatori alle varie pagine. [!INCLUDE [tooltip-inline-tip_md](includes/tooltip-inline-tip_md.md)]

### Per impostare un conto bancario per il bonifico SEPA

1. Scegli la ![lampadina che apre la funzione Dimmi.](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immetti **Conti bancari**, quindi seleziona il collegamento correlato.  
2. Seleziona il conto bancario da cui esportare i file di pagamento nel formato bonifico SEPA.
3. Nella scheda dettaglio **Generale** nel campo **Nr. messaggi bonifico**, scegliere una serie numerica da cui i numeri vengono assegnati ai movimenti di bonifici SEPA.
4. Nella scheda rapida  **Comunicazione**, inserisci l'indirizzo e le informazioni di contatto della banca. 

   > [!NOTE]
   > È necessario compilare il campo  **Codice Paese/Regione** . Se il campo è vuoto, non è possibile esportare i pagamenti per l'account. Inoltre, il paese/regione deve avere un codice ISO valido.

5. Nella scheda dettaglio **Registrazione**, nel campo **Codice valuta**, specificare la valuta per il conto bancario.  

   > [!NOTE]  
   > Il campo **Codice valuta** deve essere impostato su **EUR**, perché i bonifici SEPA possono essere eseguiti solo in valuta EURO.  

6. Nella scheda rapida  **Trasferimento**, nel campo  **Formato di esportazione pagamento**, seleziona il formato SEPA che desideri utilizzare.  
7. Nel campo  **IBAN** specificare il numero di conto bancario internazionale per il conto.  

### Per impostare una scheda fornitore per il bonifico SEPA

1. Scegli la ![lampadina che apre la funzione Dimmi.](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immettere **Fornitori**, quindi selezionare il collegamento correlato.  
2. Aprire il file scheda del fornitore a cui si desidera effettuare il pagamento elettronico utilizzando i file di pagamento esportati nel formato bonifico SEPA.  
3. Nella scheda rapida **Pagamenti**, nel campo **Codice metodo di pagamento**, scegli **BANCA**.  
4. Nel campo  **Conto bancario preferito**, seleziona la banca a cui trasferire il denaro quando viene elaborato dalla tua banca elettronica.  

    Se non hai un account set di conti per questo fornitore, puoi crearne uno ora. Per ulteriori informazioni, vedi [Per impostare conti bancari fornitori per l'esportazione di file bancari](bank-how-setup-bank-accounts.md#to-set-up-vendor-bank-accounts-for-export-of-bank-files). Il valore nel campo **Conto bancario preferito** viene copiato nel campo **Conto bancario destinatario** nella pagina **Registrazioni pagamenti**.  

### Per impostare le registrazioni pagamenti fino per esportare i file di pagamento

1. Scegli la ![lampadina che apre la funzione Dimmi.](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immetti **Registrazioni pagamenti**, quindi scegli il collegamento correlato.  
2. Nel campo **Nome batch** scegliere il pulsante a discesa.  
3. Nella pagina **Batch registrazioni COGE** scegliere l'azione **Modifica lista**.  
4. Sulla riga del giornale di pagamento che utilizzi per esportare i pagamenti, Seleziona la casella di controllo  **Consenti esportazione pagamenti** .  

### Per connettere la definizione di scambio dati per uno o più tipi di pagamento con uno o più metodi di pagamento rilevanti

1. Scegli l'icona ![lampadina che apre la funzione Dimmi.](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immetti **Metodi di pagamento**, quindi scegli il collegamento correlato.  
2. Nella pagina **Metodi di pagamento** selezionare il metodo di pagamento che viene utilizzato per esportare i pagamenti e quindi scegliere il campo **Definizione righe esport. pagam.**.  
3. Nella pagina **Definizioni righe esportazione pagamento** selezionare il codice che è stato specificato nel campo **Codice** della Scheda dettaglio **Definizioni righe** nel passaggio 4 della sezione "Per descrivere la formattazione di righe e colonne nel file" della [Impostare le definizioni di scambio di dati](across-how-to-set-up-data-exchange-definitions.md).  

## Preparazione del giornale di pagamento

Compilare le registrazioni di pagamento con le righe per i pagamenti dovuti ai fornitori, con l'opzione di inserire le date di registrazione in base alla data di scadenza dei reltivi documenti di acquisto. Per ulteriori informazioni, vedere [Gestione della contabilità fornitori](payables-manage-payables.md).

## Esportazione dei pagamenti in un file bancario

Quando sei pronto a effettuare pagamenti ai tuoi fornitori o rimborsi ai tuoi dipendenti, puoi esportare un file con le informazioni di pagamento sulle righe della pagina  **Giornali di pagamento** . È quindi possibile caricare il file sulla banca per elaborare i relativi trasferimenti di denaro.

Nella versione generica di [!INCLUDE[prod_short](includes/prod_short.md)], l'estensione AMC Banking 365 Fundamentals è disponibile. Nelle versioni per il Nord America, la stessa estensione può essere utilizzata per inviare file di pagamento come trasferimento dei fondi elettronici (EFT), ma con un processo leggermente diverso. Vedere la sezione 6 [Per esportare pagamenti in un file della banca](finance-make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer.md#to-export-payments-to-a-bank-file).

> [!NOTE]  
> Prima di esportare i file di pagamento dalle registrazioni dei pagamenti, è necessario specificare il formato elettronico per il conto corrente bancario di interesse ed è necessario abilitare l'estensione AMC Banking 365 Fundamentals. Per ulteriori informazioni, vedi [Impostare i conti correnti bancari](bank-how-setup-bank-accounts.md) e [Usare l'estensione AMC Banking 365 Fundamentals](ui-extensions-amc-banking.md). Inoltre, è necessario selezionare la casella di controllo **Consenti esportazione pagamento** nella pagina **Batch registrazioni COGE**. Per ulteriori informazioni, vedere [Elaborazione delle registrazioni COGE](ui-work-general-journals.md).  

Utilizzare la pagina  **Registri dei trasferimenti di credito** per visualizzare i file di pagamento esportati dal giornale di pagamento. Da questa pagina è anche possibile riesportare i file di pagamento nel caso in cui si siano verificati errori tecnici o modifiche ai file. Tieni presente, tuttavia, che i file EFT esportati non vengono visualizzati in questa pagina e non possono essere riesportati.  

### Per esportare pagamenti in un file della banca

Nei passaggi seguenti viene descritto come pagare un fornitore tramite assegno. I passaggi sono simili al rimborso dei clienti tramite assegno.

1. Scegli l'icona ![lampadina che apre la funzione Dimmi.](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immetti **Registrazioni pagamenti**, quindi scegli il collegamento correlato.
2. Compilare le righe di registrazione pagamenti. Per ulteriori informazioni, vedere [Registrare pagamenti e rimborsi](payables-how-post-payments-refunds.md).

    > [!NOTE]
    > Se si utilizza EFT, è necessario selezionare **Pagamento elettronico** o **Pagamento elettronico IAT** nel campo **Tipo pagamento banca**. Servizi di esportazione file diversi e i rispettivi formati richiedono valori di configurazione differenti nelle pagine **Scheda conto corrente bancario** e **Scheda C/C bancari fornitori**. Si verrà informati sui valori di setup mancanti o non corretti mentre si tenta di esportare il file.
    >
    > La funzione EFT può essere utilizzata solo per i conti bancari nella valuta locale. Non può essere utilizzata con una valuta estera, indicata da un valore nel campo **Codice valuta**. Il valore del campo vuoto indica la valuta locale.

3. Dopo aver compilato tutte le righe del giornale di pagamento, selezionare l'azione  **Esporta** .
4. Nella pagina **Esporta pagamenti elettronici** compilare i campi secondo le necessità.

    I messaggi di errore vengono visualizzati nel riquadro informativo  **Errori file pagamento**, dove puoi anche scegliere un messaggio di errore per accedere a maggiori dettagli. È necessario risolvere tutti gli errori prima di poter esportare il file di pagamento.

    > [!TIP]  
    > Quando si utilizza l'estensione AMC Banking 365 Fundamentals, un messaggio di errore comune informa che il numero di conto corrente bancario non ha la lunghezza richiesta dalla banca. Per evitare o risolvere l'errore, è necessario rimuovere il valore nel campo **IBAN** nella pagina **Scheda conto corrente bancario**, quindi nel campo **Nr. conto bancario** , immettere un numero di conto corrente bancario nel formato richiesto dalla banca.

5. Nella pagina **Salva con nome** specificare il percorso in cui verrà esportato il file e scegliere **Salva**.

    > [!NOTE]  
    > Se si utilizza EFT, salvare il modulo della risultante rimessa del fornitore come documento di Word o selezionare in modo che venga inviato tramite posta elettronica direttamente al fornitore. I pagamenti sono ora aggiunti alla pagina **Genera file EFT** da cui è possibile generare più ordini di pagamento contemporaneamente per ridurre i costi di trasmissione. Per ulteriori informazioni, vedere i seguenti passaggi:
6. Nella pagina **Giornali di pagamento**, seleziona l'azione **Genera file EFT** .

    Nella pagina **Genera file EFT**, la scheda rapida **Righe** mostra tutti i pagamenti EFT esportati dal giornale di pagamento per un conto bancario ma non ancora generati.
7. Scegliere l'opzione l'azione **Genera file EFT** per esportare un file per tutti i pagamenti EFT.
8. Nella pagina **Salva con nome** specificare il percorso in cui verrà esportato il file e scegliere **Salva**.

Il file del pagamento bancario viene esportato nella posizione specificata. Puoi caricarlo sul tuo conto bancario elettronico ed effettuare i pagamenti effettivi. Sarà quindi possibile registrare le righe esportate delle registrazioni pagamenti.

### Per pianificare quando registrare i pagamenti esportati

Se non si desidera registrare una riga del giornale di pagamento per un pagamento esportato, è possibile semplicemente eliminare la riga del giornale. Ad esempio, perché stai aspettando la conferma che la banca ha elaborato la transazione. Successivamente, quando si crea una riga del giornale di pagamento per pagare l'importo rimanente, il campo  **Importo totale esportato** mostra la quota dell'importo del pagamento già esportata. Inoltre, è possibile trovare informazioni dettagliate sul totale esportato scegliendo il pulsante **Movimenti dei registri di bonifici** per visualizzare i dettagli relativi ai file di pagamento esportati.

Se non desideri registrare i pagamenti finché la banca non ne conferma l'elaborazione, puoi:

* In un giornale di pagamento con linee di pagamento suggerite, è possibile ordinare in base a **Esportato nel file di pagamento**  colonna o la **Importo totale esportato**  e quindi eliminare i suggerimenti di pagamento per le fatture aperte per le quali sono già stati effettuati pagamenti.
* Sul **Suggerisci pagamenti al fornitore**  pagina, dove si specifica quali pagamenti inserire nel giornale di pagamento, è possibile Seleziona il **Salta i pagamenti esportati**  casella di controllo se non si desidera inserire righe di giornale per i pagamenti già esportati.

Per visualizzare le informazioni sui pagamenti esportati, scegliere l'azione **Storico esportazione pagamento**.

### Per riesportare i pagamenti in un file della banca

È possibile riesportare i file di pagamento dalla pagina **Registri di bonifici**. Prima di eliminare o registrare le righe del giornale di pagamento, è anche possibile riesportare il file di pagamento dal **Giornali di pagamento**  pagina esportandola nuovamente. Se elimini o registri le righe del giornale di pagamento dopo l'esportazione, puoi riesportare lo stesso file di pagamento dall' **Registri di trasferimento dei crediti**  pagina. Selezionare la riga per il batch di bonifici che si desidera riesportare, quindi utilizzare l'azione **Riesporta pagamenti su file**.

> [!NOTE]  
> I file esportati EFT non sono visualizzati nella pagina **Registri di bonifici** e non possono essere riesportati.

1. Scegli l'icona ![lampadina che apre la funzionalità Dimmi.](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immetti **Registri di bonifici**, quindi seleziona il collegamento correlato.
2. Selezionare un'esportazione pagamento che si desidera riesportare quindi scegliere l'azione **Riesporta pagamenti su file**.

## Registrazione dei pagamenti

Dopo che la tua banca ha elaborato il pagamento elettronico, effettua il pagamento. Per ulteriori informazioni, vedere [Effettuare i pagamenti](payables-make-payments.md).

## Vedere anche

[Usare l'estensione AMC Banking 365 Fundamentals](ui-extensions-amc-banking.md)  
[Gestione della contabilità fornitori](payables-manage-payables.md)  
[Usare le registrazioni COGE](ui-work-general-journals.md)  
[Riscuotere pagamenti con addebito diretto SEPA](finance-collect-payments-with-sepa-direct-debit.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
