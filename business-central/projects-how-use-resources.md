---
title: Registrare e rettificare l'utilizzo e i prezzi delle risorse| Documenti Microsoft
description: Descrive come registrare l'utilizzo o il consumo di risorse associato a una commessa, per tenere traccia e gestire i costi, i prezzi e i tipi di lavoro.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project management, capacity, staff
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 777de65d2cda454491b6c3ea82ebb99d4839dce4
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 03/31/2021
ms.locfileid: "5780400"
---
# <a name="use-resources-for-jobs"></a>Utilizzare le risorse per le commesse
Si registra l'utilizzo di risorse nelle registrazioni commesse per tenere traccia dei costi, dei prezzi e dei tipi di lavoro che sono collegati alle commesse. Per ulteriori informazioni, vedere [Registrare l'utilizzo nelle commesse](projects-how-record-job-usage.md).

> [!NOTE]
> Puoi inoltre acquistare risorse esterne, ad esempio, per fatturare a un fornitore per il lavoro eseguito. Per ulteriori informazioni, vedere [Registrare gli acquisti](purchasing-how-record-purchases.md).

Si può anche registrare l'utilizzo di una risorsa nelle registrazioni risorse. Le voci registrate nelle registrazioni risorse non influiscono sulla contabilità generale.

## <a name="to-assign-resources-to-jobs"></a>Per assegnare le risorse alle commesse
È possibile assegnare le risorse alle commesse creando righe di pianificazione commessa per la commessa. Per ulteriori informazioni, vedere [Creare le commesse](projects-how-create-jobs.md).

## <a name="to-record-resource-usage-for-a-job"></a>Per registrare l'utilizzo delle risorse per una commessa
1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Registrazioni commesse** e quindi scegliere il collegamento correlato.
2. Aprire il batch di registrazioni delle commesse interessato e compilare i campi in base alle esigenze. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. Una volta completate le registrazioni, scegliere l'azione **Registra**.

## <a name="to-adjust-resource-prices"></a>Per rettificare i prezzi delle risorse
Se si desidera modificare i costi o i prezzi di un gran numero di risorse, si può usare un processo batch.  

1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Rettifica costi/prezzi risorse** e quindi scegliere il collegamento correlato.
2. Compilare i campi su una riga in base alle esigenze, quindi scegliere **OK**.

> [!NOTE]  
>   Questo processo batch non consente di creare o rettificare costi e prezzi alternativi per le risorse. Modifica soltanto il contenuto del campo nella scheda risorsa per il campo **Rettifica campo** selezionato nel processo batch. Poiché la rettifica diventerà effettiva immediatamente per le risorse, controllare i fattori di rettifica prima di eseguire il processo batch.

## <a name="to-get-resource-price-change-suggestions-based-on-existing-alternate-prices"></a>Per ottenere suggerimenti per la modifica del prezzo di una risorsa sulla base dei prezzi alternativi esistenti
Se è già stato impostato il prezzo di risorsa alternativo per alcune risorse, è possibile utilizzare un processo batch per impostare più prezzi di risorse alternativi.

1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Modifiche prezzi risorse** e quindi scegliere il collegamento correlato.
2. Scegliere l'azione **Sugg. modif. prezzo ris. (prezzo)** e compilare i campi in base alle esigenze.
3. Scegliere il pulsante **OK**.  
4. Al termine del processo batch, i relativi risultati saranno visualizzati nella pagina **Modifiche prezzi risorsa**.

## <a name="to-get-resource-price-change-suggestions-based-on-standard-prices"></a>Per ottenere suggerimenti per la modifica del prezzo di una risorsa sulla base dei prezzi standard
Se si desidera impostare più prezzi di risorsa alternativi basati sui prezzi standard nelle schede risorse, è possibile utilizzare un processo batch .  

1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Modifiche prezzi risorse** e quindi scegliere il collegamento correlato.
2. Scegliere l'azione **Sugg. mod. prezzo ris. (ris.)** e compilare i campi in base alle esigenze.  
3. Scegliere il pulsante **OK**.  
4. Al termine del processo batch, aprire la pagina **Modifiche prezzi risorsa** per visualizzarne i risultati.

## <a name="to-get-resource-price-change-suggestions-based-on-alternate-prices"></a>Per ottenere suggerimenti per la modifica del prezzo di una risorsa sulla base dei prezzi alternativi
Se è già stato impostato il prezzo di risorsa alternativo per alcune risorse, è possibile utilizzare un processo batch per impostare più prezzi di risorse alternativi.

1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Sugg. mod. prezzo ris.(prezzo)** e quindi scegliere il collegamento correlato.  
2. Compilare i campi, se necessario.
3. Scegliere il pulsante **OK**.  
4. Al termine del processo batch, aprire la pagina **Modifiche prezzi risorsa** per visualizzarne i risultati.

## <a name="see-also"></a>Vedi anche
[Gestione progetti](projects-manage-projects.md)  
[Finanze](finance.md)  
[Acquisti](purchasing-manage-purchasing.md)         
[Vendite](sales-manage-sales.md)     
[Utilizzo di [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]