---
title: Configurare e usare il connettore Shopify
description: Vari scenari di integrazione per dimostrare il flusso di lavoro tra Shopify e Business Central
ms.date: 08/30/2024
ms.topic: article
ms.service: dynamics-365-business-central
ms.search.form: '30101, 30102, 30106, 30107, 30113, 30115, 30126, 30156, 30157'
ms.reviewer: bholtorf
author: brentholtorf
ms.author: bholtorf
---

# <a name="walkthrough-set-up-and-use-the-shopify-connector"></a>Procedura dettagliata: configurare e usare il connettore Shopify

Questa sezione illustra alcuni scenari tipici e illustra i passaggi per testare o addestrare gli utenti sul flusso di lavoro di [!INCLUDE[prod_short](../includes/prod_short.md)] e del punto vendita Shopify integrato.

## <a name="prerequisites"></a>Prerequisiti

### <a name="shopify"></a>Shopify

Devi avere:

- Un account Shopify
- Un negozio online con Shopify

Scopri di più su come creare valutazioni di prova e impostazioni consigliate Shopify in [Creare e configurare un account Shopify](shopify-account.md).

### <a name="business-central"></a>Business Central

È necessario avere un account [!INCLUDE[prod_short](../includes/prod_short.md)].

Ad esempio, puoi creare un account demo o avviare una valutazione. Per ulteriori informazioni, vedi [Preparare ambienti dimostrativi di Dynamics 365 Business Central](/dynamics365/business-central/dev-itpro/administration/demo-environment) e [Iscriversi per la versione di valutazione](../trial-signup.md). 

## <a name="connect-business-central-to-the-shopify-shop"></a>Collegamento di Business Central al punto vendita Shopify

In [!INCLUDE[prod_short](../includes/prod_short.md)] esegui le operazioni seguenti:

1. Seleziona l'icona ![lampadina che apre la funzionalità Dimmi](../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), e immetti **Punti vendita Shopify**, quindi seleziona il collegamento correlato.
2. Seleziona l'azione **Nuovo**.
3. Nel campo **Codice** immetti **DEMO1**.
4. Nel campo **URL Shopify**, immetti l'URL per il punto vendita online a cui desideri connetterti.
5. Attiva l'interruttore **Abilitato** quindi rivedi e accetta i termini e le condizioni.

Per configurare il punto vendita Shopify, esegui i passaggi seguenti:

1. Disattiva l'interruttore **Consenti sincronizzazioni in background**.
2. Seleziona *A Shopify* nel campo **Sincronizza articolo**.
3. Seleziona *A Shopify* nel campo **Sincronizza immagini articolo**.
4. Abilita l'interruttore **Sincronizza attributi articolo**.
5. Abilita l'interruttore **Inventario tracciato**.
6. Seleziona *Nega* nel campo **Criterio di inventario predefinito**.
7. Abilita l'interruttore **Crea automaticamente clienti sconosciuti**.
8. Compila il campo **Codice modello cliente/società** con il modello appropriato.
9. Compila il campo **Conto costo spedizione**, **Conto mance** con il conto ricavi. Ad esempio, negli Stati Uniti, utilizzare **40210**.
10. Abilita l'interruttore **Creazione automatica degli ordini**.
11. Disattiva l'interruttore **Rilascia automaticamente ordini vendita**.

Configurare il mapping della posizione:

1. Seleziona l'azione **Posizioni** per aprire **Posizioni punto vendita Shopify**.
2. Seleziona l'azione **Ottieni ubicazioni Shopify** per importare tutte le posizioni definite in Shopify. Seleziona la voce con l'interuttore **Primario** selezionato.
3. Nel **filtro posizione**, inserisci **''|EAST|MAIN**.
4. Per abilitare la sincronizzazione dell'inventario per una posizione selezionata, nel campo  Shopify Calcolo scorte **, Seleziona** Saldo disponibile previsto per oggi **.**

## <a name="walkthrough-start-selling-products-online"></a>Procedura dettagliata: iniziare a vendere prodotti online

### <a name="scenario"></a>Scenario

Supponiamo che tu voglia provare Shopify come punto vendita online senza dedicare molto tempo alla configurazione, soprattutto perché mantieni già i tuoi articoli in [!INCLUDE[prod_short](../includes/prod_short.md)] correttamente. Dopo aver lanciato il tuo punto vendita online Shopify, ottieni immediatamente nuovi clienti che sono soddisfatti del tuo punto vendita e della loro esperienza di acquisto. Quindi, decidono di lasciare mance alla cassa.

### <a name="steps"></a>Passaggi

In [!INCLUDE[prod_short](../includes/prod_short.md)], attieniti alla seguente procedura:

1. Seleziona l'icona ![lampadina che apre la funzionalità Dimmi](../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immetti **Prodotti Shopify** e scegli il collegamento correlato.
2. Seleziona **Aggiungi articoli**.
3. Nel campo  **Codice negozio**, inserisci  **DEMO1**.
4. Nel campo **Codice categoria articolo**, imposta il filtro **SEDIA**.
5. Attiva l'interruttore **Sincronizza immagini prodotto**.
6. Attiva l'interruttore **Sincronizza inventario**.
7. Seleziona **OK** e attendi che la sincronizzazione iniziale di articoli, prezzi, immagini e inventario sia completata.

Nel **punto vendita online Shopify**:
> [!Tip]  
> Apri **Amministrazione Shopify**, accedendo all'URL specificato nel campo **URL** della pagina **Scheda punto vendita Shopify**. Seleziona l'icona a forma di occhio accanto al canale di vendita **Punto vendita online**, situato nella barra laterale di **Amministrazione Shopify**. 

Apri il catalogo dei prodotti. Avviso:

* Titoli, immagini e prezzi dei prodotti.
* Indicatore di disponibilità (esaurito in caso di esaurimento scorte).

Scegli un prodotto qualsiasi che possa essere venduto. Ad esempio, la **sedia girevole BERLIN, gialla**. Nota che la descrizione contiene gli attributi dell'articolo.

Seleziona **Compralo subito** e procedi alla fase di pagamento.

1. Nel campo  **Indirizzo e-mail o numero di cellulare**, inserisci  **cl@contoso.com** (oppure un indirizzo e-mail dove desideri ricevere le conferme di ordine e spedizione).
2. Nei campi **Nome** e **Cognome**, inserisci **Claudia** e **Lawson**.
3. Inserisci l'indirizzo locale.
4. Seleziona la casella di controllo **Salva queste informazioni per la prossima volta**.
6. Mantieni *Standard* come metodo di spedizione.
8. Nel campo  **Numero di credito scheda**, inserisci  **1** se utilizzi  **(per il test) Bogus Gateway**, oppure inserisci  **5555 5555 5555 4444** se utilizzi  **Shopify pagamenti** in modalità test.
9. Compila il campo **Nome sulla scheda**.
10. Nel campo **Data di scadenza**, immetti il mese e l'anno corrente.
11. Nel **Codice di sicurezza**, inserisci **111**.
12. Facoltativo: Seleziona **mancia del 10%** .
13. Seleziona **Paga adesso**.

In [!INCLUDE[prod_short](../includes/prod_short.md)], effettua i seguenti passaggi:

1. Seleziona l'icona ![lampadina che apre la funzionalità Dimmi](../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immetti **Ordini Shopify**, quindi scegli il collegamento correlato.
2. Seleziona l'azione **Sincronizza ordini da Shopify**.
3. Seleziona **OK**.

L'ordine importato è pronto per l'elaborazione.

1. Seleziona l'ordine importato per aprire la finestra **Ordine Shopify**.
2. Nota che vengono creati il nuovo cliente e nuovi ordini cliente.
3. Esplora le azioni  **Rischi** e  **Costi di spedizione** .
4. Seleziona **Ordine vendita** per aprire la finestra **Ordine vendita** L'ordine cliente è una domanda che, se necessario, può essere soddisfatta con l'assemblaggio, la produzione o l'acquisto con l'ausilio del motore di pianificazione. Supporta inoltre vari processi di gestione del magazzino con completa separazione dei compiti.
6. Nel campo  **Agente** immettere  **DHL**. Riapri l'ordine, se necessario, scegliendo l'azione **Riapri**.
7. Nel  **Numero di tracciamento del pacco**, inserisci **123456789**.
8. Seleziona **Registra**, l'opzione **Spedisci e fattura**, quindi il pulsante **OK**.

Ora i dati fisici e finanziari sono registrati in [!INCLUDE[prod_short](../includes/prod_short.md)]. È ora di inviare una notifica a Shopify relativa alle modifiche.

1. Seleziona l'icona ![lampadina che apre la funzionalità Dimmi](../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), icona, immetti **Sincronizza spedizioni con Shopify**, quindi seleziona il collegamento correlato.
2. Seleziona **OK**.

In **Amministrazione Shopify** nota che l'ordine è ora contrassegnato come *Completato*. Puoi anche rivedere i dettagli della spedizione e vedere l'URL di tracciamento lì. Se esegui **Sincronizza ordini da Shopify** di nuovo, l'ordine verrà archiviato in entrambi i sistemi.

## <a name="walkthrough-add-your-customers-to-your-new-online-store"></a>Procedura dettagliata: aggiungere i clienti al nuovo punto vendita online

### <a name="scenario-1"></a>Scenario

Dopo un avvio rapido di successo del tuo nuovo punto vendita online, desideri che i tuoi attuali clienti lo visitino e inizino a effettuare ordini. A seconda del piano e del processo Shopify, puoi provare i flussi B2B e DTC

### <a name="dtc-steps"></a>Passaggi per DTC

In [!INCLUDE[prod_short](../includes/prod_short.md)] esegui le operazioni seguenti:

1. Seleziona l'icona ![lampadina che apre la funzionalità Dimmi](../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immetti **Clienti Shopify**, quindi seleziona il collegamento correlato.
2. Seleziona **Aggiungi clienti**.
3. Nel campo  **Codice negozio**, inserisci  **DEMO1**.
4. Nel campo **Nr.** Campo, impostare il filtro **20000**.
5. Seleziona **OK** e attendi il completamento della sincronizzazione iniziale dei clienti.

In **Amministrazione Shopify** nota che il cliente è stato importato. Apri i clienti e nota che il nome e il cognome del cliente provengono dal campo **Nome contatto** di **Scheda cliente**. Il nome della società si trova nell'indirizzo predefinito, collegato al cliente. Se utilizzi  **Account cliente classici**, puoi Seleziona **Invia invito account** per invitare il cliente. Con i **nuovi account cliente**, i clienti non hanno bisogno di una password per effettuare l'accesso. Invece, Shopify consente ai tuoi clienti di accedere utilizzando un codice di verifica monouso di 6 cifre inviato via e-mail. 

### <a name="b2b-steps"></a>Fasi B2B

[!INCLUDE [shopify-preview](../includes/shopify-preview.md)]

In [!INCLUDE[prod_short](../includes/prod_short.md)] esegui le operazioni seguenti:

1. Seleziona l'icona ![lampadina che apre la funzionalità Dimmi](../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immetti **Società Shopify**, quindi seleziona il collegamento correlato.
2. Seleziona **Aggiungi società**.
3. Nel campo Negozio **Codice**, inserisci **DEMO1**.
4. Imposta il filtro **30000** sul **N.** .
5. Seleziona **OK** e attendi il completamento della sincronizzazione iniziale dei clienti.

In  **Shopify Amministrazione**, notare che sono stati importati sia l'azienda che il cliente. Apri i clienti e nota che il riquadro Informazioni aziendali contiene collegamenti all'azienda, alla posizione e alle autorizzazioni assegnate.
Per invitare il cliente, Seleziona **[...]** nel  **Riquadro informativo** Azienda, quindi Seleziona **Invia e-mail di accesso B2B**.

## <a name="walkthrough-fine-tuning-of-item-management"></a>Procedura dettagliata: messa a punto della gestione degli elementi

### <a name="scenario-2"></a>Scenario

Ti piacerà aggiungere maggiore flessibilità e controllo ai tuoi processi relativi alla gestione degli articoli. Desideri migliorare le descrizioni dei prodotti e aggiungere ulteriori passaggi di revisione prima che i prodotti diventino disponibili per tutti i clienti.

### <a name="steps-1"></a>Passaggi

In [!INCLUDE[prod_short](../includes/prod_short.md)] esegui le operazioni seguenti:

Preparare i dati.

1. Seleziona l'icona ![lampadina che apre la funzionalità Dimmi](../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), , immetti **Gruppo di prezzi per clienti** e seleziona il relativo collegamento.
2. Aggiungi nuovo gruppo di prezzo. Nel campo  **Codice**, inserisci  **SHOPIFY**.
3. Chiudi la finestra **Gruppo prezzi cliente**.
4. Seleziona l'icona ![lampadina che apre la funzionalità Dimmi](../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immetti **Articoli** e seleziona il collegamento correlato.
5. Seleziona oggetto **1896-S, Athens Desk**, e quindi seguire questi passaggi:

6. Seleziona l'azione **Varianti** e quindi aggiungi due varianti: **PREMIUM, Athens Desk, edizione Premium** e **ESSENTIAL, Athens Desk, edizione Essential**.
7. Seleziona l'azione **Testo di marketing** e utilizza  **Bozza con Copilot** per ottenere un testo creativo e accattivante. Se il suggerimento di testo di marketing non è abilitato, inserisci semplicemente: '**Design semplice ed elegante** si adatta a qualsiasi abbigliamento. *Disponibile in due edizioni.*.
8. Seleziona l'azione **Prezzi vendita** e aggiungi nuovi prezzi come mostrato nella seguente tabella:

   |A linee|Tipo vendita|Codice vendita|Tipo|Codice|Codice variante<br>(aggiungi il campo tramite personalizzazione)|Prezzo unitario|
   |------|------------|------------|------------|----------------|------------|------------|
   |1|Gruppo di prezzi cliente|SHOPIFY|Elemento|1896-S|ESSENTIAL|700|
   |2|Gruppo di prezzi cliente|SHOPIFY|Elemento|1896-S|PREMIUM|1000|

9. Seleziona l'azione **Sconti sulle vendite** e aggiungi un nuovo sconto:

   * **Tipo vendita** *Gruppo sconti cliente*
   * **Codice vendita** *DETTAGLIO*
   * **Tipo** *Articolo*
   * **Codice** *1896-S*
   * **Cod. Unità di Misura** *PCS*
   * **Sconto riga %** *10*

10. Seleziona l'azione **Riferimenti elemento** e aggiungi le seguenti righe:

   |A linee|Tipo riferimento|Nr. Riferimento|Codice variante|
   |------|------------|------------|------------|
   |1|Codice a barre|77777777|ESSENTIAL|
   |2|Codice a barre|11111111|PREMIUM|

11. Seleziona la voce **1920-S, ANTWERP Conference Table** ed esegui i seguenti passaggi.
12. Seleziona **Regola Inventario** e nel campo **Nuovo inventario** inserisci **100** per le posizioni **EST** e **OVEST**.
13. Seleziona **OK**.

Regolare le impostazioni di sincronizzazione.

1. Seleziona l'icona ![lampadina che apre la funzionalità Dimmi](../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), e immetti **Punti vendita Shopify**, quindi seleziona il collegamento correlato.
2. Seleziona il **DEMO1** negozio per il quale vuoi sincronizzare gli articoli per aprire la pagina **Shopify Negozio scheda** .
3. Abilita il campo **Sincronizza testo marketing**.
4. Nello **SKU mapping** field, Seleziona **numero articolo+ codice variante**.
5. Nel campo  **Criterio inventario predefinito**, Seleziona **Continua**.
6. Nel campo  **Stato dei prodotti creati**, Seleziona **Bozza**.
7. Nel campo  **Azione per prodotto rimosso**, Seleziona **Stato su Archiviato**.
8. Nel campo  **Gruppo prezzi cliente**, Seleziona **SHOPIFY**.
9. Nel campo  **Gruppo sconto cliente**, Seleziona **VENDITA AL DETTAGLIO**.

Esegui la sincronizzazione.

1. Seleziona l'icona ![lampadina che apre la funzionalità Dimmi](../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), e immetti **Punti vendita Shopify**, quindi seleziona il collegamento correlato.
2. Seleziona il **DEMO1** negozio per il quale vuoi sincronizzare gli articoli per aprire la pagina **Shopify Negozio scheda** .
3. Seleziona **Prodotti** per aprire la pagina **Shopify Prodotti** .
4. Seleziona l'azione **Aggiungi articoli**.
5. Imposta il filtro **TAVOLA|SCRIVANIA** sul campo **Codice categoria articolo** .
6. Attiva l'interruttore **Sincronizza immagini prodotto**.
7. Attiva l'interruttore **Sincronizza inventario**.
8. Seleziona **OK** e attendi che la sincronizzazione iniziale di articoli, prezzi, immagini e inventario sia completata.

I prodotti vengono aggiunti. Si noti che lo stato è impostato su **Bozza** e pertanto gli articoli non sono visibili nello Shopify negozio online.

1. Seleziona la riga con l'articolo **1920-S, Tavolo da conferenza ANTWERP**. Nel  **titolo SEO**, inserisci **Tavolo riunioni rettangolare Anversa, 10 posti, nero**.
2. Nel campo  **Stato**, Seleziona **Attivo**.
3. Seleziona la riga con l'articolo **1906-S, ATHENS, Mobile Pedestal** e quindi Seleziona **Elimina**.

In **Amministrazione Shopify** nota che tutti i prodotti hanno stati diversi.

* *Il tavolo da conferenza ANTWERP* è *attivo* perché ne abbiamo modificato lo stato nella pagina **Shopify Prodotto** .
* *Scrivania ATENE* è *Bozza* perché abbiamo configurato lo stato predefinito per tutti i prodotti aggiunti come *Bozza*.
* *Piedistallo ATENE* è *Archiviato* perché abbiamo configurato il punto vendita per assegnare automaticamente lo stato su *Archiviato* per i prodotti eliminati.

Si noti che l'inventario per il tavolo della conferenza di ANTWERP è 100, perché abbiamo configurato il sistema in modo da utilizzare l'inventario solo da due posizioni, MAIN ed EAST. L'inventario in un'altra località (OVEST) viene ignorato.

* Apri *Tavolo conferenza ANTWERP*, annota i campi **Tipo personalizzato**, **Fornitore**, **Peso**, **Costo per articolo** e la sezione **Anteprima elenco motore di ricerca**.
* Apri *Scrivania Atene*, scorri verso il basso fino alla sezione **Varianti** e nota come è popolato **SKU**.
* Per rivedere il codice a barre e i prezzi, Seleziona **Modifica**.
* Cambia lo stato di **Athens Desk** in **Attivo** e Seleziona **anteprima**.

Nello Shopify negozio online, apri il catalogo prodotti e trova il prodotto **ATHENS Desk** . Nota che sono disponibili diverse opzioni. Per diverse opzioni, i prezzi sono diversi. Presta attenzione alle informazioni sugli sconti.

### <a name="additional-steps-for-b2b"></a>Ulteriori passaggi per B2B

[!INCLUDE [shopify-preview](../includes/shopify-preview.md)]

Puoi configurare il connettore per creare e assegnare automaticamente il catalogo per le società esportate. I passaggi seguenti sono utili se desideri un controllo più preciso di ciò che è disponibile per i clienti B2B.

In **Shopify Amministrazione**, crea e assegna un catalogo.

1. Seleziona **Prodotti** e quindi **Cataloghi** nella barra laterale di **Shopify - Amministra**.
2. Crea un catalogo per prodotti specifici. Dagli il titolo "B2B". 
3. Scegli **Gestisci**, quindi **Gestisci prodotti e prezzi**.
4. Seleziona il filtro **Esclusi**, trova **ATHENS Desk** e scegli **Includi nel catalogo**.
5. Seleziona **Clienti**, quindi **Aziende** nella barra laterale di **Shopify admin**.
6. Seleziona **Facoltà di Belle Arti**, scegli **[...]**, quindi **Aggiungi cataloghi** e aggiungi il catalogo **B2B** creato in precedenza.

In [!INCLUDE[prod_short](../includes/prod_short.md)] esegui le operazioni seguenti:

Preparare i dati.

1. Seleziona l'icona ![lampadina che apre la funzionalità Dimmi](../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immetti **Articoli** e seleziona il collegamento correlato.
2. Seleziona oggetto **1896-S, Athens Desk**, e quindi seguire questi passaggi:
3. Seleziona l'azione **Sconti sulle vendite** e aggiungi un nuovo sconto:

   * **Tipo vendita** *Gruppo sconti cliente*
   * **Codice vendita** *INGROSSO*
   * **Tipo** *Articolo*
   * **Codice** *1896-S*
   * **Cod. Unità di Misura** *PCS*
   * **Sconto riga %** *25*

4. Seleziona l'icona ![lampadina che apre la funzionalità Dimmi](../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immetti **Cataloghi Shopify** e seleziona il collegamento correlato.
5. Seleziona **Ottieni cataloghi**.
6. Nel campo  **Codice negozio**, inserisci  **DEMO1**.
7. Seleziona la voce con il catalogo *B2B* per il quale vuoi sincronizzare i prezzi.
8. Abilita l'interruttore **Sincronizza prezzi**.
9. Nel campo  **Gruppo prezzi cliente**, Seleziona **SHOPIFY**.
10. Nel campo  **Gruppo sconto cliente**, Seleziona **GRANDE ACC**.
11. Scegli **Sincronizza prezzi** e attendi il completamento della sincronizzazione dei prezzi.

In **Shopify Amministrazione**, esplora i prezzi per il catalogo **B2B** .

Nel **punto vendita Shopify online** apri il catalogo prodotti, trova il prodotto *Scrivania ATENE*. Prendi nota delle informazioni su prezzi e sconti.

## <a name="walkthrough-check-out-and-order-synchronization-for-individual-buyer-and-company-representative"></a>Procedura dettagliata: sincronizzare il completamento della transazione e l'ordine per l'acquirente individuale e il rappresentante della società

Questa è una continuazione di [Procedura dettagliata: iniziare a vendere prodotti online](walkthrough-setting-up-and-using-shopify.md#walkthrough-start-selling-products-online). Puoi anche provare con i tuoi dati, ad esempio utilizzando il tuo Shopify store o sandbox.

Acquirente individuale

1. In **Punto vendita online Shopify**: Scegli l'icona **Conto**. Immetti l'indirizzo e-mail a cui hai accesso.
2. Accedi utilizzando il codice di verifica monouso di 6 cifre inviato all'indirizzo email che hai inserito.
3. Esplora il catalogo prodotti. Dovresti essere in grado di vedere tutti i prodotti con i prezzi al dettaglio.
4. Seleziona la variante Essential e quindi **Acquista ora** e completa la transazione.
5. Compila i campi **Nome** e **Cognome**.
6. Inserisci l'indirizzo locale.
7. Mantieni *Standard* come metodo di spedizione.
8. Nel campo  **Numero di credito scheda**, inserisci  **1** se utilizzi  **(per il test) Bogus Gateway**, oppure inserisci  **5555 5555 5555 4444** se utilizzi  **Shopify pagamenti** in modalità test.
9. Nel campo **Data di scadenza**, immetti il mese e l'anno corrente.
10. Nel **Codice di sicurezza**, inserisci **111**.
11. Compila il campo **Nome sulla scheda**.
12. Seleziona **Paga adesso**.

Rappresentante della società

[!INCLUDE [shopify-preview](../includes/shopify-preview.md)]

1. In **Shopify - Amministra**.
2. Seleziona **Clienti** e quindi **Società** nella barra laterale di **Shopify - Amministra**.
3. Apri la voce *School of Fine Art*.
4. Seleziona **[...]** nel **School of Fine Art** FactBox, quindi **Modifica condizioni di pagamento** e quindi Seleziona **Scadenza evasione**.
5. Seleziona **[...]** nel riquadro **Clienti**, quindi **Aggiungi cliente** e infine aggiungi quello con l'email che hai utilizzato in precedenza per accedere al negozio.
6. In **Punto vendita online Shopify**: Scegli l'icona **Conto**. Immetti l'indirizzo e-mail a cui hai accesso.
7. Accedi utilizzando il codice di verifica monouso di 6 cifre inviato all'indirizzo email che hai inserito.
8. Esplora il catalogo prodotti: dovresti riuscire a vedere solo i prodotti aggiunti al catalogo B2B con prezzi speciali al dettaglio.
9. Seleziona la variante essenziale, Seleziona **Acquistala subito** e procedi al pagamento.
10. Nota che i campi Account, Spedisci a e Metodo di pagamento sono compilati.
11. Compila il campo  **Numero ordine di acquisto** con  **PO-12345**.
12. Seleziona **Invia ordine**.

In [!INCLUDE[prod_short](../includes/prod_short.md)], effettua i seguenti passaggi:

1. Seleziona l'icona ![lampadina che apre la funzionalità Dimmi](../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immetti **Ordini Shopify**, quindi scegli il collegamento correlato.
2. Seleziona l'azione **Sincronizza ordini da Shopify**.
3. Seleziona **OK**.

L'ordine importato è pronto per l'elaborazione.

1. Seleziona l'ordine importato per aprire la pagina **Shopify Ordine** .
2. Si noti che entrambi gli ordini sono stati inviati dalla stessa persona e sono collegati a due clienti diversi.
3. Nell'ordine inviato per conto dell'azienda, è possibile visualizzare un valore nel campo  **Numero ordine di acquisto**, che viene trasferito anche nel campo  **Numero documento esterno** del documento di vendita creato.
4. Poiché abbiamo configurato l'azienda B2B per gestire i pagamenti al di fuori di Shopify, lo **stato finanziario** è impostato su **in sospeso**. Dopo aver ricevuto il pagamento, Seleziona l'azione **Segna come pagato** . Aggiornamenti sulla situazione finanziaria in Shopify.

## <a name="walkthrough-import-items-customers-companies-from-shopify"></a>Procedura dettagliata: importare articoli, clienti, società da Shopify

### <a name="scenario-3"></a>Scenario

Hai già un punto vendita online di successo e vorresti iniziare a usare [!INCLUDE[prod_short](../includes/prod_short.md)] come software gestionale aziendale. Desideri importare quanti più dati possibile da Shopify.

### <a name="steps-2"></a>Passaggi

Questa è la continuazione di [Procedura dettagliata: iniziare a vendere prodotti online](walkthrough-setting-up-and-using-shopify.md#walkthrough-start-selling-products-online) e [ Procedura dettagliata: aggiungere i clienti al nuovo punto vendita online](walkthrough-setting-up-and-using-shopify.md#walkthrough-add-your-customers-to-your-new-online-store). Puoi anche provare con i tuoi dati, ad esempio utilizzando il tuo Shopify store o sandbox.

In [!INCLUDE[prod_short](../includes/prod_short.md)], segui i passaggi elencati di seguito.

#### <a name="prepare-data"></a>Preparare i dati

1. Passa a una prova gratuita di 30 giorni senza dati di esempio. Per ulteriori informazioni, vedi [Aggiungere i propri dati a una prova vuota](/dynamics365/business-central/dev-itpro/administration/trials-subscriptions#add-your-own-data-to-an-empty-trial-company).
2. Seleziona l'icona ![lampadina che apre la funzionalità Dimmi](../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), e immetti **Punti vendita Shopify**, quindi seleziona il collegamento correlato.
3. Seleziona **Nuovo**.
4. Nel campo **Codice** immetti **DEMO2**.
5. Nel campo **URL Shopify**, immetti l'URL al punto vendita online a cui desideri connetterti.
6. Attiva l'interruttore **Abilitato** quindi rivedi e accetta i termini e le condizioni.

Configura il punto vendita Shopify come descritto qui:

1. Disattiva l'interruttore **Consenti sincronizzazioni in background**.
2. Nel campo  **Elemento di sincronizzazione**, Seleziona **Da Shopify**.
3. Attiva l'opzione  **Crea automaticamente elementi sconosciuti** .
4. Compila il campo **Codice modello articolo** con il modello appropriato.
5. Nel campo  **Sincronizza immagini elemento**, Seleziona **Da Shopify**.
6. Nello **SKU mapping** field, Seleziona **numero articolo+ codice variante**.
7. Nel campo  **Importazione cliente da Shopify**, Seleziona **Tutti i clienti**.
8. Abilita l'interruttore **Crea automaticamente clienti sconosciuti**.
9. Compila il campo **Codice modello cliente/società** con il modello appropriato.
10. Nel campo  **Importazione azienda da Shopify**, Seleziona **Tutti i clienti**.
11. Attiva l'opzione  **Creazione automatica azienda sconosciuta** .

#### <a name="run-the-synchronization"></a>Esegui la sincronizzazione

1. Seleziona l'icona ![lampadina che apre la funzionalità Dimmi](../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), e immetti **Punti vendita Shopify**, quindi seleziona il collegamento correlato.
2. Seleziona il punto vendita *DEMO2* per il quale desideri sincronizzare i dati per l'apertura della pagina **Scheda del punto vendita Shopify**.
3. Seleziona **Sincronizza prodotti**.
4. Seleziona **Sincronizza immagini prodotto**.
5. Seleziona **Sincronizza clienti**.
6. Seleziona **Sincronizza società**.

### <a name="results"></a>Risultati

* I prodotti Shopify vengono importati. Per verificare, seleziona l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni.](../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immetti **Prodotti Shopify** e scegli il collegamento correlato.
* Vengono creati elementi con immagini. Per verificare, seleziona l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni.](../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immetti **Articolo** e seleziona il collegamento correlato.
* Shopify i clienti vengono importati. Per verificare, seleziona l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni.](../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immetti **Clienti Shopify**, quindi seleziona il collegamento correlato.
* Shopify le aziende vengono importate. Per verificare, seleziona l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni.](../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immetti **Società Shopify**, quindi seleziona il collegamento correlato.
* I clienti vengono creati. Per verificare, seleziona l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni.](../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immetti **Clienti**, quindi seleziona il collegamento correlato.

## <a name="see-also"></a>Vedere anche

[Iniziare a usare il connettore Shopify](get-started.md)  
