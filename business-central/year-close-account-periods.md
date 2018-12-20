---
title: Chiusura dei periodi contabili per un anno fiscale | Documenti Microsoft
description: Descrive come chiudere i periodi contabili alla base di un anno fiscale.
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: year closing, close accounting period, close fiscal year, bank account detailed trial balance
ms.date: 10/01/2018
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: f0bdc88cb2d52ed8e1558fb140f904f792e539ff
ms.contentlocale: it-ch
ms.lasthandoff: 09/28/2018

---
# <a name="close-accounting-periods"></a>Chiudere periodi contabili
Al termine di un anno fiscale, è necessario chiudere i periodi di cui è costituito.

## <a name="to-close-accounting-periods"></a>Per chiudere periodi contabili
1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Periodi contabili** e quindi scegliere il collegamento correlato.
2. Nella finestra **Periodi contabili** scegliere l'azione **Chiudi anno**.

    Se più anni fiscali sono aperti, viene automaticamente selezionato quello meno recente per la chiusura. Viene visualizzato un messaggio che identifica l'anno che verrà chiuso e le conseguenze di tale operazione.
3. Per chiudere l'anno, scegliere il pulsante **Sì**.

L'anno fiscale viene chiuso e vengono selezionati i campi **Chiuso** e **Data bloccata** per tutti i periodi dell'anno. L'anno fiscale non può essere riaperto e i segni di spunta nei campi **Chiuso** e **Data bloccata** non possono essere rimossi.

> [!NOTE]  
>   Non è possibile chiudere un anno fiscale prima di crearne uno nuovo. Si noti che una volta chiuso un anno fiscale, non è possibile modificare la data iniziale di quello successivo.

Anche se l'anno fiscale è stato chiuso, è possibile registrarvi dei movimenti C/G. In questo caso, i movimenti vengono contrassegnati come registrati in un anno fiscale chiuso e viene selezionato il campo **Mov. anno prec.**

Una volta chiuso un anno fiscale, è necessario chiudere i conti economici e trasferire i risultati dell'anno su un conto nello stato patrimoniale. È possibile ripetere queste operazioni ogni volta che si effettua una registrazione sull'anno fiscale chiuso.

## <a name="see-also"></a>Vedi anche
[Chiusura registri](year-close-books.md)  
[Registrare il movimento di chiusura di fine anno](year-how-post-year-end-close-entry.md)  
[Aprire un nuovo anno fiscale](finance-how-open-new-fiscal-year.md)  
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
