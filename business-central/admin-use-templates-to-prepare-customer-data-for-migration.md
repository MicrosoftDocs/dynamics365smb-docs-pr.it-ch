---
title: Preparazione della migrazione dei dati dei clienti | Documenti Microsoft
description: "Dopo aver importato e collegato i dati di setup nel nuovo database, è possibile iniziare la migrazione dei dati master esistenti del cliente, ad esempio numeri e nomi di articoli e di clienti. Per assicurarsi che questi dati siano creati rapidamente e in modo accurato nella nuova società, è necessario utilizzare modelli per la strutturazione dei dati."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 03/07/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 3cfc53c1ea3c8d30f65b2d475a8dab052519e81e
ms.contentlocale: it-ch
ms.lasthandoff: 03/22/2018

---
# <a name="prepare-to-migrate-customer-data"></a>Preparazione per la migrazione dei dati dei clienti
Dopo aver importato e collegato i dati di setup nel nuovo database, è possibile iniziare la migrazione dei dati master esistenti del cliente, ad esempio numeri e nomi di articoli e di clienti. Per assicurarsi che questi dati siano creati rapidamente e in modo accurato nella nuova società, è necessario utilizzare modelli per la strutturazione dei dati.  

In genere, si creano modelli dati per le seguenti tabelle di dati master:  

-   **Contatto**  
-   **Cliente**  
-   **Articolo**  
-   **Fornitore**  

Tuttavia, è possibile creare una struttura del modello a tale scopo e applicarla a qualsiasi tabella in [!INCLUDE[d365fin](includes/d365fin_md.md)].  

> [!TIP]  
>  È anche possibile utilizzare modelli dati per le operazioni quotidiane per creare nuovi record basati su modelli. Questi modelli dati funzionano solo per le tabelle di dati master supportate. Per ulteriori informazioni, vedere, ad esempio, [Registrare nuovi articoli](inventory-how-register-new-items.md).  

Quando si importano dati sui clienti, ad esempio relativi agli articoli, i dati specificati nei campi obbligatori vengono recuperati dal modello dati collegato. Quando si crea un nuovo articolo, immettere soltanto le informazioni generali quali il numero, la descrizione e il prezzo dell'articolo e quindi recuperare il resto dei dati obbligatori del campo da un modello dati selezionato.  

Alla creazione di un nuovo record dati master, ad esempio una scheda cliente, alcuni campi sono obbligatori e devono essere compilati. È possibile raggruppare la maggior parte dei campi obbligatori, come le categorie di registrazione e le condizioni di pagamento, per rendere la creazione di record dati master più semplice e stabile. Ad esempio, è possibile raggruppare i campi obbligatori per la tabella 18, **Cliente** come tipi **Nazionale**, **Estero** o **Esporta**.

## <a name="to-select-a-data-template"></a>Per selezionare un modello dati
Quando si seleziona un modello dati esistente, è necessario stabilire se i modelli creati per la nuova azienda sono sufficienti per il cliente. Analizzare i campi e i valori forniti per determinare quali modelli sono appropriati per una nuova società.  

> [!TIP]  
>  È anche possibile utilizzare i modelli dati per creare rapidamente nuovi record. Utilizzarli per una creazione dei dati più rapida e precisa. Per ulteriori informazioni, vedere [Registrare nuovi articoli](inventory-how-register-new-items.md).

1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Modelli di configurazione**, quindi scegliere il collegamento correlato.  
2. Nella finestra **Lista modelli di configurazione**, selezionare un modello di dati dalla lista e quindi scegliere l'azione **Modifica**.  

Se i modelli di default non corrispondono alle proprie esigenze, è possibile creare nuovi modelli o aggiungere i campi a un modello esistente. Se i modelli di default sono sufficienti, è possibile utilizzarli per creare record in base ai modelli dati master.

## <a name="to-create-a-data-template"></a>Per creare un modello di dati
È possibile creare un nuovo modello di dati se i modelli di default non soddisfano le esigenze della nuova società. Se si creano più modelli, può essere utile adottare una convenzione di denominazione per il campo **Codice**.

Ogni modello include una testata e più righe. Quando si crea un modello, è possibile specificare i campi da applicare sempre ai dati di un determinato tipo. Ad esempio, è possibile creare modelli di cliente diversi da applicare ai diversi tipi di cliente. Quando si crea un cliente che utilizzano un modello, è possibile utilizzare i dati del modello per prepopolare determinati campi.

### <a name="to-create-a-data-template-header"></a>Per creare una testata modello dati
1. Aprire la finestra **Lista modelli di configurazione**.
2. Scegliere l'azione **Nuovo**.
3. Nel campo **ID tabella** immettere la tabella a cui si applica il modello. Il campo **Nome tabella** viene compilato automaticamente quando si imposta il campo **ID tabella**.

### <a name="to-create-a-data-template-line"></a>Per creare una riga modello dati
1. Nella prima riga, selezionare il campo **Nome campo**. Nella finestra **Lista campi** viene visualizzata la lista dei campi della tabella.
2. Selezionare un campo e scegliere il pulsante **OK**. Il campo **Didascalia campo** viene compilato con il nome del campo.
3. Nel campo **Valore predefinito**, immettere un valore appropriato. In alcuni casi, potrebbe essere necessario utilizzare un valore che non è disponibile nel database. In questo caso, è possibile selezionare la casella di controllo **Ignora verifica relazione** per consentire di collegare i dati senza errori.

    > [!TIP]  
    > Poiché il campo **Valore predefinito** non dispone di una funzione di ricerca per le opzioni campo [!INCLUDE[d365fin](includes/d365fin_md.md)] corrispondenti, copiare e incollare il valore desiderato dalla pagina correlata nel modello.

    > Selezionare la casella di controllo **Obbligatorio**. La casella di controllo viene visualizzata soltanto a scopo informativo. Indica che le informazioni devono essere immesse nel campo dall'utente, ma non viene applicata alcuna logica di business. Non è ad esempio possibile fatturare e registrare un ordine se le categorie di registrazione non sono ancora state impostate. Poiché le categorie di registrazione sono obbligatorie, è possibile selezionare la casella di controllo **Obbligatorio** per i rispettivi campi.

3. Nel campo **Riferimento** immettere informazioni sul campo in base alle necessità.
4. Scegliere il pulsante **OK**.

## <a name="to-export-to-a-template-in-excel"></a>Per esportare in un modello in Excel
È possibile creare un foglio di lavoro di Excel da utilizzare come modello basato sulla struttura di una tabella di database esistente. È quindi possibile utilizzare il modello per riunificare i dati dei clienti in formato uniforme per la successiva importazione in [!INCLUDE[d365fin](includes/d365fin_md.md)].

1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Foglio di lavoro configurazione**, quindi scegliere il collegamento correlato.
2. Aggiungere una tabella alla lista oppure selezionare una tabella esistente. Per ulteriori informazioni, vedere [Gestione della configurazione della società in un foglio di lavoro](admin-how-to-manage-company-configuration-in-a-worksheet.md).
3. Definire i campi della tabella che si desidera includere nel modello.
4. Scegliere l'azione **Esporta in modello**.
5. Denominare e salvare il file Excel. Il foglio di lavoro di Excel viene aperto automaticamente.

È possibile immettere i dati dei clienti nel foglio di lavoro di Excel. Se sono state esportate più tabelle, ogni tabella verrà inserita in un singolo foglio di lavoro. Salvare il foglio di lavoro prima di proseguire con la procedura descritta di seguito.

> [!NOTE]  
> È possibile che si verifichi il seguente errore quando si esegue una versione di Excel in lingua inglese, ma nelle impostazioni internazionali è impostata una lingua diversa dall'inglese: "Formato precedente o tipo di libreria non valido". Per correggere questo errore, controllare che sia installato il Language Pack per una lingua diversa dall'inglese.

## <a name="to-import-from-a-template-in-excel"></a>Per importare da un modello in Excel
1. Nella finestra **Foglio di lavoro configurazione**, scegliere l'azione **Importa da modello**.
3. Passare al foglio di lavoro del modello creato, quindi scegliere l'azione **Apri**.
4. Per aggiungere i dati sul cliente raccolti al database, scegliere l'azione **Collega dati**.

Quando si collegano i dati di un modello in Excel a una tabella, anch'essa collegata a un modello di configurazione nel pacchetto di configurazione, vengono applicati anche i valori di default del campo del modello di configurazione.

Risulta completo qualsiasi record che presenta questa modalità di collegamento dei dati, poiché è composto dai dati immessi da un utente in Excel e dai valori di default specificati nel modello di configurazione.

## <a name="to-create-a-record-from-a-configuration-template"></a>Per creare un record da un modello di configurazione
È possibile utilizzare la struttura dei dati contenuti nei modelli di dati per convertire singolarmente le informazioni in record nel database. A tale scopo, utilizzare la funzione **Crea istanza**. Si tratta di una versione miniatura del processo di migrazione dei dati e può essere utile per creare prototipi o gestire attività di creazione di dati di dimensioni più piccole.  

Nella seguente procedura viene illustrato come creare una scheda articolo da un modello dati dell'articolo. È possibile creare un record da qualsiasi modello dati utilizzando la stessa procedura.  

1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Modelli di configurazione**, quindi scegliere il collegamento correlato.  
2. Selezionare il modello **Articolo**, quindi scegliere l'azione **Modifica**. Per ulteriori informazioni, vedere la sezione "Per creare un modello di dati".
3. Selezionare l'azione **Crea istanza**. Una scheda articolo viene creata.  
4. Scegliere il pulsante **OK**.  
5. Per esaminare la nuova scheda articolo, scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Articoli**, quindi scegliere il collegamento correlato.  
6. Aprire la nuova scheda articolo.  
7. Espandere le varie Schede dettaglio e verificare che le informazioni siano state create correttamente.  

## <a name="to-use-a-configuration-template-on-a-record"></a>Per utilizzare un modello di configurazione su un record
È possibile applicare un modello dati a qualsiasi record in [!INCLUDE[d365fin](includes/d365fin_md.md)] e utilizzare questa tecnica per modificare un record. Tuttavia, se si esegue questa operazione, sovrascrivere i valori presenti nel record con quelli del modello. Di conseguenza, è necessario prestare attenzione quando si applica un modello ai record esistenti.

> [!WARNING]  
>  La funzione **Collega modello** sovrascrive i dati esistenti in un record. Se questa funzione viene utilizzata nella migrazione dei dati master, i dati importati verranno sovrascritti alla creazione dei record.

La seguente procedura è basata su una nuova scheda cliente.  

1. Creare un cliente Per ulteriori informazioni, vedere [Registrare nuovi clienti](sales-how-register-new-customers.md).
2. Nella finestra **Scheda cliente** scegliere l'azione **Applica modello**.  
3. Nella finestra **Modelli clienti**, selezionare uno dei modelli, quindi scegliere il pulsante **OK**.  

I valori di default dal modello cliente scelto sono inseriti nella scheda cliente.

## <a name="see-also"></a>Vedi anche  
[Impostare una società con RapidStart Services](admin-set-up-a-company-with-rapidstart.md)  
[Amministrazione](admin-setup-and-administration.md)  
[Registrare nuovi clienti](sales-how-register-new-customers.md)
