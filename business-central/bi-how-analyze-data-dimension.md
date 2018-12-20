---
title: Analizzare i dati per dimensioni| Documenti Microsoft
description: Descrive come analizzare i diversi dati aziendali per dimensioni.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: bi, power BI, analysis, KPI
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 5176b7c04c09b9357041ec4fed5ed37c385d13ce
ms.contentlocale: it-ch
ms.lasthandoff: 09/28/2018

---
#  <a name="analyze-data-by-dimensions"></a>Analizzare i dati per dimensioni
Nelle analisi finanziarie, una dimensione corrisponde ai dati che è possibile aggiungere a un movimento come una specie di contrassegno. Tali dati vengono utilizzati per raggruppare movimenti con caratteristiche simili, ad esempio clienti, aree, prodotti e agenti, quindi recuperare facilmente questi gruppi per l'analisi. Le dimensioni possono essere utilizzate per i movimenti nelle registrazioni, nei documenti e nei. Con il termine dimensione viene descritta la modalità di esecuzione dell'analisi. Un'analisi bidimensionale, ad esempio, corrisponde a vendite per area. Creando tuttavia più di due dimensioni quando si crea un movimento, è possibile eseguire analisi molto più complesse, ad esempio vendite per campagna di vendita per gruppo di clienti per area. Per ulteriori informazioni, vedere [Utilizzo delle dimensioni](finance-dimensions.md).

L'analisi dei dati per dimensioni consente di ottenere informazioni più dettagliate sull'attività commerciale, in modo da valutare le informazioni, ad esempio il livello di successo dell'attività, in quali aree è fiorente e in quali non lo è e dove è necessario assegnare ulteriori risorse.

> [!TIP]
> Un modo rapido per analizzare i dati transazionali in base alle dimensioni consiste nel filtrare i totali nel piano dei conti e le voci in tutte le finestre **Voci** in base alle dimensioni. Cercare l'azione **Imposta filtro dimensione**.

## <a name="to-set-up-an-analysis-view"></a>Per impostare una visualizzazione analisi  
Un'analisi basata sulle dimensioni consente di visualizzare una combinazione selezionata di dimensioni. È possibile archiviare e in seguito recuperare ogni analisi che viene impostata. Le informazioni relative all'impostazione di un'analisi sono memorizzate nella scheda di **visualizzazione analisi**, per semplificare le analisi successive.  

1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Visualizzazioni analisi** e quindi scegliere il collegamento correlato.  
2. Nella finestra **Lista visualizzazione analisi** scegliere l'azione **Nuovo**.
3. Compilare i campi, se necessario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. Per aggiungere altri codici di dimensione ai quattro disponibili nella Scheda dettaglio **Dimensioni**, scegliere l'azione **Filtro**, compilare i campi e scegliere il pulsante **OK**.  
5. Per aggiornare la visualizzazione, scegliere l'azione **Aggiorna**.

## <a name="to-analyze-by-dimensions"></a>Per analizzare per dimensioni
È possibile utilizzare la matrice **Analisi per dimensioni** per visualizzare gli importi della contabilità generale utilizzando le visualizzazioni analisi precedentemente impostate. Impostare la finestra **Analisi per dimensioni** per definire gli elementi visualizzati nella matrice, quindi scegliere l'azione **Mostra matrice** per visualizzare la matrice.  

- Nelle colonne a sinistra sono contenute informazioni sulla base di ciò che è stato selezionato nel campo **Mostra come righe** della testata.  
- Le colonne a destra contengono informazioni sulla base di ciò che è stato selezionato nel campo **Mostra come colonne** della testata.  

1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Analisi per dimensioni** e quindi scegliere il collegamento correlato.  
2. Selezionare la visualizzazione di analisi desiderata e scegliere l'azione **Modifica visualizzazione analisi**.
3. All'inizio della finestra **Analisi vendite per dimensioni**, compilare i campi per definire con viene visualizzato.
4. 5. Per visualizzare la specifica di un importo nella finestra matrice, selezionare l'importo.  

> [!IMPORTANT]  
>   Non è possibile selezionare una durata periodo più breve rispetto a quello specificato per la compressione data nella scheda **Visualizzazione analisi**. I comandi **Periodo successivo** e **Periodo precedente** non sono attivi se nel campo **Mostra come righe** oppure **Mostra come colonne** è stato selezionato il valore **Periodo**.  

> [!NOTE]  
>   È possibile utilizzare il report **Dimensioni - Dettagli** per visualizzare una classificazione dettagliata di come sono state utilizzate le dimensioni per i movimenti di un determinato periodo selezionato. È possibile utilizzare il report **Dimensioni - Totali** per visualizzare solo gli importi totali.  

> [!TIP]  
>   È inoltre possibile modificare la visualizzazione modificando il contenuto dei campi **Mostra come righe** e **Mostra come colonne**. Per ripristinare un'impostazione di visualizzazione, scegliere l'azione **Inverti righe e colonne**.

## <a name="to-update-an-analysis-view"></a>Per aggiornare una visualizzazione analisi  
Gli importi visualizzati nella finestra **Analisi per dimensioni** forniscono un'immagine dello stato della società al momento dell'ultimo aggiornamento. Per avere un'immagine dello stato corrente, è necessario eseguire la funzione di aggiornamento per aggiornare la visualizzazione dell'analisi.

La seguente procedura indica come aggiornare una visualizzazione analisi dalla finestra **Analisi per Dimensioni**. I passaggi sono simili a quelli delle finestre **Scheda visualizzazione analisi** e **Lista visualizzazione analisi**.  

1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Analisi per dimensioni** e quindi scegliere il collegamento correlato.  
2. Nella finestra **Analisi per dimensioni**, selezionare il campo **Codice visual. analisi**.  
3. Selezionare la riga con la visualizzazione analisi desiderata.  
4. Scegliere l'azione **Aggiorna**.  

> [!TIP]  
>   Se si seleziona la casella di controllo **Aggiorna in registrazione** in una scheda di visualizzazione analisi, la visualizzazione viene aggiornata automaticamente alla registrazione di una transazione interessata.

> [!NOTE]  
>   Per aggiornare contemporaneamente alcune o tutte le visualizzazioni analisi, è necessario utilizzare il processo batch **Aggiorna visualizzazione analisi**.  

## <a name="see-also"></a>Vedi anche
[Business Intelligence](bi.md)  
[Finanze](finance.md)  
[Impostazione di dati finanziari](finance-setup-finance.md)  
[Contabilità generale e piano dei conti](finance-general-ledger.md)  
[Utilizzo delle dimensioni](finance-dimensions.md)  
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
