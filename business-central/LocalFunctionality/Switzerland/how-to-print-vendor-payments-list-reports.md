---
title: Come stampare report di liste di pagamenti fornitore
description: Il report Lista pagamenti fornitore fornisce una lista di pagamenti per ogni fornitore. Nel report i pagamenti possono essere ordinati cronologicamente o raggruppati per fornitore.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: e3d8e38ed8dfa9143c0436c366be1f090b18be55
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 03/31/2019
ms.locfileid: "930519"
---
# <a name="print-vendor-payments-list-reports"></a><span data-ttu-id="04690-104">Stampare report di liste di pagamenti fornitore</span><span class="sxs-lookup"><span data-stu-id="04690-104">Print Vendor Payments List Reports</span></span>
<span data-ttu-id="04690-105">Il report **Lista pagamenti fornitore** fornisce una lista di pagamenti per ogni fornitore.</span><span class="sxs-lookup"><span data-stu-id="04690-105">The **Vendor Payments List** report provides a list of payments for each vendor.</span></span> <span data-ttu-id="04690-106">Nel report i pagamenti possono essere ordinati cronologicamente o raggruppati per fornitore.</span><span class="sxs-lookup"><span data-stu-id="04690-106">The report can sort payments chronologically or grouped by vendor.</span></span>  

## <a name="to-print-the-vendor-payments-list-report"></a><span data-ttu-id="04690-107">Per stampare il report di liste di pagamenti fornitore</span><span class="sxs-lookup"><span data-stu-id="04690-107">To print the vendor payments list report</span></span>  

1.  <span data-ttu-id="04690-108">Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "Cerca pagina o report"), immettere **Lista pagamenti fornitore**, quindi selezionare il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="04690-108">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Vendor Payments List**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="04690-109">Nella Scheda dettaglio **Opzioni** compilare i campi come descritto nella tabella riportata di seguito.</span><span class="sxs-lookup"><span data-stu-id="04690-109">On the **Options** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="04690-110">Campo</span><span class="sxs-lookup"><span data-stu-id="04690-110">Field</span></span>|<span data-ttu-id="04690-111">Descrizione</span><span class="sxs-lookup"><span data-stu-id="04690-111">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="04690-112">**Ordinamento**</span><span class="sxs-lookup"><span data-stu-id="04690-112">**Sorting**</span></span>|<span data-ttu-id="04690-113">Specifica l'ordinamento.</span><span class="sxs-lookup"><span data-stu-id="04690-113">Specifies the sort order.</span></span> <span data-ttu-id="04690-114">È possibile eseguire l'ordinamento cronologicamente o per fornitore.</span><span class="sxs-lookup"><span data-stu-id="04690-114">You can sort by vendor or chronologically.</span></span> <span data-ttu-id="04690-115">Se si esegue l'ordinamento per fornitore, verrà visualizzato un subtotale per ogni fornitore.</span><span class="sxs-lookup"><span data-stu-id="04690-115">If you sort by vendor, you will see a subtotal for each vendor.</span></span> <span data-ttu-id="04690-116">Se si esegue l'ordinamento cronologicamente, non verrà visualizzato alcun subtotale.</span><span class="sxs-lookup"><span data-stu-id="04690-116">If you sort chronologically, you will not see subtotals.</span></span>|  
    |<span data-ttu-id="04690-117">**Layout**</span><span class="sxs-lookup"><span data-stu-id="04690-117">**Layout**</span></span>|<span data-ttu-id="04690-118">Specifica il layout del report.</span><span class="sxs-lookup"><span data-stu-id="04690-118">Specifies the layout of the report.</span></span><br /><br /> <span data-ttu-id="04690-119">I risultati possono essere visualizzati nei layout seguenti:</span><span class="sxs-lookup"><span data-stu-id="04690-119">The results can be displayed in the following layouts:</span></span><br /><br /> <span data-ttu-id="04690-120">**Standard**</span><span class="sxs-lookup"><span data-stu-id="04690-120">**Standard**</span></span><br /> <span data-ttu-id="04690-121">Visualizza il numero e il nome del fornitore, nonché i dettagli di registrazione, ad esempio il numero di documento e l'importo in valuta locale.</span><span class="sxs-lookup"><span data-stu-id="04690-121">Displays the vendor number and vendor name, together with posting details, such as the document number and the amount in local currency.</span></span><br /><br /> <span data-ttu-id="04690-122">**Importi VL**</span><span class="sxs-lookup"><span data-stu-id="04690-122">**FCY Amounts**</span></span><br /> <span data-ttu-id="04690-123">Visualizza il numero e il nome del fornitore, il numero del documento, lo stato del pagamento (A per aperto, PP per pagamento parziale e C per chiuso) e l'importo del pagamento.</span><span class="sxs-lookup"><span data-stu-id="04690-123">Displays the vendor number, vendor name, document number, payment status (O for open, PP for partial payment, and C for closed), and payment amount.</span></span><br /><br /> <span data-ttu-id="04690-124">**Informazioni di registrazione**</span><span class="sxs-lookup"><span data-stu-id="04690-124">**Posting Info**</span></span><br /> <span data-ttu-id="04690-125">Visualizza il numero e il nome del fornitore, il costo e l'oggetto di costo, l'ID utente e l'importo di pagamento.</span><span class="sxs-lookup"><span data-stu-id="04690-125">Displays the vendor number, vendor name, cost center, cost object, user ID, and payment amount.</span></span>|  

 <span data-ttu-id="04690-126">Alla fine del report viene visualizzato il numero di pagamenti elaborati.</span><span class="sxs-lookup"><span data-stu-id="04690-126">At the end of the report, the number of processed payments is displayed.</span></span>  

## <a name="see-also"></a><span data-ttu-id="04690-127">Vedere anche</span><span class="sxs-lookup"><span data-stu-id="04690-127">See Also</span></span>  
[<span data-ttu-id="04690-128">Effettuare i pagamenti</span><span class="sxs-lookup"><span data-stu-id="04690-128">Making Payments</span></span>](../../payables-make-payments.md)
