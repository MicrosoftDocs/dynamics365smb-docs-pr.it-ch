---
title: Chiusura dei periodi contabili per un anno fiscale | Documenti Microsoft
description: Descrive come chiudere i periodi contabili alla base di un anno fiscale.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: year closing, close accounting period, close fiscal year, bank account detailed trial balance
ms.date: 04/01/2021
ms.author: jswymer
ms.openlocfilehash: a26baaf947fdac133e3bfcd50489d680231d9971
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 03/31/2021
ms.locfileid: "5786700"
---
# <a name="close-accounting-periods"></a>Chiudere periodi contabili
Al termine di un anno fiscale, è necessario chiudere i periodi di cui è costituito.

## <a name="to-close-accounting-periods"></a>Per chiudere periodi contabili
1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Periodi contabili** e quindi scegliere il collegamento correlato.
2. Nella pagina **Periodi contabili** scegliere l'azione **Chiudi anno**.

    Se più anni fiscali sono aperti, viene automaticamente selezionato quello meno recente per la chiusura. Viene visualizzato un messaggio che identifica l'anno che verrà chiuso e le conseguenze di tale operazione.
3. Per chiudere l'anno, scegliere il pulsante **Sì**.

L'anno fiscale viene chiuso e vengono selezionati i campi **Chiuso** e **Data bloccata** per tutti i periodi dell'anno. L'anno fiscale non può essere riaperto e i segni di spunta nei campi **Chiuso** e **Data bloccata** non possono essere rimossi.

> [!NOTE]  
>   Non è possibile chiudere un anno fiscale prima di crearne uno nuovo. Si noti che una volta chiuso un anno fiscale, non è possibile modificare la data iniziale di quello successivo.

Anche se l'anno fiscale è stato chiuso, è possibile registrarvi dei movimenti C/G. In questo caso, i movimenti vengono contrassegnati come registrati in un anno fiscale chiuso e viene selezionato il campo **Mov. anno prec.**

Una volta chiuso un anno fiscale, è necessario chiudere i conti economici e trasferire i risultati dell'anno su un conto nello stato patrimoniale. È possibile ripetere queste operazioni ogni volta che si effettua una registrazione sull'anno fiscale chiuso.

## <a name="see-also"></a>Vedere anche

[Chiusura registri](year-close-books.md)  
[Registrare il movimento di chiusura di fine anno](year-how-post-year-end-close-entry.md)  
[Utilizzare periodi contabili e anni fiscali](finance-accounting-periods-and-fiscal-years.md)  
[Utilizzo di [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]