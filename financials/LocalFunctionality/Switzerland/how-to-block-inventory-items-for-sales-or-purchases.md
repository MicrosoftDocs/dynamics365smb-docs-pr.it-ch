---
title: Come bloccare gli articoli in magazzino per le vendite o gli acquisti
description: "In Business Central, un articolo può essere contrassegnato come bloccato per la vendita, per l'acquisto o per tutti gli scopi."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 02/02/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: e6e662ee13db1f9002e1c3e74a0d15e2aa2e2a98
ms.openlocfilehash: 4a64a29e005713b3aa8d839bdb21cff3034edc81
ms.contentlocale: it-ch
ms.lasthandoff: 03/22/2018

---
# <a name="block-inventory-items-for-sales-or-purchases"></a>Bloccare gli articoli in magazzino per le vendite o gli acquisti
In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], un articolo può essere contrassegnato come bloccato per la vendita, per l'acquisto o per tutti gli scopi.  

Nella tabella seguente vengono descritti diversi scenari che si verificano quando gli articoli sono bloccati.  

|Articolo contrassegnato come|Risultato|  
|--------------------|------------|  
|**Bloccato Vendita**|Non è possibile usare l'articolo in un documento di vendita né nelle registrazioni di magazzino per l'articolo di vendita.|  
|**Bloccato Acquisto**|Non è possibile usare l'articolo in un documento di acquisto, nelle registrazioni di magazzino per l'articolo di acquisto o nei processi di pianificazione degli acquisti.|  
|**Bloccato**|Non è possibile usare l'articolo per alcuna transazione articolo. Per ulteriori informazioni sul blocco di un articolo per tutti gli scopi, vedere la scheda Articolo.|  

## <a name="to-block-inventory-items-for-sales"></a>Per bloccare gli articoli in magazzino per le vendite  

1.  Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "Cerca pagina o report"), immettere **Articoli**, quindi scegliere il collegamento correlato.  
2.  Scegliere l'articolo che si intende bloccare, quindi scegliere l'azione **Modifica**.  
3.  Per bloccare l'articolo selezionato per le transazioni di vendita, nella Scheda dettaglio **Prezzi e vendite**, selezionare la casella di controllo **Bloccato vendita**.  
4.  Scegliere il pulsante **OK**.  

## <a name="to-block-inventory-items-for-purchase"></a>Per bloccare gli articoli in magazzino per gli acquisti  

1.  Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "Cerca pagina o report"), immettere **Articoli**, quindi scegliere il collegamento correlato.  
2.  Scegliere l'articolo che si intende bloccare, quindi scegliere l'azione **Modifica**.  
3.  Per bloccare un articolo selezionato per le transazioni di acquisto, nella Scheda dettaglio **Rifornimento**, selezionare la casella di controllo **Bloccato acquisto**.  
4.  Scegliere il pulsante **OK**.  

Se si prova a effettuare una delle operazioni seguenti, verrà visualizzato un messaggio di errore:  

- Immettere righe di vendita e di acquisto nei documenti di vendita e di acquisto per gli articoli bloccati. Per ulteriori informazioni, vedere le tabelle Righe vendite e Righe acquisto.  
- Creare nuove righe nelle registrazioni magazzino per gli articoli bloccati. Per ulteriori informazioni, vedere la finestra Registrazioni magazzino.  
- Registrare transazioni articolo per gli articoli bloccati.  

## <a name="see-also"></a>Vedi anche  
 [Gestione del magazzino per la Svizzera](swiss-inventory-management.md)   
 [Copiare articoli esistenti in nuovi articoli](how-to-copy-existing-items-to-new-items.md)   
 [Disattivare la tracciabilità dei costi articolo](how-to-deactivate-item-cost-tracking.md)

