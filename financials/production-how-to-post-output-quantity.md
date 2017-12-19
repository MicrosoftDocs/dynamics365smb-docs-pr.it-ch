---
title: Come registrare l'output e i tempi di lavorazione tramite processo batch| Microsoft Docs
description: "La quantità di output rappresenta la quantità finita nel WIP ( work in progress)."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: ee5ee5d08804439a79f8029eaa25ab7547349a1b
ms.contentlocale: it-ch
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-batch-post-output-and-run-times"></a>Procedura: Registrare l'output e i tempi di lavorazione tramite processo batch
La quantità di output rappresenta la quantità finita nel WIP (work in progress).  

> [!NOTE]
> il magazzino viene aggiornato automaticamente solo quando si registra la quantità di output per l'ultima operazione.  

## <a name="to-post-output-quantities-for-one-or-more-production-order-lines"></a>Per registrare quantità di output per una o più righe dell'ordine di produzione
1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Registrazioni output**, quindi scegliere il collegamento correlato.  
2. Compilare i campi inserendo i dati relativi agli ordini di produzione e all'output. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. Se l'operazione è stata completata, selezionare il campo **Completato** .  

    Se l'ubicazione della warehouse in cui devono essere stoccati gli articoli prevede l'utilizzo di collocazioni, ma non richiede l'elaborazione degli stoccaggi,  assegnare un codice collocazione alla riga delle registrazioni per specificare dove dovranno essere immagazzinati gli articoli nella warehouse. Per ulteriori informazioni, vedere [Procedura: Stoccare l'output produzione o l'output assemblaggio](warehouse-how-to-put-away-production-output.md).  

4. Per registrare le operazioni scegliere l'azione **Registra**. La quantità di output verrà registrata. A questo punto, l'articolo è disponibile per la spedizione.  

## <a name="to-post-run-times-for-one-or-more-production-order-lines"></a>Per registrare il tempo di lavorazione per una o più righe dell'ordine di produzione
Il tempo di lavorazione rappresenta le ore di lavoro necessarie per il WIP (work in progress).    

1.  Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Registrazioni output**, quindi scegliere il collegamento correlato.  
2. Compilare i campi inserendo i dati relativi agli ordini di produzione e all'output.  
3.  Se l'operazione è terminata, selezionare il campo **Completato** .  
4. Scegliere l'azione **Registra** per registrare il tempo impiegato per operazione. I movimenti contabili capacità vengono aggiornati per le aree di produzione o i centri di lavoro utilizzati.

## <a name="see-also"></a>Vedi anche  
[Manufacturing](production-manage-manufacturing.md)    
[Impostazione della produzione](production-configure-production-processes.md)  
[Pianif.](production-planning.md)      
[Magazzino](inventory-manage-inventory.md)  
[Acquisti](purchasing-manage-purchasing.md)  
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
