---
title: 'Conteggiare, rettificare e riclassificare l''inventario'
description: Scopri come eseguire il conteggio fisico e apportare modifiche e riclassificazioni.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.service: dynamics-365-business-central
ms.topic: how-to
ms.date: 05/24/2024
ms.custom: bap-template
---
# <a name="count-adjust-and-reclassify-inventory-using-journals"></a>Conteggiare, rettificare e riclassificare l'inventario utilizzando registrazioni

Per assicurarti che le quantità siano corrette, conteggia fisicamente tutti gli articoli nell'inventario. Alcune aziende eseguono un conteggio fisico annuale e altre contano tutti o solo alcuni articoli più spesso. Dopo aver contato gli articoli, utilizza i giornali di registrazione per registrare le quantità effettive nella contabilità generale. Ad esempio, quando valuti l'inventario alla fine di un periodo.

Per contare alcuni oggetti più spesso di altri, ad esempio a causa del loro valore, usa i conteggi ciclici. Per i conteggi ciclici assegna speciali periodi di conteggio agli articoli. Per ulteriori informazioni vedi [Per eseguire il conteggio ciclico](inventory-how-count-adjust-reclassify.md#to-do-cycle-counting).

Per rettificare le quantità dopo un conteggio fisico o per altri scopi, utilizza un giornale di registrazione articoli per modificare i movimenti contabili di inventario senza registrare le transazioni. Puoi rettificare la quantità di un singolo articolo anche nella scheda articolo.

Per modificare gli attributi dei movimenti contabili articoli, utilizza le registrazioni di riclassificazione articoli. Gli attributi tipici da riclassificare includono dimensioni e codici delle campagne di vendita. Puoi anche usare i giornali di riclassificazione per trasferimenti riclassificando i codici collocazione e ubicazione. Passaggi speciali si applicano quando si desidera riclassificare i numeri di serie o di lotto e le relative date di scadenza. Per ulteriori informazioni, vedere [Utilizzo dei numeri di serie e di lotto](inventory-how-work-item-tracking.md).

> [!NOTE]
> Nei processi a più passaggi gli articoli sono registrati nelle collocazioni come movimenti warehouse e non come movimenti contabili articoli. Di conseguenza, esegui il conteggio, la rettifica e la riclassificazione in registrazioni di warehouse speciali che supportano le collocazioni. Quindi, sincronizza i movimenti warehouse nuovi o modificati con i movimenti contabili articoli correlati per riflettere le modifiche nelle quantità e nei valori di magazzino.

[!INCLUDE [edit-in-excel](includes/edit-in-excel.md)]

## <a name="to-count-physical-inventory"></a>Per contare l'inventario fisico

Per controllare se le quantità registrate corrispondono alle quantità fisiche presenti in magazzino, contare l'inventario fisico. In pratica, conteggia gli oggetti effettivi disponibili. In genere, i conteggi avvengono alla fine di un anno fiscale, ma alcune aziende conteggiano gli articoli più spesso. Se esistono differenze, registra le quantità effettive nei conti articoli prima di eseguire la valutazione del magazzino.

> [!NOTE]
> Questa procedura consente come eseguire un inventario fisico utilizzando una registrazione nella pagina **Registrazioni inventario fis.**. È possibile utilizzare i documenti nelle pagine **Ordine inventario fisico** e **Registrazione inventario fisico**. Questi documenti offrono maggiore controllo e supporto per la distribuzione del lavoro di conteggio a più dipendenti. Per ulteriori informazioni vedi [Conteggio dell'inventario utilizzando documenti](inventory-how-count-inventory-with-documents.md).<br /><br />
> Nota che non puoi usare la funzionalità basata su documenti per conteggiare articoli in collocazioni o movimenti di warehouse.

Il processo di conteggio prevede anche le seguenti attività:

- Calcolo delle giacenze previste.
- Stampa il report da usare per il conteggio.
- Immissione e registrazione delle quantità effettive.

In base al setup della warehouse, conteggia l'inventario fisico in uno dei seguenti modi. Per ulteriori informazioni, vedere [Impostazione gestione warehouse](warehouse-setup-warehouse.md).  

- Se la tua ubicazione non utilizza lo stoccaggio e il prelievo diretti, utilizza la pagina **Registrazioni inventario fis.**. La procedura è simile all'inventario fisico senza conteggio ciclico.  
- Se la tua ubicazione utilizza lo stoccaggio e il prelievo diretti, utilizza la pagina **Registrazione dell'inventario fisico warehouse**. Quindi utilizza la pagina **Registrati articoli** per eseguire l'azione **Calcola rettifica warehouse**. <!--We should say what to do on each of these pages.-->

### <a name="to-calculate-expected-inventory-in-basic-warehouse-configurations"></a>Per calcolare le giacenze previste nelle configurazioni warehouse di base

1. Scegli la ![lampadina che apre la funzione Dimmi.](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immetti **Registrazioni inventario fisico**, quindi scegli il collegamento correlato.
2. Selezionare l'azione **Calcola inventario** da **Prepara**.
3. Nella pagina **Calcola giacenze** specificare le condizioni da utilizzare per creare le righe registrazioni, ad esempio se includere gli articoli che non hanno inventario registrato.
4. Impostare i filtri se si desidera soltanto calcolare le giacenze per determinati articoli, collocazioni, ubicazioni o dimensioni.
5. Scegliere il pulsante **OK**.

> [!NOTE]  
> I movimenti articoli vengono elaborati in base alle informazioni inserite e le righe vengono create in registrazioni inventario fisico. Nota che il campo **Qtà (inv. fisico)** ha la stessa quantità del campo **Qtà (calcolata)** . Non è necessario inserire la quantità conteggiata per gli articoli in cui questi valori corrispondono. Tuttavia, se la quantità conteggiata è diversa, immetti la quantità che è stata conteggiata.

### <a name="to-print-the-report-to-be-used-when-counting"></a>Per stampare il report da utilizzare nel conteggio

1. Nella pagina  **Giornali di inventario fisico** contenente l'inventario previsto calcolato, selezionare l'azione  **Stampa** da  **Home**.
2. Nella pagina  **Elenco inventario fisico**, specificare se il report mostrerà la quantità calcolata e gli articoli di inventario in base ai numeri di serie e di lotto.
3. Impostare i filtri se si desidera stampare il report solo per determinati articoli, collocazioni, ubicazioni o dimensioni.
4. Scegli **Stampa**.

Gli addetti al magazzino possono quindi conteggiare l'inventario e registrare le differenze nel report stampato.

> [!NOTE]
> Potrebbero essere necessari diversi giorni prima che i report stampati tornino per l'elaborazione e la registrazione finali. Quando si specificano e registrano le giacenze effettive conteggiate, il sistema rettifica le giacenze in modo da riflettere la differenza tra le giacenze previste e quelle effettive conteggiate. È necessario mantenere le righe di registrazione calcolate originariamente e non ricalcolare le giacenze previste, poiché le giacenze previste potrebbero cambiare e determinare livelli di magazzino non corretti. Se è necessario emettere più report, ad esempio per ubicazioni o gruppi di articoli diversi, è necessario creare e conservare batch di registrazioni separati.

### <a name="to-enter-and-post-the-actual-counted-inventory-in-basic-warehouse-configurations"></a>Per immettere e registrare le giacenze effettive conteggiate nelle configurazioni di warehouse di base

1. In ogni riga della pagina  **Giornali di inventario fisico** in cui l'inventario effettivo disponibile, determinato dal conteggio fisico, differisce dalla quantità calcolata, immettere l'inventario effettivo disponibile nel campo  **Qtà (inventario fisico)** .
  
  > [!NOTE]  
  > Se dal conteggio fisico risultano differenze determinate dalla registrazione degli articoli con ubicazione non corrette, le differenze non devono essere inserite nelle registrazioni inventario fisico. In alternativa, utilizza le registrazioni di riclassificazione o un ordine di trasferimento per reindirizzare gli articoli alle ubicazioni corrette. 

2. Per convertire le quantità calcolate in quelle effettivamente conteggiate, seleziona l'azione  **Post** da **Home**.

    La registrazione crea i movimenti contabili articoli e i movimenti contabili di inventario fisico. Apri la pagina Scheda articolo per l'articolo per trovare i movimenti contabili di inventario fisico.

3. Scegli la ![lampadina che apre la funzione Dimmi.](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immetti **Articoli** e scegli il collegamento correlato.
4. Per verificare il conteggio, apri la pagina  **Articolo scheda** per l'articolo e scegli l'azione  **Voci contabili inventario fisico** da **Articolo**
1. .

### <a name="to-calculate-the-expected-inventory-in-advanced-warehouse-configurations"></a>Per calcolare le giacenze previste nelle configurazioni di warehouse avanzate

Sincronizza la contabilità articoli e warehouse <!--warehouse what?--> prima di contare l'inventario fisico. In caso contrario, ciò che si registra nel giornale di registrazione dell'inventario fisico e nella contabilità articoli sono i risultati dell'inventario fisico combinati con altre rettifiche di warehouse per gli articoli. Per ulteriori informazioni, vedi [Sincronizzare le quantità nei movimenti contabili e nella warehouse](inventory-how-count-adjust-reclassify.md#to-synchronize-the-adjusted-warehouse-entries-with-the-related-item-ledger-entries).

1. Scegli la ![lampadina che apre la funzione Dimmi.](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immetti **Registrazione dell'inventario fisico warehouse**, quindi scegli il collegamento correlato.  
2. Scegliere l'azione **Calcola inventario** per aprire la pagina **Calcola inventario whse.**.  
3. Imposta i filtri per specificare gli articoli che verranno conteggiati nelle registrazioni e scegli **OK**.

   [!INCLUDE [prod_short](includes/prod_short.md)] crea una riga per ciascuna collocazione che soddisfa i requisiti del filtro. Puoi eliminare alcune righe. Tuttavia, se vuoi registrare i risultati come inventario fisico, è necessario conteggiare l'articolo in tutte le collocazioni in cui è contenuto.  

   Se scegli di conteggiare l'articolo solo in alcune collocazioni, è possibile immettere le differenze e registrarle nella pagina **Registrazione articoli** successivamente utilizzando l'azione **Calcola rettifica whse**.  

### <a name="to-enter-and-post-the-actual-counted-inventory-in-advanced-warehouse-configurations"></a>Per immettere e registrare le giacenze effettive conteggiate nelle configurazioni di warehouse avanzate

1. Nella pagina **Registrazione dell'inventario fisico warehouse** immetti le quantità effettive nel campo **Qtà (inv. fisico)**.  

    > [!NOTE]  
    > Il campo **Qtà. (calcolata)** viene compilato in base ai record collocazione. La quantità è copiata nel campo **Qtà. (fisica)** in ogni riga. Se le quantità in questi campi non corrispondono, inserisci la quantità effettiva.  

2. Dopo avere immesso tutte le quantità effettive, scegli l'azione **Registra**.  

    Quando si effettua la registrazione, [!INCLUDE [prod_short](includes/prod_short.md)] crea nel registro warehouse due movimenti di warehouse per ogni riga conteggiata e registrata, nel modo descritto di seguito.  

    - Se le quantità effettive e le quantità calcolate risultano differenti, viene registrata una quantità positiva o negativa per la collocazione e viene contabilizzata una quantità di compensazione nella collocazione di rettifica dell'ubicazione.  
    - Se la quantità calcolata è uguale alla quantità fisica, [!INCLUDE [prod_short](includes/prod_short.md)] registra **0** sia per la collocazione che per la collocazione di rettifica. 

Quando si registra l'inventario fisico, non si esegue la registrazione nell'articolo, nell'inventario fisico o nei movimenti contabili di valori. Tuttavia, i record sono disponibili per la riconciliazione quando necessario. Per mantenere le quantità accurate, dopo aver conteggiato gli articoli in tutte le collocazioni, registra i risultati.<!--physical inventory journal--> Per ulteriori informazioni, vedi [Sincronizzare le quantità nei movimenti contabili e nel warehouse](inventory-how-count-adjust-reclassify.md#to-synchronize-the-adjusted-warehouse-entries-with-the-related-item-ledger-entries).

## <a name="to-do-cycle-counting"></a>Per eseguire un conteggio ciclico

Puoi contare gli articoli tutte le volte che vuoi. Ad esempio, perché sono più preziosi o più venduti. Specifica la frequenza di conteggio assegnando periodi di conteggio speciali agli articoli.

In base al setup della warehouse puoi eseguire il conteggio ciclico in uno dei seguenti modi. Per ulteriori informazioni vedi [Impostazione di Warehouse Management](warehouse-setup-warehouse.md).  

- Se la tua ubicazione non utilizza lo stoccaggio e il prelievo diretti, utilizza la pagina **Registrazioni inventario fisico**. I passaggi sono simili al conteggio dell'inventario fisico senza conteggio ciclico.  
- Se la tua ubicazione utilizza lo stoccaggio e il prelievo diretti, utilizza la pagina **Registrazione dell'inventario fisico warehouse**. Quindi utilizza la pagina **Registrati articoli** per eseguire l'azione **Calcola rettifica warehouse**. <!--we should say what to do on each of these pages-->  

### <a name="to-set-up-counting-periods"></a>Per impostare i periodi di conteggio

Il conteggio dell'inventario fisico viene in genere eseguito ad intervalli regolari, ad esempio con frequenza mensile, trimestrale o annuale. Puoi impostare i periodi di conteggio dell'inventario necessari, quindi assegnarne uno a ciascun articolo. Successivamente, utilizza l'azione **Calcola periodo di conteggio** nella pagina **Registrazioni inventario fisico** per creare automaticamente le righe per gli articoli.

1. Scegli l'icona ![lampadina che apre la funzione Dimmi.](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immetti **Periodo conteggio inventario fisico**, quindi scegli il collegamento correlato.  
2. Compilare i campi in base alle esigenze. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

### <a name="to-assign-a-counting-period-to-an-item"></a>Per assegnare un periodo di conteggio a un articolo

1. Scegli l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni.](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immetti **Articoli**, quindi scegli il collegamento correlato.  
2. Selezionare l'articolo a cui si desidera assegnare un periodo di conteggio.  
3. Nel campo **Codice periodo conteggio magazzino fisico**, seleziona il periodo di conteggio.  

> [!NOTE]
> Se stai modificando il periodo di conteggio, un messaggio visualizza le informazioni sui risultati della modifica. Scegli **Sì** per modificare il codice e calcolare il primo periodo di conteggio per l'articolo. Alla successiva scelta di calcolare un periodo di conteggio nelle registrazioni di inventario fisico, l'articolo verrà visualizzato come riga nella pagina **Selez. articoli inv. fis.**. È quindi possibile contare periodicamente l'articolo.

### <a name="to-start-a-count-based-on-counting-periods-in-basic-warehouse-configurations"></a>Per iniziare un conteggio basato sui periodi di conteggio nelle configurazioni warehouse di base

1. Scegli l'icona ![lampadina che apre la funzione Dimmi.](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immetti **Registrazioni inventario fisico**, quindi scegli il collegamento correlato.
2. Scegliere l'azione **Calcola conteggio periodo**.

    Viene visualizzata la pagina **Selez. articoli inv. fis.** con gli articoli da conteggiare in base ai periodi di conteggio.
3. Esegui il conteggio dell'inventario fisico. Per ulteriori informazioni vedi [Per contare l'inventario fisico](inventory-how-count-adjust-reclassify.md#to-count-physical-inventory).

### <a name="to-start-a-count-based-on-counting-periods-in-advanced-warehouse-configurations"></a>Per iniziare un conteggio basato sui periodi di conteggio nelle configurazioni warehouse avanzate

1. Scegli l'icona ![lampadina che apre la funzione Dimmi.](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immetti **Registrazione dell'inventario fisico warehouse**, quindi scegli il collegamento correlato.  
2. Scegliere l'azione **Calcola conteggio periodo**.

    Viene visualizzata la pagina **Selez. articoli inv. fis.** con gli articoli da conteggiare in base ai periodi di conteggio.
3. Esegui il conteggio dell'inventario fisico. Per ulteriori informazioni vedi [Per contare l'inventario fisico](inventory-how-count-adjust-reclassify.md#to-count-physical-inventory).  

   > [!NOTE]  
   > Conta l'articolo in tutte le collocazioni che lo contengono. Se elimini alcune righe relative alle collocazioni che sono state recuperate per il conteggio nella pagina **Inventario fis. whse.**, il conteggio sarà incorretto quando lo registri nelle registrazioni inventario fisico.  

## <a name="to-adjust-the-quantity-of-one-item"></a>Per rettificare la quantità di un articolo

Dopo aver eseguito un conteggio fisico di un articolo, usa l'azione **Rettifica magazzino** per registrare l'effettiva quantità di magazzino.

1. Scegli l'icona ![lampadina che apre la funzione Dimmi.](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immetti **Articoli**, quindi scegli il collegamento correlato.
2. Selezionare l'articolo per cui si desidera rettificare il magazzino e scegliere l'azione **Rettifica magazzino**.
3. Nel campo **Nuovo inventario** per l'ubicazione, inserisci il risultato del conteggio.
4. Scegliere il pulsante **OK**.

<!-- I don't see a "Quantity on Hand" field on the Item Card page. Should this point to the options for viewing availability?

The item’s inventory is adjusted. The new quantity is shown in the **Quantity on Hand** field on the **Item Card** page.-->

È inoltre possibile utilizzare l'azione **Rettifica magazzino** come semplice mezzo per aggiungere articoli acquistati nel magazzino se non usi fatture o ordini di acquisto per registrare gli acquisti. Ulteriori informazioni in [Registrare gli acquisti](purchasing-how-record-purchases.md).

> [!NOTE]  
> Dopo aver modificato l'inventario, aggiornane il valore corrente. Per ulteriori informazioni, vedere [Rivalutare il magazzino](inventory-how-revalue-inventory.md).

### <a name="to-adjust-the-quantities-of-multiple-items-in-basic-warehouse-configurations"></a>Per rettificare le quantità di più articoli nelle configurazioni warehouse di base

Nella pagina  **Giornali di registrazione articoli**, è possibile registrare le transazioni degli articoli direttamente nell'inventario Regola per acquisti, vendite e variazioni positive o negative senza utilizzare documenti.

Se le registrazioni magazzino sono spesso utilizzate per la stessa riga di registrazione o per righe di registrazione simili, ad esempio in relazione al consumo di materiale, puoi utilizzare la pagina **Registrazioni magazzino standard** per rendere più semplice questo tipo di lavoro ricorrente. Per ulteriori informazioni, vedi [Utilizzare le registrazioni standard](ui-work-general-journals.md#work-with-standard-journals).

1. Scegli l'icona ![lampadina che apre la funzione Dimmi.](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immetti **Registrazioni articoli**, quindi scegli il collegamento correlato.
2. Compilare i campi in base alle esigenze. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. Per rettificare le quantità scegli l'azione **Registra**.

### <a name="to-adjust-bin-quantities-in-advanced-warehouse-configurations"></a>Per rettificare le quantità di collocazioni nelle configurazioni di warehouse avanzate

Se l'ubicazione utilizza stoccaggi e prelievi diretti, utilizza la pagina **Registrazione articoli warehouse** per registrare le modifiche di quantità positive e negative non pianificate. Ad esempio, per articoli registrati come mancanti che si presentano inaspettatamente o per perdite dovute ad articoli danneggiati.  

I giornali di registrazione articoli warehouse offrono più livelli di rettifica per rendere le quantità più precise. La warehouse sa quanti articoli sono disponibili e dove sono immagazzinati, ma ogni rettifica non viene registrata nella contabilità articoli. Gli accrediti o gli addebiti vengono effettuati nella collocazione reale con la rettifica della quantità. Viene effettuato un movimento di contropartita in una collocazione di rettifica. La collocazione di rettifica è una collocazione virtuale senza articoli reali. Specifica la collocazione virtuale nel campo **Codice collocazione rettifica magazzino** nelle pagine **Scheda ubicazione**.

1. Scegli l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni.](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immetti **Registrazione degli articoli di warehouse**, quindi scegli il collegamento correlato.  
2. Compilare le informazioni di testata.  
3. Nel campo **Nr. articolo** della riga seleziona l'articolo.  
4. Immetti la collocazione in cui inserire gli articoli extra o la posizione in cui sono stati rilevati articoli mancanti.  
5. Nel campo **Quantità** , se trovi articoli extra, inserisci una quantità positiva. In caso di articoli mancanti, immettere una quantità negativa.  
6. Scegliere l'azione **Registra**.

## <a name="to-synchronize-the-adjusted-warehouse-entries-with-the-related-item-ledger-entries"></a>Per sincronizzare i movimenti warehouse rettificati con i movimenti contabili articoli correlati

Registra i record della collocazione di rettifica nella contabilità articoli per i periodi definiti. Alcune aziende registrano le rettifiche giornalmente nella contabilità articoli, mentre altre si riconciliano meno spesso.

1. Scegli l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni.](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immetti **Registrazioni articoli**, quindi scegli il collegamento correlato.  
2. Compilare i campi di ogni riga di registrazione.  
3. Scegli l'azione **Calcola rettifica warehouse** , quindi aggiungi i filtri nella pagina **Calcola rettifica warehouse**. Le rettifiche vengono calcolate solo per i movimenti nella collocazione rettifica che soddisfano i criteri dei filtri.  
4. Nella Scheda dettaglio **Opzioni** immettere un numero nel campo **Nr. documento**. Il numero appare nelle righe di registrazione magazzino.
5. Selezionare **OK**. Le rettifiche positive e negative vengono sommate per ogni articolo e le righe create nelle registrazioni magazzino.  
6. Registrare le righe di registrazione per immettere le differenze di quantità nei movimenti contabili magazzino. Le quantità nelle collocazioni e la contabilità articoli ora corrispondono.  

## <a name="see-also"></a>Vedere anche

[Conteggiare l'inventario utilizzando documenti](inventory-how-count-inventory-with-documents.md)  
[Magazzino](inventory-manage-inventory.md)  
[Panoramica della gestione warehouse](design-details-warehouse-management.md)  
[Vendite](sales-manage-sales.md)  
[Acquisti](purchasing-manage-purchasing.md)  
[Utilizzare [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
