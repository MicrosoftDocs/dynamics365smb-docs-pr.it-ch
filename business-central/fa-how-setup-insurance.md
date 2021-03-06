---
title: Impostare l'assicurazione cespiti| Documenti Microsoft
description: Per gestire la copertura assicurativa del cespite è necessario impostare le informazioni generali sull'assicurazione e una scheda assicurazione.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: policy, coverage
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 0ebb62a4ef9ea84ec5bfddc099dfb6120a4e6405
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 03/31/2021
ms.locfileid: "5774059"
---
# <a name="set-up-fixed-asset-insurance"></a>Impostare l'assicurazione cespiti
Per gestire la copertura assicurativa del cespite, è prima necessario impostare alcune informazioni generali sull'assicurazione e una scheda assicurazione per ogni polizza.

## <a name="to-set-up-general-insurance-information"></a>Per impostare le informazioni generali delle assicurazioni
Per utilizzare le funzionalità dell'assicurazione in [!INCLUDE[prod_short](includes/prod_short.md)], occorre impostare alcune informazioni generali sull'assicurazione.  

1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Setup cespiti** e quindi scegliere il collegamento correlato.  
2. Compilare i campi in base alle esigenze. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

## <a name="to-set-up-insurance-types"></a>Per impostare i tipi di assicurazione
È possibile raggruppare le polizze assicurative in categorie, ad esempio assicurazione da furti o incendi. I tipi di assicurazione vengono utilizzati nella Scheda Assicurazione.

1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Tipi di assicurazione** e quindi scegliere il collegamento correlato.  
2. Compilare i campi, se necessario.

## <a name="to-set-up-insurance-cards"></a>Per impostare le schede assicurazione
È possibile raggruppare informazioni relative ad ogni polizza assicurativa nella scheda di assicurazione.  

1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Assicurazione** e quindi scegliere il collegamento correlato.  
2. Scegliere l'azione **Nuovo** nella pagina **Assicurazione** per creare una nuova scheda per l'assicurazione.  
3. Compilare i campi come necessario.

## <a name="to-set-up-insurance-journal-templates"></a>Per impostare le definizioni registrazioni assicurazioni
Una definizione delle registrazioni assicurazioni viene creata automaticamente in [!INCLUDE[prod_short](includes/prod_short.md)] la prima volta che si apre la pagina **Registr. assicuraz.**. È tuttavia possibile impostare definizioni delle registrazioni aggiuntive. Per ulteriori informazioni, vedere [Utilizzo delle registrazioni COGE](ui-work-general-journals.md).  

1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Definizioni registrazioni assicurazioni** e quindi scegliere il collegamento correlato.  
2. Compilare i campi, se necessario.

## <a name="to-set-up-insurance-journal-batches"></a>Per impostare i batch registrazioni assicurazioni
I batch possono essere impostati in una definizione registrazioni assicurazioni. I valori nel batch delle registrazioni vengono utilizzati come valori di default nel caso in cui i campi nelle righe delle registrazioni non siano compilati. Per ulteriori informazioni, vedere [Elaborazione delle registrazioni COGE](ui-work-general-journals.md)  

1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Definizioni registrazioni assicurazioni** e quindi scegliere il collegamento correlato.  
2. Selezionare una definizione registrazioni assicurazione e quindi scegliere l'azione **Batch**.
3. Nella pagina **Batch registrazioni assicurazioni** compilare i campi in base alle esigenze.

> [!NOTE]  
>   I numeri hanno una funzione speciale nei nomi delle registrazioni. Se il nome definizione registrazioni o un nome batch registrazioni contiene un numero, quest'ultimo viene automaticamente incrementato di una unità ogni volta che le registrazioni vengono contabilizzate. Se ad esempio si immette HH1 nel campo **Nome**, il nome della registrazione verrà modificato in HH2 dopo la contabilizzazione della registrazione denominata HH1.

## <a name="see-also"></a>Vedere anche
[Impostazione di cespiti](fa-setup.md)  
[Cespiti](fa-manage.md)  
[Finanze](finance.md)  
[Preparazione al business](ui-get-ready-business.md)  
[Utilizzo di [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]