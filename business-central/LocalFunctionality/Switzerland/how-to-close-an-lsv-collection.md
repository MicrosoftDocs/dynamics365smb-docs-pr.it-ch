---
title: Chiudere una riscossione LSV [CH]
description: Per scrivere file LSV che possono essere inviati alla banca per la riscossione dei pagamenti, è necessario chiudere le riscossioni Lastchrift Verfahren (LSV+).
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.search.form: 3010830, 3010831, 3010832,3010834, 3010835
ms.date: 06/21/2021
ms.author: edupont
ms.openlocfilehash: 5e6d78d3c38866e877acfc5cd87e8827027ae480
ms.sourcegitcommit: ef80c461713fff1a75998766e7a4ed3a7c6121d0
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 02/15/2022
ms.locfileid: "8146004"
---
# <a name="close-an-lsv-collection-in-the-swiss-version"></a>Chiudere una riscossione LSV nella versione per la Svizzera
Per scrivere file LSV che possono essere inviati alla banca per la riscossione dei pagamenti, è necessario chiudere le riscossioni Lastchrift Verfahren (LSV+). Quando si chiude una riscossione, questa risulta completata e vengono combinati gli inserimenti nelle registrazioni LSV.  

Quando la riscossione è completata, il numero di riscossione corrente viene assegnato nelle registrazioni LSV, in base all'ultima riscossione. Tale numero LSV viene trasferito ai movimenti clienti per tutte le fatture inevase. Il file di riscossione può essere ricostruito in qualsiasi momento tramite il numero LSV. Il campo **In sospeso** viene inoltre popolato con il valore **LSV** nei movimenti clienti per evitare la duplicazione dei movimenti aperti. Per ulteriori informazioni, vedere le tabelle **Registrazioni LSV** e **Mov. contabili clienti**. È inoltre possibile riaprire una riscossione chiusa.  

## <a name="to-close-an-lsv-collection"></a>Per chiudere una riscossione LSV  

1.  Scegliere la ![lampadina che apre la funzionalità delle informazioni.](../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immettere **Lista registrazioni LSV**, quindi selezionare il collegamento correlato.  
2.  Selezionare la riga delle registrazioni richiesta e scegliere l'azione **Modifica data di registrazione**. In questo modo verrà modificato il valore nel campo **Data movimento Avere** usando il valore suggerito durante la riscossione LSV.  
3.  Nel campo **Nuova data** immettere la nuova data.  
4.  Scegliere *l'azione *Chiudi riscossione**.  

    > [!NOTE]  
    >  I campi nella Scheda dettaglio **Opzioni** per il processo batch **Chiudi riscossione LSV** non possono essere modificati e corrispondono alla riga di registrazioni selezionata.  

5.  Scegliere il pulsante **OK**.  

    Nella pagina **Lista registrazioni LSV** il valore del campo **Stato LSV** viene modificato da **Modifica** a **Rilasciato**. Le righe di registrazioni non possono più essere modificate.  

## <a name="to-reopen-an-lsv-collection"></a>Per riaprire una riscossione LSV  

1.  Scegliere la ![lampadina che apre la funzionalità delle informazioni.](../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immettere **Lista registrazioni LSV**, quindi selezionare il collegamento correlato.  
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