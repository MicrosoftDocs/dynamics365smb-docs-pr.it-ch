---
title: Gestione dei documenti migliorata
description: "In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], è possibile archiviare documenti e tenere traccia delle attività su documenti archiviati e non archiviati."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b34f276a764f0e828fbc1f015429df9852242a4c
ms.openlocfilehash: bc677eb2b3864e569b6f25a0df68301aee709202
ms.contentlocale: it-ch
ms.lasthandoff: 03/22/2018

---
# <a name="enhanced-document-management"></a><span data-ttu-id="fa8dd-103">Gestione dei documenti migliorata</span><span class="sxs-lookup"><span data-stu-id="fa8dd-103">Enhanced Document Management</span></span>
<span data-ttu-id="fa8dd-104">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], è possibile archiviare documenti e tenere traccia delle attività su documenti archiviati e non archiviati.</span><span class="sxs-lookup"><span data-stu-id="fa8dd-104">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you can archive documents and track work across archived and non-archived documents.</span></span>  

## <a name="archiving-documents"></a><span data-ttu-id="fa8dd-105">Archiviazione di documenti</span><span class="sxs-lookup"><span data-stu-id="fa8dd-105">Archiving Documents</span></span>  
 <span data-ttu-id="fa8dd-106">È possibile usare la gestione migliorata dei documenti archiviati per effettuare le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="fa8dd-106">You can use enhanced archive document management to:</span></span>  

- <span data-ttu-id="fa8dd-107">Archiviare ordini programmati</span><span class="sxs-lookup"><span data-stu-id="fa8dd-107">Archive blanket orders</span></span>  
- <span data-ttu-id="fa8dd-108">Copiare documenti</span><span class="sxs-lookup"><span data-stu-id="fa8dd-108">Copy documents</span></span>  
- <span data-ttu-id="fa8dd-109">Tenere traccia delle righe dei documenti</span><span class="sxs-lookup"><span data-stu-id="fa8dd-109">Track document lines</span></span>  

## <a name="archiving-blanket-orders"></a><span data-ttu-id="fa8dd-110">Archiviazione di ordini programmati</span><span class="sxs-lookup"><span data-stu-id="fa8dd-110">Archiving Blanket Orders</span></span>  
<span data-ttu-id="fa8dd-111">È possibile archiviare ordini programmati di acquisto o di vendita ed è possibile usare tali ordini archiviati per creare ordini di vendita e di acquisto standard.</span><span class="sxs-lookup"><span data-stu-id="fa8dd-111">You can archive blanket sales and purchase orders, and use archived blanket sales and purchase orders to create standard sales and purchase orders.</span></span>  

<span data-ttu-id="fa8dd-112">È possibile archiviare automaticamente gli elementi seguenti ogni volta che viene eliminato un ordine o un'offerta:</span><span class="sxs-lookup"><span data-stu-id="fa8dd-112">You can automatically archive the following each time a quote or order is deleted:</span></span>  

- <span data-ttu-id="fa8dd-113">Offerte di vendita o di acquisto</span><span class="sxs-lookup"><span data-stu-id="fa8dd-113">Sales and purchase quotes</span></span>  
- <span data-ttu-id="fa8dd-114">Ordini programmati di vendita e di acquisto</span><span class="sxs-lookup"><span data-stu-id="fa8dd-114">Blanket sales and blanket purchase orders</span></span>  
- <span data-ttu-id="fa8dd-115">Ordini di vendita o di acquisto</span><span class="sxs-lookup"><span data-stu-id="fa8dd-115">Sales and purchase orders</span></span>  

<span data-ttu-id="fa8dd-116">È possibile eliminare la versione archiviata degli ordini programmati di vendita o di acquisto eliminati tramite il processo batch **Elimina versione ordini di acquisto programmati archiviati** o **Elimina versione ordini di vendita programmati archiviati**.</span><span class="sxs-lookup"><span data-stu-id="fa8dd-116">You can delete the archived version of the blanket purchase orders or blanket sales orders that have been deleted using the **Delete Archived Blanket Purchase Order Version** batch job or **Delete Archived Blanket Sales Order Version** batch job.</span></span> <span data-ttu-id="fa8dd-117">È inoltre possibile copiare dettagli da un ordine programmato archiviato in un ordine.</span><span class="sxs-lookup"><span data-stu-id="fa8dd-117">Also, you can copy details from an archived blanket order to an order.</span></span>  

## <a name="tracking-document-lines"></a><span data-ttu-id="fa8dd-118">Tenere traccia delle righe del documento</span><span class="sxs-lookup"><span data-stu-id="fa8dd-118">Tracking Document Lines</span></span>  
<span data-ttu-id="fa8dd-119">È possibile selezionare una riga documento in un tipo di documento e visualizzare e recuperare i documenti correlati.</span><span class="sxs-lookup"><span data-stu-id="fa8dd-119">You can select a document line within a document type, and view and retrieve the related documents.</span></span> <span data-ttu-id="fa8dd-120">È possibile tenere traccia delle righe documento dagli elementi seguenti:</span><span class="sxs-lookup"><span data-stu-id="fa8dd-120">You can track document lines from:</span></span>  

- <span data-ttu-id="fa8dd-121">Ordini</span><span class="sxs-lookup"><span data-stu-id="fa8dd-121">Orders</span></span>  
- <span data-ttu-id="fa8dd-122">Ordini archiviati</span><span class="sxs-lookup"><span data-stu-id="fa8dd-122">Archived orders</span></span>  
- <span data-ttu-id="fa8dd-123">Ordini programmati</span><span class="sxs-lookup"><span data-stu-id="fa8dd-123">Blanket orders</span></span>  
- <span data-ttu-id="fa8dd-124">Ordini programmati archiviati</span><span class="sxs-lookup"><span data-stu-id="fa8dd-124">Archived blanket orders</span></span>  
- <span data-ttu-id="fa8dd-125">Offerte</span><span class="sxs-lookup"><span data-stu-id="fa8dd-125">Quotes</span></span>  
- <span data-ttu-id="fa8dd-126">Offerte archiviate</span><span class="sxs-lookup"><span data-stu-id="fa8dd-126">Archived quotes</span></span>  
- <span data-ttu-id="fa8dd-127">Spedizioni registrate</span><span class="sxs-lookup"><span data-stu-id="fa8dd-127">Posted shipments</span></span>  
- <span data-ttu-id="fa8dd-128">Fatture registrate</span><span class="sxs-lookup"><span data-stu-id="fa8dd-128">Posted invoices</span></span>  

## <a name="see-also"></a><span data-ttu-id="fa8dd-129">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="fa8dd-129">See Also</span></span>  
 <span data-ttu-id="fa8dd-130">[Creare ordini vendita programmati](../../sales-how-to-create-blanket-sales-orders.md) </span><span class="sxs-lookup"><span data-stu-id="fa8dd-130">[Create Blanket Sales Orders](../../sales-how-to-create-blanket-sales-orders.md) </span></span>  
 [<span data-ttu-id="fa8dd-131">Tenere traccia delle righe dei documenti</span><span class="sxs-lookup"><span data-stu-id="fa8dd-131">Track Document Lines</span></span>](how-to-track-document-lines.md)

