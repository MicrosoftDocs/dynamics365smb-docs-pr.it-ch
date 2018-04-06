---
title: Come impostare l'archiviazione automatica dei documenti in Svizzera
description: "È possibile impostare l'archiviazione automatica di documenti di vendita e di acquisto, ad esempio offerte, ordini programmati e ordini, prima di eliminarli."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b34f276a764f0e828fbc1f015429df9852242a4c
ms.openlocfilehash: 09fca5cba94bed83b862cd8bb9d4b5be895c509d
ms.contentlocale: it-ch
ms.lasthandoff: 03/22/2018

---
# <a name="set-up-automatic-archiving-of-documents-in-switzerland"></a>Impostare l'archiviazione automatica dei documenti in Svizzera
È possibile impostare l'archiviazione automatica di documenti di vendita e di acquisto, ad esempio offerte, ordini programmati e ordini, prima di eliminarli.  

La procedura seguente descrive come impostare l'archiviazione automatica dei documenti di vendita, ma gli stessi passaggi si applicano anche a documenti di acquisto.  

## <a name="to-set-up-automatic-archiving-of-documents"></a>Per impostare l'archiviazione automatica dei documenti  

1.  Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Setup contabilità clienti e vendite**, quindi scegliere il collegamento correlato.  
2.  Nella Scheda dettaglio **Archiviazione** della finestra **Setup contabilità clienti e vendite** compilare i campi come descritto nella tabella riportata di seguito.  

    |Campo|Descrizione|  
    |---------------------------------|---------------------------------------|  
    |**Archiviazione Offerta Vendita**|**Mai** per non archiviare mai offerte di vendita quando vengono eliminate.<br /><br /> -o-<br /><br /> **Domanda** per chiedere all'utente di scegliere se archiviare le offerte di vendita quando vengono eliminate.<br /><br /> -o-<br /><br /> **Sempre** per non archiviare automaticamente le offerte di vendita quando vengono eliminate.|  
    |**Archiviazione ordini di vendita programmati**|Selezionare questa opzione per archiviare automaticamente gli ordini di vendita programmati ogni volta che vengono eliminati.|  
    |**Ordini archiviati e ordini di reso**|Selezionare questa opzione per archiviare automaticamente gli ordini di vendita ogni volta che vengono eliminati.|  
    |**Log interazione automatico**|Selezionare questa opzione per creare automaticamente un movimento per il contatto nel log interazione quando viene registrato un ordine di vendita o una spedizione parziale o quando un'offerta di vendita viene convertita in un ordine di vendita. **Nota**: questo campo non è disponibile nella pagina **Setup contabilità fornitori e acquisti**.|  

3.  Scegliere il pulsante **OK**.  

## <a name="see-also"></a>Vedi anche  
 [Documenti di acquisto e di vendita per la Svizzera](swiss-purchase-documents-and-sales-documents.md)   
 [Importare codici postali svizzeri](how-to-import-swiss-post-codes.md)   
 [Stampare una lista prelievi magazzino da un ordine di vendita](how-to-print-an-inventory-picking-list-from-a-sales-order.md)   
 [Stampare ordini di vendita e acquisto durante la registrazione batch](how-to-print-sales-and-purchase-orders-during-batch-posting.md)

