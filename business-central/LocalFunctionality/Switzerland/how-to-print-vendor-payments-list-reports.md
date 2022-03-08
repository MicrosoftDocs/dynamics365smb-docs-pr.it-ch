---
title: Come stampare report di liste di pagamenti fornitore
description: Il report Lista pagamenti fornitore fornisce una lista di pagamenti per ogni fornitore. Nel report i pagamenti possono essere ordinati cronologicamente o raggruppati per fornitore.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: a9c3c80fcbca4c948543c3cf6f78f31df25d1469
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 03/31/2021
ms.locfileid: "5776548"
---
# <a name="print-vendor-payments-list-reports"></a>Stampare report di liste di pagamenti fornitore

Il report **Lista pagamenti fornitore** fornisce una lista di pagamenti per ogni fornitore. Nel report i pagamenti possono essere ordinati cronologicamente o raggruppati per fornitore.  

> [!NOTE]
> Il report **Lista di pagamenti fornitore** è disponibile nei seguenti mercati: Austria, Germania, Svizzera.

## <a name="to-print-the-vendor-payments-list-report"></a>Per stampare il report di liste di pagamenti fornitore  

1. Scegliere l'![icona a forma di lampadina che consente di aprire la funzionalità delle informazioni](../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Lista pagamenti fornitore** e quindi scegliere il collegamento correlato.  
2. Nella Scheda dettaglio **Opzioni** compilare i campi come descritto nella tabella riportata di seguito.  

    |Campo|Descrizione|  
    |---------------------------------|---------------------------------------|  
    |**Ordinamento**|Specifica l'ordinamento. È possibile eseguire l'ordinamento cronologicamente o per fornitore. Se si esegue l'ordinamento per fornitore, verrà visualizzato un subtotale per ogni fornitore. Se si esegue l'ordinamento cronologicamente, non verrà visualizzato alcun subtotale.|  
    |**Layout**|Specifica il layout del report.<br /><br /> I risultati possono essere visualizzati nei layout seguenti:<br /><br /> **Standard**<br /> Visualizza il numero e il nome del fornitore, nonché i dettagli di registrazione, ad esempio il numero di documento e l'importo in valuta locale.<br /><br /> **Importi VL**<br /> Visualizza il numero e il nome del fornitore, il numero del documento, lo stato del pagamento (A per aperto, PP per pagamento parziale e C per chiuso) e l'importo del pagamento.<br /><br /> **Informazioni di registrazione**<br /> Visualizza il numero e il nome del fornitore, il costo e l'oggetto di costo, l'ID utente e l'importo di pagamento.|  

 Alla fine del report viene visualizzato il numero di pagamenti elaborati.  

## <a name="see-also"></a>Vedere anche

[Effettuare i pagamenti](../../payables-make-payments.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]