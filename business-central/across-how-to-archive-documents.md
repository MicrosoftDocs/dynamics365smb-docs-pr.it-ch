---
title: Come archiviare documenti di acquisto e vendita | Documenti Microsoft
description: "È possibile archiviare ordini di acquisto e vendita, offerte, ordini di reso e ordini programmati e utilizzare il documento archiviato per ricreare il documento da cui è stato archiviato."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: 4827e25d97127faf691b96df9868320bb47dee39
ms.contentlocale: it-ch
ms.lasthandoff: 11/26/2018

---
# <a name="archive-documents"></a><span data-ttu-id="4a3c3-103">Archiviare documenti</span><span class="sxs-lookup"><span data-stu-id="4a3c3-103">Archive Documents</span></span>
<span data-ttu-id="4a3c3-104">È possibile archiviare ordini di acquisto e vendita, offerte, ordini di reso e ordini programmati e utilizzare il documento archiviato per ricreare il documento da cui è stato archiviato.</span><span class="sxs-lookup"><span data-stu-id="4a3c3-104">You can archive sales and purchase orders, quotes, return orders, and blanket orders, and you can use the archived document to recreate the document that it was archived from.</span></span>

## <a name="to-set-up-automatic-document-archiving"></a><span data-ttu-id="4a3c3-105">Per impostare l'archiviazione automatica dei documenti</span><span class="sxs-lookup"><span data-stu-id="4a3c3-105">To set up automatic document archiving</span></span>  
<span data-ttu-id="4a3c3-106">È possibile impostare l'archiviazione automatica di documenti di vendita e di acquisto, offerte, ordini programmati e ordini di reso, prima di eliminarli.</span><span class="sxs-lookup"><span data-stu-id="4a3c3-106">You can set up automatic archiving of sales and purchase orders, quotes, blanket orders, and return orders, before you delete documents.</span></span>

<span data-ttu-id="4a3c3-107">La procedura seguente illustra come configurare l'archiviazione automatica di documenti di vendita.</span><span class="sxs-lookup"><span data-stu-id="4a3c3-107">The following procedure describes how to set up automatic archiving of sales documents.</span></span> <span data-ttu-id="4a3c3-108">I passaggi sono simili per i documenti di acquisto.</span><span class="sxs-lookup"><span data-stu-id="4a3c3-108">The steps are similar for purchase documents.</span></span>
1.  <span data-ttu-id="4a3c3-109">Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Setup contabilità clienti e vendite** e quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="4a3c3-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales & Receivables Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="4a3c3-110">Nella pagina **Setup contabilità clienti e vendite** compilare i campi come descritto di seguito.</span><span class="sxs-lookup"><span data-stu-id="4a3c3-110">On the **Sales & Receivables Setup** page, fill in the fields as follows.</span></span>

|<span data-ttu-id="4a3c3-111">Campo</span><span class="sxs-lookup"><span data-stu-id="4a3c3-111">Field</span></span>|<span data-ttu-id="4a3c3-112">Description</span><span class="sxs-lookup"><span data-stu-id="4a3c3-112">Description</span></span>|
|-----|-----------|
|<span data-ttu-id="4a3c3-113">**Archiviazione Offerte Vendita**</span><span class="sxs-lookup"><span data-stu-id="4a3c3-113">**Archiving Sales Quotes**</span></span>|<span data-ttu-id="4a3c3-114">**Mai** per non archiviare mai offerte di vendita quando vengono eliminate.</span><span class="sxs-lookup"><span data-stu-id="4a3c3-114">**Never** to never archive sales quotes when they are deleted.</span></span> <span data-ttu-id="4a3c3-115">**Domanda** per chiedere all'utente di scegliere se archiviare le offerte di vendita quando vengono eliminate.</span><span class="sxs-lookup"><span data-stu-id="4a3c3-115">**Question** to prompt the user to choose whether to archive sales quotes when they are deleted.</span></span> <span data-ttu-id="4a3c3-116">**Sempre** per non archiviare automaticamente le offerte di vendita quando vengono eliminate.</span><span class="sxs-lookup"><span data-stu-id="4a3c3-116">**Always** to archive sales quotes automatically when they are deleted.</span></span>|
|<span data-ttu-id="4a3c3-117">**Archiviazione ordini di vendita programmati**</span><span class="sxs-lookup"><span data-stu-id="4a3c3-117">**Archiving Blanket Sales Orders**</span></span>|<span data-ttu-id="4a3c3-118">Selezionare questa opzione per archiviare automaticamente gli ordini di vendita programmati ogni volta che vengono eliminati.</span><span class="sxs-lookup"><span data-stu-id="4a3c3-118">Select to archive blanket sales orders automatically each time they are deleted.</span></span>|
|<span data-ttu-id="4a3c3-119">**Ordini archiviati e ordini di reso**</span><span class="sxs-lookup"><span data-stu-id="4a3c3-119">**Arch. Orders and Ret. Orders**</span></span>|<span data-ttu-id="4a3c3-120">Selezionare questa opzione per archiviare automaticamente gli ordini di vendita ogni volta che vengono eliminati.</span><span class="sxs-lookup"><span data-stu-id="4a3c3-120">Select to automatically archive sales orders each time they are deleted.</span></span>|

## <a name="to-archive-a-sales-order"></a><span data-ttu-id="4a3c3-121">Per archiviare un ordine di vendita</span><span class="sxs-lookup"><span data-stu-id="4a3c3-121">To archive a sales order</span></span>
<span data-ttu-id="4a3c3-122">Di seguito viene descritto come archiviare un ordine di vendita.</span><span class="sxs-lookup"><span data-stu-id="4a3c3-122">The following procedure describes how to archive a sales order.</span></span> <span data-ttu-id="4a3c3-123">I passaggi sono simili per tutti gli ordini, gli ordini programmati, gli ordini di reso e le offerte.</span><span class="sxs-lookup"><span data-stu-id="4a3c3-123">The steps are similar for all orders, blanket orders, return orders, and quotes.</span></span>

1.  <span data-ttu-id="4a3c3-124">Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Ordini di vendita** e quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="4a3c3-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="4a3c3-125">Aprire un ordine di vendita da archiviare.</span><span class="sxs-lookup"><span data-stu-id="4a3c3-125">Open a sales order that you want to archive.</span></span>  
3.  <span data-ttu-id="4a3c3-126">Scegliere l'azione **Archivia documento**.</span><span class="sxs-lookup"><span data-stu-id="4a3c3-126">Choose the **Archive Document** action.</span></span>

<span data-ttu-id="4a3c3-127">L'ordine di vendita è archiviato.</span><span class="sxs-lookup"><span data-stu-id="4a3c3-127">The sales order is archived.</span></span> <span data-ttu-id="4a3c3-128">È possibile visualizzarlo nella pagina **Ordine vendite archiviato**.</span><span class="sxs-lookup"><span data-stu-id="4a3c3-128">You can view it on the **Archived Sales orders** page.</span></span> <span data-ttu-id="4a3c3-129">Da qui, è anche possibile utilizzarlo per ricreare l'ordine di vendita da cui è stato archiviato.</span><span class="sxs-lookup"><span data-stu-id="4a3c3-129">From here, you can also use it to recreate the sales order that it was archived from.</span></span>

## <a name="to-recreate-a-sales-order-from-the-archive"></a><span data-ttu-id="4a3c3-130">Per ricreare un ordine di vendita dall'archivio</span><span class="sxs-lookup"><span data-stu-id="4a3c3-130">To recreate a sales order from the archive</span></span>
<span data-ttu-id="4a3c3-131">Di seguito viene descritto come ricreare un ordine di vendita.</span><span class="sxs-lookup"><span data-stu-id="4a3c3-131">The following procedure describes how to recreate a sales order.</span></span> <span data-ttu-id="4a3c3-132">I passaggi sono simili per tutti gli ordini, gli ordini programmati, gli ordini di reso e le offerte.</span><span class="sxs-lookup"><span data-stu-id="4a3c3-132">The steps are similar for all orders, blanket orders, return orders, and quotes.</span></span>

1.  <span data-ttu-id="4a3c3-133">Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Ordini vendita archiviati** e quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="4a3c3-133">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Archived Sales Orders**, and then choose the related link.</span></span>
2.  <span data-ttu-id="4a3c3-134">Selezionare l'ordine di vendita archiviato da ricreare, quindi scegliere l'azione **Ripristina**.</span><span class="sxs-lookup"><span data-stu-id="4a3c3-134">Select the archived sales order that you want to recreate, and then choose the **Restore** action.</span></span>  

<span data-ttu-id="4a3c3-135">L'ordine di vendita viene creato e aggiunto alla pagina **Ordini vendita**.</span><span class="sxs-lookup"><span data-stu-id="4a3c3-135">The sales order is created and added to the **Sales Orders** page.</span></span>

## <a name="to-delete-archived-sales-orders"></a><span data-ttu-id="4a3c3-136">Per eliminare ordini di vendita archiviati</span><span class="sxs-lookup"><span data-stu-id="4a3c3-136">To delete archived sales orders</span></span>
<span data-ttu-id="4a3c3-137">Di seguito viene descritto come eliminare ordini di vendita archiviati.</span><span class="sxs-lookup"><span data-stu-id="4a3c3-137">The following procedure describes how to delete archived sales orders.</span></span> <span data-ttu-id="4a3c3-138">I passaggi sono simili per altri altri documenti di acquisto e vendita archiviati.</span><span class="sxs-lookup"><span data-stu-id="4a3c3-138">The steps are similar for other archived sales and purchase documents.</span></span>

1.  <span data-ttu-id="4a3c3-139">Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Elimina versioni ordine vendita archiviate** e quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="4a3c3-139">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Delete Archived Sales Order Versions**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="4a3c3-140">Nella pagina **Elimina versioni ordine vendita archiviate**, selezionare i filtri appropriati.</span><span class="sxs-lookup"><span data-stu-id="4a3c3-140">On the **Delete Archived Sales Order Versions** page, select the appropriate filters.</span></span>  
3.  <span data-ttu-id="4a3c3-141">Scegliere il pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="4a3c3-141">Choose the **OK** button.</span></span>

## <a name="see-also"></a><span data-ttu-id="4a3c3-142">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="4a3c3-142">See Also</span></span>
[<span data-ttu-id="4a3c3-143">Tenere traccia delle righe dei documenti</span><span class="sxs-lookup"><span data-stu-id="4a3c3-143">Track Document Lines</span></span>](across-how-to-track-document-lines.md)  
[<span data-ttu-id="4a3c3-144">Vendite</span><span class="sxs-lookup"><span data-stu-id="4a3c3-144">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="4a3c3-145">Funzionalità aziendali generali</span><span class="sxs-lookup"><span data-stu-id="4a3c3-145">General Business Functionality</span></span>](ui-across-business-areas.md)  
<span data-ttu-id="4a3c3-146">[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="4a3c3-146">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

