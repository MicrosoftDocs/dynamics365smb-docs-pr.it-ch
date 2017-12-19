---
title: 'Dettagli di progettazione: Il ruolo del punto di riordino | Microsoft Docs'
description: "In questo argomento viene evidenziata l'importanza di impostare un punto di riordino, in modo da sapere quando è necessario approvvigionare il magazzino."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: desigh, reorder, demand, supply
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 5b5e3cec4bc5af8188470ea1d711422c0130677e
ms.contentlocale: it-ch
ms.lasthandoff: 09/22/2017

---
# <a name="design-details-the-role-of-the-reorder-point"></a>Dettagli di progettazione: Il ruolo del punto di riordino
Oltre alla contropartita generale di approvvigionamento e domanda, il sistema di pianificazione deve inoltre monitorare i livelli di magazzino per gli articoli interessati in modo che siano rispettati i metodi di riordino definiti:  
  
Un punto di riordino rappresenta la domanda durante il lead time. Quando la giacenza disponibile scende sotto il livello di magazzino definito dal punto di riordino, è tempo di ordinare una maggiore quantità. Nel frattempo, si prevede una diminuzione graduale della giacenza, che possibilmente raggiunge lo zero (o il livello di scorta di sicurezza), finché non arriva il rifornimento.  
  
Di conseguenza, il sistema di pianificazione suggerirà un ordine di approvvigionamento programmato in avanti alla fase in cui la giacenza prevista passa al di sotto del punto di riordino.  
  
Il punto di riordino riflette un determinato livello di magazzino. Tuttavia, i livelli di magazzino possono spostarsi in modo significativo nell'intervallo di tempo e, pertanto, il sistema di pianificazione deve costantemente monitorare le scorte disponibili previste.  
  
## <a name="see-also"></a>Vedi anche  
[Dettagli di progettazione: Criteri di riordino](design-details-reordering-policies.md)   
[Dettagli di progettazione: Parametri di pianificazione](design-details-planning-parameters.md)   
[Dettagli di progettazione: Gestione dei metodi di riordino](design-details-handling-reordering-policies.md)   
[Dettagli di progettazione: Pianificazione approvvigionamento](design-details-supply-planning.md)