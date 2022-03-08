---
title: Come chiudere una riscossione LSV
description: Per scrivere file LSV che possono essere inviati alla banca per la riscossione dei pagamenti, è necessario chiudere le riscossioni Lastchrift Verfahren (LSV+). Quando si chiude una riscossione, questa risulta completata e vengono combinati gli inserimenti nelle registrazioni LSV.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: c850eca99de389f9750e3bc2f7fc0d8a72c4a1cf
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 03/31/2021
ms.locfileid: "5775705"
---
# <a name="close-an-lsv-collection"></a>Chiudere una riscossione LSV
Per scrivere file LSV che possono essere inviati alla banca per la riscossione dei pagamenti, è necessario chiudere le riscossioni Lastchrift Verfahren (LSV+). Quando si chiude una riscossione, questa risulta completata e vengono combinati gli inserimenti nelle registrazioni LSV.  

Quando la riscossione è completata, il numero di riscossione corrente viene assegnato nelle registrazioni LSV, in base all'ultima riscossione. Tale numero LSV viene trasferito ai movimenti clienti per tutte le fatture inevase. Il file di riscossione può essere ricostruito in qualsiasi momento tramite il numero LSV. Il campo **In sospeso** viene inoltre popolato con il valore **LSV** nei movimenti clienti per evitare la duplicazione dei movimenti aperti. Per ulteriori informazioni, vedere le tabelle **Registrazioni LSV** e **Mov. contabili clienti**. È inoltre possibile riaprire una riscossione chiusa.  

## <a name="to-close-an-lsv-collection"></a>Per chiudere una riscossione LSV  

1.  Scegliere l'![icona a forma di lampadina che consente di aprire la funzionalità delle informazioni](../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Lista registrazioni LSV** e quindi scegliere il collegamento correlato.  
2.  Selezionare la riga delle registrazioni richiesta e scegliere l'azione **Modifica data di registrazione**. In questo modo verrà modificato il valore nel campo **Data movimento Avere** usando il valore suggerito durante la riscossione LSV.  
3.  Nel campo **Nuova data** immettere la nuova data.  
4.  Scegliere *l'azione *Chiudi riscossione**.  

    > [!NOTE]  
    >  I campi nella Scheda dettaglio **Opzioni** per il processo batch **Chiudi riscossione LSV** non possono essere modificati e corrispondono alla riga di registrazioni selezionata.  

5.  Scegliere il pulsante **OK**.  

    Nella pagina **Lista registrazioni LSV** il valore del campo **Stato LSV** viene modificato da **Modifica** a **Rilasciato**. Le righe di registrazioni non possono più essere modificate.  

## <a name="to-reopen-an-lsv-collection"></a>Per riaprire una riscossione LSV  

1.  Scegliere l'![icona a forma di lampadina che consente di aprire la funzionalità delle informazioni](../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Lista registrazioni LSV** e quindi scegliere il collegamento correlato.  
2.  Selezionare la riga di registrazioni per cui si desidera riaprire la riscossione, quindi scegliere l'azione **Riapri riscossione**.  

    > [!NOTE]  
    >  È possibile riaprire la riscossione solo se il file LSV+ non è ancora stato inviato alla banca.  

3.  Scegliere il pulsante **Sì** per confermare la riapertura della riscossione.  

## <a name="see-also"></a>Vedi anche  
 [Pagamenti elettronici svizzeri tramite LSV+](swiss-electronic-payments-using-lsv-.md)   
 [Elaborare una riscossione LSV](how-to-process-an-lsv-collection.md)   
 [Registrare pagamenti LSV+](how-to-post-lsv-payments.md)   
 [Esportare pagamenti tramite LSV](how-to-export-payments-using-lsv.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]