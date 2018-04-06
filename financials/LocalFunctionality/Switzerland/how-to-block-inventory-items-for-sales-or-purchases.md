---
title: Come bloccare gli articoli in magazzino per le vendite o gli acquisti
description: "In Business Central, un articolo può essere contrassegnato come bloccato per la vendita, per l'acquisto o per tutti gli scopi."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 02/02/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: e6e662ee13db1f9002e1c3e74a0d15e2aa2e2a98
ms.openlocfilehash: 4a64a29e005713b3aa8d839bdb21cff3034edc81
ms.contentlocale: it-ch
ms.lasthandoff: 03/22/2018

---
# <a name="block-inventory-items-for-sales-or-purchases"></a><span data-ttu-id="475ff-103">Bloccare gli articoli in magazzino per le vendite o gli acquisti</span><span class="sxs-lookup"><span data-stu-id="475ff-103">Block Inventory Items for Sales or Purchases</span></span>
<span data-ttu-id="475ff-104">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], un articolo può essere contrassegnato come bloccato per la vendita, per l'acquisto o per tutti gli scopi.</span><span class="sxs-lookup"><span data-stu-id="475ff-104">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], an item can be marked as blocked for sales, blocked for purchase, or blocked for all purposes.</span></span>  

<span data-ttu-id="475ff-105">Nella tabella seguente vengono descritti diversi scenari che si verificano quando gli articoli sono bloccati.</span><span class="sxs-lookup"><span data-stu-id="475ff-105">The following table illustrates what occurs when items are blocked.</span></span>  

|<span data-ttu-id="475ff-106">Articolo contrassegnato come</span><span class="sxs-lookup"><span data-stu-id="475ff-106">Item marked as</span></span>|<span data-ttu-id="475ff-107">Risultato</span><span class="sxs-lookup"><span data-stu-id="475ff-107">Result</span></span>|  
|--------------------|------------|  
|<span data-ttu-id="475ff-108">**Bloccato Vendita**</span><span class="sxs-lookup"><span data-stu-id="475ff-108">**Sale blocked**</span></span>|<span data-ttu-id="475ff-109">Non è possibile usare l'articolo in un documento di vendita né nelle registrazioni di magazzino per l'articolo di vendita.</span><span class="sxs-lookup"><span data-stu-id="475ff-109">You cannot use the item in a sales document or in a sales item journal.</span></span>|  
|<span data-ttu-id="475ff-110">**Bloccato Acquisto**</span><span class="sxs-lookup"><span data-stu-id="475ff-110">**Purchase blocked**</span></span>|<span data-ttu-id="475ff-111">Non è possibile usare l'articolo in un documento di acquisto, nelle registrazioni di magazzino per l'articolo di acquisto o nei processi di pianificazione degli acquisti.</span><span class="sxs-lookup"><span data-stu-id="475ff-111">You cannot use the item in a purchase document, in a purchase item journal, or in purchase planning processes.</span></span>|  
|<span data-ttu-id="475ff-112">**Bloccato**</span><span class="sxs-lookup"><span data-stu-id="475ff-112">**Blocked**</span></span>|<span data-ttu-id="475ff-113">Non è possibile usare l'articolo per alcuna transazione articolo.</span><span class="sxs-lookup"><span data-stu-id="475ff-113">You cannot use the item for any item transaction.</span></span> <span data-ttu-id="475ff-114">Per ulteriori informazioni sul blocco di un articolo per tutti gli scopi, vedere la scheda Articolo.</span><span class="sxs-lookup"><span data-stu-id="475ff-114">For more information about blocking an item for all purposes, see Item Card.</span></span>|  

## <a name="to-block-inventory-items-for-sales"></a><span data-ttu-id="475ff-115">Per bloccare gli articoli in magazzino per le vendite</span><span class="sxs-lookup"><span data-stu-id="475ff-115">To block inventory items for sales</span></span>  

1.  <span data-ttu-id="475ff-116">Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "Cerca pagina o report"), immettere **Articoli**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="475ff-116">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Items**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="475ff-117">Scegliere l'articolo che si intende bloccare, quindi scegliere l'azione **Modifica**.</span><span class="sxs-lookup"><span data-stu-id="475ff-117">Select the item that you want to block, and then choose the **Edit** action.</span></span>  
3.  <span data-ttu-id="475ff-118">Per bloccare l'articolo selezionato per le transazioni di vendita, nella Scheda dettaglio **Prezzi e vendite**, selezionare la casella di controllo **Bloccato vendita**.</span><span class="sxs-lookup"><span data-stu-id="475ff-118">To block the selected item for sales transactions, on the **Prices & Sales** FastTab, select the **Sale blocked** check box.</span></span>  
4.  <span data-ttu-id="475ff-119">Scegliere il pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="475ff-119">Choose the **OK** button.</span></span>  

## <a name="to-block-inventory-items-for-purchase"></a><span data-ttu-id="475ff-120">Per bloccare gli articoli in magazzino per gli acquisti</span><span class="sxs-lookup"><span data-stu-id="475ff-120">To block inventory items for purchase</span></span>  

1.  <span data-ttu-id="475ff-121">Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "Cerca pagina o report"), immettere **Articoli**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="475ff-121">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Items**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="475ff-122">Scegliere l'articolo che si intende bloccare, quindi scegliere l'azione **Modifica**.</span><span class="sxs-lookup"><span data-stu-id="475ff-122">Select the item that you want to block, and then choose the **Edit** action.</span></span>  
3.  <span data-ttu-id="475ff-123">Per bloccare un articolo selezionato per le transazioni di acquisto, nella Scheda dettaglio **Rifornimento**, selezionare la casella di controllo **Bloccato acquisto**.</span><span class="sxs-lookup"><span data-stu-id="475ff-123">To block an item for purchase transactions, on the **Replenishment** FastTab, select the **Purchase blocked** check box.</span></span>  
4.  <span data-ttu-id="475ff-124">Scegliere il pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="475ff-124">Choose the **OK** button.</span></span>  

<span data-ttu-id="475ff-125">Se si prova a effettuare una delle operazioni seguenti, verrà visualizzato un messaggio di errore:</span><span class="sxs-lookup"><span data-stu-id="475ff-125">You will receive an error message if you try to do the following:</span></span>  

- <span data-ttu-id="475ff-126">Immettere righe di vendita e di acquisto nei documenti di vendita e di acquisto per gli articoli bloccati.</span><span class="sxs-lookup"><span data-stu-id="475ff-126">Enter sales lines and purchase lines in sales documents and purchase documents for blocked items.</span></span> <span data-ttu-id="475ff-127">Per ulteriori informazioni, vedere le tabelle Righe vendite e Righe acquisto.</span><span class="sxs-lookup"><span data-stu-id="475ff-127">For more information, see the Sales Line table and the Purchase Line table.</span></span>  
- <span data-ttu-id="475ff-128">Creare nuove righe nelle registrazioni magazzino per gli articoli bloccati.</span><span class="sxs-lookup"><span data-stu-id="475ff-128">Create new lines in an item journal for blocked items.</span></span> <span data-ttu-id="475ff-129">Per ulteriori informazioni, vedere la finestra Registrazioni magazzino.</span><span class="sxs-lookup"><span data-stu-id="475ff-129">For more information, see the Item Journal window.</span></span>  
- <span data-ttu-id="475ff-130">Registrare transazioni articolo per gli articoli bloccati.</span><span class="sxs-lookup"><span data-stu-id="475ff-130">Post item transactions for blocked items.</span></span>  

## <a name="see-also"></a><span data-ttu-id="475ff-131">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="475ff-131">See Also</span></span>  
 <span data-ttu-id="475ff-132">[Gestione del magazzino per la Svizzera](swiss-inventory-management.md) </span><span class="sxs-lookup"><span data-stu-id="475ff-132">[Swiss Inventory Management](swiss-inventory-management.md) </span></span>  
 <span data-ttu-id="475ff-133">[Copiare articoli esistenti in nuovi articoli](how-to-copy-existing-items-to-new-items.md) </span><span class="sxs-lookup"><span data-stu-id="475ff-133">[Copy Existing Items to New Items](how-to-copy-existing-items-to-new-items.md) </span></span>  
 [<span data-ttu-id="475ff-134">Disattivare la tracciabilità dei costi articolo</span><span class="sxs-lookup"><span data-stu-id="475ff-134">Deactivate Item Cost Tracking</span></span>](how-to-deactivate-item-cost-tracking.md)

