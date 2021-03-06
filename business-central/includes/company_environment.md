---
author: edupont04
ms.service: dynamics365-accountant
ms.topic: include
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: fa7e5a51696c149e66da0d76cf1042c5e8f7e7e3
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 03/31/2021
ms.locfileid: "5776415"
---
Le persone a volte supportano più di un'azienda e devono passare facilmente da un'azienda a un'altra in [!INCLUDE [prod_short](prod_short.md)]. Ad esempio, un'azienda potrebbe avere uffici di vendita in diverse città e in più paesi, quindi ha creato una business unit separata per ciascun ufficio. Gli uffici che si trovano nello stesso paese sono istituiti come società separate in un ambiente condiviso. Altri uffici vengono creati come aziende in ambienti separati perché sono geograficamente in altri paesi.<br><br>  

Che cos'è un ambiente? Le aziende in [!INCLUDE[prod_short](prod_short.md)] esistono in ciò che viene indicato come *ambiente*. Esistono due tipi di ambienti, **produzione** e **sandbox**. In breve, gli ambienti di produzione contengono dati aziendali in tempo reale e gli ambienti sandbox vengono utilizzati come luogo sicuro per testare operazioni come nuovi processi o funzionalità aziendali. Per ulteriori informazioni, vedere [Tipi di ambienti](/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-environments#types-of-environments). Se è disponibile l'accesso a un'azienda, è disponibile l'accesso all'ambiente in cui si trova. Se si ha accesso a più di una società e tali società si trovano in ambienti diversi, quando si accede a [!INCLUDE[prod_short](prod_short.md)] è necessario specificare l'ambiente in cui si desidera lavorare. Gli ambienti sono specifici di un determinato paese, quindi se l'organizzazione lavora in più paesi, sono necessari ambienti separati per ciascun paese.<br><br>  

Cos'è un'azienda? Una *società* è come contenitore che contiene informazioni su una persona giuridica. Usando l'esempio sopra, l'azienda ha un ufficio vendite a Seattle e un altro a New York, quindi crea una società in [!INCLUDE[prod_short](prod_short.md)] per ogni ufficio in modo che possa gestire le operazioni separatamente per ogni ufficio.  
