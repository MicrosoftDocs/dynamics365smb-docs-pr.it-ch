---
title: Come stampare report di liste di pagamenti fornitore
description: Il report Lista pagamenti fornitore fornisce una lista di pagamenti per ogni fornitore. Nel report i pagamenti possono essere ordinati cronologicamente o raggruppati per fornitore.
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
ms.sourcegitcommit: b8a5f4dcfa9a4e3f728c8de3786e7d5716ac82c7
ms.openlocfilehash: bdec8ef89e4c09b3046b4c58683bb86c65815fd8
ms.contentlocale: it-ch
ms.lasthandoff: 10/04/2018

---
# <a name="print-vendor-payments-list-reports"></a><span data-ttu-id="be5b8-104">Stampare report di liste di pagamenti fornitore</span><span class="sxs-lookup"><span data-stu-id="be5b8-104">Print Vendor Payments List Reports</span></span>
<span data-ttu-id="be5b8-105">Il report **Lista pagamenti fornitore** fornisce una lista di pagamenti per ogni fornitore.</span><span class="sxs-lookup"><span data-stu-id="be5b8-105">The **Vendor Payments List** report provides a list of payments for each vendor.</span></span> <span data-ttu-id="be5b8-106">Nel report i pagamenti possono essere ordinati cronologicamente o raggruppati per fornitore.</span><span class="sxs-lookup"><span data-stu-id="be5b8-106">The report can sort payments chronologically or grouped by vendor.</span></span>  

## <a name="to-print-the-vendor-payments-list-report"></a><span data-ttu-id="be5b8-107">Per stampare il report di liste di pagamenti fornitore</span><span class="sxs-lookup"><span data-stu-id="be5b8-107">To print the vendor payments list report</span></span>  

1.  <span data-ttu-id="be5b8-108">Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "Cerca pagina o report"), immettere **Lista pagamenti fornitore**, quindi selezionare il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="be5b8-108">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Vendor Payments List**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="be5b8-109">Nella Scheda dettaglio **Opzioni** compilare i campi come descritto nella tabella riportata di seguito.</span><span class="sxs-lookup"><span data-stu-id="be5b8-109">On the **Options** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="be5b8-110">Campo</span><span class="sxs-lookup"><span data-stu-id="be5b8-110">Field</span></span>|<span data-ttu-id="be5b8-111">Descrizione</span><span class="sxs-lookup"><span data-stu-id="be5b8-111">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="be5b8-112">**Ordinamento**</span><span class="sxs-lookup"><span data-stu-id="be5b8-112">**Sorting**</span></span>|<span data-ttu-id="be5b8-113">Specifica l'ordinamento.</span><span class="sxs-lookup"><span data-stu-id="be5b8-113">Specifies the sort order.</span></span> <span data-ttu-id="be5b8-114">È possibile eseguire l'ordinamento cronologicamente o per fornitore.</span><span class="sxs-lookup"><span data-stu-id="be5b8-114">You can sort by vendor or chronologically.</span></span> <span data-ttu-id="be5b8-115">Se si esegue l'ordinamento per fornitore, verrà visualizzato un subtotale per ogni fornitore.</span><span class="sxs-lookup"><span data-stu-id="be5b8-115">If you sort by vendor, you will see a subtotal for each vendor.</span></span> <span data-ttu-id="be5b8-116">Se si esegue l'ordinamento cronologicamente, non verrà visualizzato alcun subtotale.</span><span class="sxs-lookup"><span data-stu-id="be5b8-116">If you sort chronologically, you will not see subtotals.</span></span>|  
    |<span data-ttu-id="be5b8-117">**Layout**</span><span class="sxs-lookup"><span data-stu-id="be5b8-117">**Layout**</span></span>|<span data-ttu-id="be5b8-118">Specifica il layout del report.</span><span class="sxs-lookup"><span data-stu-id="be5b8-118">Specifies the layout of the report.</span></span><br /><br /> <span data-ttu-id="be5b8-119">I risultati possono essere visualizzati nei layout seguenti:</span><span class="sxs-lookup"><span data-stu-id="be5b8-119">The results can be displayed in the following layouts:</span></span><br /><br /> <span data-ttu-id="be5b8-120">**Standard**</span><span class="sxs-lookup"><span data-stu-id="be5b8-120">**Standard**</span></span><br /> <span data-ttu-id="be5b8-121">Visualizza il numero e il nome del fornitore, nonché i dettagli di registrazione, ad esempio il numero di documento e l'importo in valuta locale.</span><span class="sxs-lookup"><span data-stu-id="be5b8-121">Displays the vendor number and vendor name, together with posting details, such as the document number and the amount in local currency.</span></span><br /><br /> <span data-ttu-id="be5b8-122">**Importi VL**</span><span class="sxs-lookup"><span data-stu-id="be5b8-122">**FCY Amounts**</span></span><br /> <span data-ttu-id="be5b8-123">Visualizza il numero e il nome del fornitore, il numero del documento, lo stato del pagamento (A per aperto, PP per pagamento parziale e C per chiuso) e l'importo del pagamento.</span><span class="sxs-lookup"><span data-stu-id="be5b8-123">Displays the vendor number, vendor name, document number, payment status (O for open, PP for partial payment, and C for closed), and payment amount.</span></span><br /><br /> <span data-ttu-id="be5b8-124">**Informazioni di registrazione**</span><span class="sxs-lookup"><span data-stu-id="be5b8-124">**Posting Info**</span></span><br /> <span data-ttu-id="be5b8-125">Visualizza il numero e il nome del fornitore, il costo e l'oggetto di costo, l'ID utente e l'importo di pagamento.</span><span class="sxs-lookup"><span data-stu-id="be5b8-125">Displays the vendor number, vendor name, cost center, cost object, user ID, and payment amount.</span></span>|  

 <span data-ttu-id="be5b8-126">Alla fine del report viene visualizzato il numero di pagamenti elaborati.</span><span class="sxs-lookup"><span data-stu-id="be5b8-126">At the end of the report, the number of processed payments is displayed.</span></span>  

## <a name="see-also"></a><span data-ttu-id="be5b8-127">Vedere anche</span><span class="sxs-lookup"><span data-stu-id="be5b8-127">See Also</span></span>  
[<span data-ttu-id="be5b8-128">Effettuare i pagamenti</span><span class="sxs-lookup"><span data-stu-id="be5b8-128">Making Payments</span></span>](../../payables-make-payments.md)

