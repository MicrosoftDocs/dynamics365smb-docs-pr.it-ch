---
title: Analisi degli importi effettivi e degli importi di budget| Documenti Microsoft
description: Descrive come analizzare gli importi effettivi e gli importi di budget.
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
ms.openlocfilehash: 17a6368e5a25ad12db05825b863ce29cd329cd39
ms.contentlocale: it-ch
ms.lasthandoff: 09/28/2018

---
# <a name="analyze-actual-amounts-versus-budgeted-amounts"></a>Analisi degli importi effettivi e degli importi di budget
Come parte della raccolta, dell'analisi e della condivisione dei dati della società, si visualizzano gli importi effettivi rispetto agli importi di budget per tutti i conti e per diversi periodi.

Per analizzare gli importi di budget, è prima necessario creare budget C/G. Per ulteriori informazioni, vedere [Creare budget C/G](finance-how-create-budgets.md).

## <a name="to-view-a-gl-budget"></a>Per visualizzare un budget C/G
In un budget per cui siano state impostate delle dimensioni è possibile filtrare i movimenti e visualizzare budget specifici.

1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Budget C/G** e quindi scegliere il collegamento correlato.
2. Nella finestra **Budget CG** aprire il budget che si desidera visualizzare.  
3. All'inizio della finestra, compilare i campi secondo le necessità per definire cosa viene visualizzato. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]  
>   Se è stato selezionato il valore **Periodo** nel campo **Mostra come righe** oppure nel campo **Mostra come colonne**, è necessario compilare il campo **Visualizza per**. Se non è stato selezionato il valore **Periodo** nel campo **Mostra come righe** o **Mostra come colonne** immettere il periodo appropriato nel campo **Filtro data**.  

> [!NOTE]  
>   Sono inclusi nel calcolo solo i movimenti del budget contabilità generale con i codici di filtro che vengono immessi nella Scheda dettaglio **Filtri**. I movimenti di budget con codici di filtro diversi o privi di codice ne sono esclusi. Finché il filtro rimane nella finestra nel budget vengono visualizzate unicamente i movimenti con questi codici di filtro.  

> [!TIP]  
>   Se si desidera modificare il budget, è possibile modificare i movimenti del budget. Scegliere un importo per visualizzare i movimenti del budget della contabilità generale sottostanti.

## <a name="to-view-actual-and-budgeted-amounts-for-all-accounts"></a>Per visualizzare gli importi effettivi e preventivati di tutti i conti  
È possibile visualizzare budget di contabilità generale e confrontarli con le cifre effettive in diverse aree di [!INCLUDE[d365fin](includes/d365fin_md.md)].

1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Piano dei conti** e quindi scegliere il collegamento correlato.  
2. Nella finestra **Piano dei conti**, selezionare l'azione **Saldo budget C/G**.
3. All'inizio della finestra, compilare i campi secondo le necessità per definire cosa viene visualizzato.  
4. Per visualizzare una specifica che costituisce l'importo mostrato, selezionare il campo.  

> [!NOTE]  
>   I filtri impostati nella testata della finestra verranno applicati sia ai movimenti C/G che ai movimenti budget.

Le colonne a sinistra contengono il piano dei conti. Delle quattro colonne sulla destra, le prime quattro indicano gli importi dare e avere effettivi e previsti per ciascun conto. La quinta indica la relazione proporzionale tra gli importi effettivi e preventivati del conto C/G.  

> [!TIP]  
>   Utilizzare il campo **Visualizza per** nella finestra **Saldo budget C/G** per selezionare la durata del periodo. Utilizzare il campo **Visualizza come** per selezionare la modalità di calcolo degli importi, **Saldo periodo** o **Saldo alla data**. Scegliere l'azione **Periodo precedente** o **Periodo successivo** per modificare il periodo.  

## <a name="to-view-actual-and-budgeted-amounts-for-several-periods"></a>Per visualizzare importi effettivi e preventivati per più periodi  
Oltre a visualizzare importi effettivi e preventivati di tutti i conti all'interno di un unico periodo è possibile visualizzare un certo numero di periodo per un unico conto.  

1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Piano dei conti** e quindi scegliere il collegamento correlato.  
2. Nella finestra **Piano dei conti**, selezionare il conto di contabilità generale pertinente quindi scegliere l'azione **Confronto budget/contabilità generale**.  
3. All'inizio della finestra, compilare i campi secondo le necessità per definire cosa viene visualizzato.   
4. Per visualizzare una specifica di un importo mostrato, selezionare il campo.  

## <a name="see-also"></a>Vedi anche
[Business Intelligence](bi.md)  
[Utilizzare le situazioni contabili](bi-how-work-account-schedule.md)  
[Finanze](finance.md)  
[Impostazione di dati finanziari](finance-setup-finance.md)  
[Contabilità generale e piano dei conti](finance-general-ledger.md)  
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
