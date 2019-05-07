---
title: Dettagli di progettazione | Microsoft Docs
description: Questo argomento contiene informazioni tecniche dettagliate su funzionalità dell'applicazione complesse in Business Central.
author: SorenGP
documentationcenter: ''
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: e16ebdd8fc7b1b147b17d395241b6e67bb008fd1
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 03/31/2019
ms.locfileid: "911358"
---
# <a name="design-details"></a><span data-ttu-id="866bb-103">Dettagli di progettazione</span><span class="sxs-lookup"><span data-stu-id="866bb-103">Design Details</span></span>
<span data-ttu-id="866bb-104">Questo argomento contiene informazioni tecniche dettagliate su funzionalità dell'applicazione complesse in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="866bb-104">This content contains detailed technical information about complex application features in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

 <span data-ttu-id="866bb-105">Il contenuto di Dettagli di progettazione è destinato a implementatori, sviluppatori e utenti con privilegi avanzati che necessitano di informazioni più approfondite per implementare, personalizzare o configurare le funzionalità in questione.</span><span class="sxs-lookup"><span data-stu-id="866bb-105">Design details content is aimed at implementers, developers, and super users who need deeper insight to implement, customize, or set up the features in question.</span></span>  

|<span data-ttu-id="866bb-106">**Per**</span><span class="sxs-lookup"><span data-stu-id="866bb-106">**To**</span></span>|<span data-ttu-id="866bb-107">**Vedere**</span><span class="sxs-lookup"><span data-stu-id="866bb-107">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="866bb-108">Informazioni sul funzionamento del sistema di pianificazione e su come rettificare gli algoritmi per soddisfare i requisiti di pianificazione in vari ambienti.</span><span class="sxs-lookup"><span data-stu-id="866bb-108">Learn how the planning system works and how to adjust the algorithms to meet planning requirements in different environments.</span></span>|[<span data-ttu-id="866bb-109">Dettagli di progettazione: Pianificazione approvvigionamento</span><span class="sxs-lookup"><span data-stu-id="866bb-109">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)|  
|<span data-ttu-id="866bb-110">Comprendere i meccanismi del motore di costing, ad esempio il metodo di costing e la rettifica costo e i principi di contabilità per cui sono progettati.</span><span class="sxs-lookup"><span data-stu-id="866bb-110">Understand mechanisms in the costing engine, such as costing method and cost adjustment, and which accounting principles they are designed for.</span></span>|[<span data-ttu-id="866bb-111">Dettagli di progettazione: Costing di magazzino</span><span class="sxs-lookup"><span data-stu-id="866bb-111">Design Details: Inventory Costing</span></span>](design-details-inventory-costing.md)|  
|<span data-ttu-id="866bb-112">Informazioni sui principi centrali dietro alle funzionalità di base e avanzate della warehouse e sulla relativa integrazione con altre funzionalità della supply chain.</span><span class="sxs-lookup"><span data-stu-id="866bb-112">Learn about central principles behind advanced and basic warehouse features and how they integrate with other supply chain features.</span></span>|[<span data-ttu-id="866bb-113">Dettagli di progettazione: Gestione warehouse</span><span class="sxs-lookup"><span data-stu-id="866bb-113">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)|  
|<span data-ttu-id="866bb-114">Informazioni sulla progettazione storica e corrente delle funzionalità di tracciabilità articolo e su come si integra con il sistema di impegno per includere i numeri seriali o di lotto nei calcoli della disponibilità.</span><span class="sxs-lookup"><span data-stu-id="866bb-114">Learn about historic and the current design of item tracking functionality and how it integrates with the reservation system to include serial/lot numbers in availability calculations.</span></span>|[<span data-ttu-id="866bb-115">Dettagli di progettazione: Tracciabilità articolo</span><span class="sxs-lookup"><span data-stu-id="866bb-115">Design Details: Item Tracking</span></span>](design-details-item-tracking.md)|  
|<span data-ttu-id="866bb-116">Ottenere informazioni sulla funzionalità della riga di registrazione di contabilità generale, incluse le semplificazioni recenti della progettazione di codeunit 12.</span><span class="sxs-lookup"><span data-stu-id="866bb-116">Learn about the General Journal Posting Line feature, including recent simplifications to the design of codeunit 12.</span></span>|[<span data-ttu-id="866bb-117">Dettagli di progettazione: Riga di registrazione di contabilità generale</span><span class="sxs-lookup"><span data-stu-id="866bb-117">Design Details: General Journal Post Line</span></span>](design-details-general-journal-post-line.md)|
|<span data-ttu-id="866bb-118">Ottenere informazioni sulla progettazione per archiviare e registrare le dimensioni, inclusi gli esempi di codice su come eseguire la migrazione e aggiornare il codice dimensione.</span><span class="sxs-lookup"><span data-stu-id="866bb-118">Learn about the design for storing and posting dimensions, including code examples on how to migrate and upgrade dimension code.</span></span>|[<span data-ttu-id="866bb-119">Dettagli di progettazione: Movimenti set di dimensioni</span><span class="sxs-lookup"><span data-stu-id="866bb-119">Design Details: Dimension Set Entries</span></span>](design-details-dimension-set-entries.md)| 

## <a name="see-also"></a><span data-ttu-id="866bb-120">Vedere anche</span><span class="sxs-lookup"><span data-stu-id="866bb-120">See Also</span></span>  
 <span data-ttu-id="866bb-121">[Pianif.](production-planning.md) </span><span class="sxs-lookup"><span data-stu-id="866bb-121">[Planning](production-planning.md) </span></span>  
 <span data-ttu-id="866bb-122">[Gestione dei costi di magazzino](finance-manage-inventory-costs.md) </span><span class="sxs-lookup"><span data-stu-id="866bb-122">[Managing Inventory Costs](finance-manage-inventory-costs.md) </span></span>  
 <span data-ttu-id="866bb-123">[Gestione warehouse](warehouse-manage-warehouse.md) </span><span class="sxs-lookup"><span data-stu-id="866bb-123">[Warehouse Management](warehouse-manage-warehouse.md) </span></span>  
 [<span data-ttu-id="866bb-124">Impostazione di aree di applicazione complesse utilizzando le procedure ottimali</span><span class="sxs-lookup"><span data-stu-id="866bb-124">Setting Up Complex Application Areas Using Best Practices</span></span>](set-up-complex-application-areas-using-best-practices.md)  
 <span data-ttu-id="866bb-125">[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="866bb-125">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

 ## [!INCLUDE[d365fin](includes/free_trial_md.md)]  
