---
title: Come impostare origini e destinazioni dell'allocazione | Microsoft Docs
description: "Ogni allocazione è costituita da un'origine di allocazione e da una o più destinazioni di allocazione. L'origine di allocazione definisce i costi che verranno allocati. Le destinazioni di allocazione determinano dove i costi verranno allocati."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 11/13/2018
ms.author: sgroespe
redirect_url: finance-define-and-allocate-costs
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 0f49faba7360ccf2e93ab62176752a503335f3f1
ms.contentlocale: it-ch
ms.lasthandoff: 09/28/2018

---
# <a name="set-up-allocation-source-and-targets"></a>Impostare origini e destinazioni dell'allocazione
Ogni allocazione è costituita da un'origine di allocazione e da una o più destinazioni di allocazione. L'origine di allocazione definisce i costi che verranno allocati. Le destinazioni di allocazione determinano dove i costi verranno allocati.  

## <a name="to-set-up-cost-allocations"></a>Per impostare le allocazioni costi  
1.  Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Allocazione costi** e quindi scegliere il collegamento correlato.  
2.  Nella finestra **Allocazione costi** scegliere l'azione **Modifica**.  
3.  Immettere un ID dell'origine allocazione nel campo **ID**.  
4.  Definire un livello come numero compreso tra 1 e 99 nel campo **Livello**. La registrazione di allocazione seguirà l'ordine dei livelli.  
5.  Immettere un tipo di costo per definire quali di questi verranno allocati nel campo **Intervallo tipi di costo**. Se tutti i costi per un tipo di costo sono allocati, non viene definito alcun intervallo.  
6.  Immettere un centro di costo insieme ai costi da allocare nel campo **Codice centro di costo**.  
7.  Immettere un oggetto di costo insieme ai costi da allocare nel campo **Codice oggetto di costo**. Molto spesso questo campo rimane vuoto poiché gli oggetti di costo sono raramente allocati ad altri relativi oggetti.  
8.  Immettere un tipo di costo nel campo **Importo dare in tipo di costo**. I costi allocati verranno accreditati al tipo di costo di origine. La registrazione di accredito verrà immessa nel tipo di costo specificato in questo punto.  
9. Definire i target di allocazione nella Scheda dettaglio **Righe**. Nel campo **Tipo di costo di destinazione** della prima riga immettere un tipo di costo. Esso consente di definire a quale tipo di costo viene addebitata l'allocazione.  
10. Nella prima riga immettere la prima destinazione di allocazione nel campo **Centro di costo di destinazione** o **Oggetto di costo di destinazione**. Questi due campi consentono di definire a quale centro di costo o oggetto di costo viene addebitata l'allocazione. È possibile compilare uno di questi campi, ma non entrambi.  
11. Ripetere gli stessi passaggi nella seconda riga per impostare destinazioni di allocazione aggiuntive.  
12. Dopo aver impostato le origini e le destinazioni delle allocazioni, scegliere **Calcola chiave di allocazione** per calcolare i valori delle quote totali.  

> [!NOTE]  
>  Selezionare la casella di controllo **Bloccato** per disattivare l'impostazione dell'allocazione.  

## <a name="see-also"></a>Vedi anche  
[Contabilizzazione dei costi](finance-manage-cost-accounting.md)  
 [Impostazione di filtri per le basi di allocazione dinamica](finance-setting-filters-for-dynamic-allocation-bases.md)   
 [Esempio dello scenario: definizione della allocazioni statiche in base al rapporto di allocazione](finance-scenario-example-defining-static-allocations-based-on-allocation-ratio.md)   
 [Esempio dello scenario: definizione delle allocazioni dinamiche in base agli articoli venduti](finance-scenario-example-defining-dynamic-allocations-based-on-items-sold.md)   
 [Definizione e allocazione dei costi](finance-define-and-allocate-costs.md)   
 [Terminologia della contabilità industriale](finance-terminology-in-cost-accounting.md)  
 [Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
