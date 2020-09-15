---
title: Come stampare report di liste di pagamenti fornitore
description: Il report Lista pagamenti fornitore fornisce una lista di pagamenti per ogni fornitore. Nel report i pagamenti possono essere ordinati cronologicamente o raggruppati per fornitore.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: edupont
ms.openlocfilehash: 35f867b1aaf62ee41abc96a4caa1d8ce32730edb
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 09/09/2020
ms.locfileid: "3778212"
---
# <a name="print-vendor-payments-list-reports"></a><span data-ttu-id="a1f6e-104">Stampare report di liste di pagamenti fornitore</span><span class="sxs-lookup"><span data-stu-id="a1f6e-104">Print Vendor Payments List Reports</span></span>
<span data-ttu-id="a1f6e-105">Il report **Lista pagamenti fornitore** fornisce una lista di pagamenti per ogni fornitore.</span><span class="sxs-lookup"><span data-stu-id="a1f6e-105">The **Vendor Payments List** report provides a list of payments for each vendor.</span></span> <span data-ttu-id="a1f6e-106">Nel report i pagamenti possono essere ordinati cronologicamente o raggruppati per fornitore.</span><span class="sxs-lookup"><span data-stu-id="a1f6e-106">The report can sort payments chronologically or grouped by vendor.</span></span>  

## <a name="to-print-the-vendor-payments-list-report"></a><span data-ttu-id="a1f6e-107">Per stampare il report di liste di pagamenti fornitore</span><span class="sxs-lookup"><span data-stu-id="a1f6e-107">To print the vendor payments list report</span></span>  

1.  <span data-ttu-id="a1f6e-108">Scegliere l'![icona a forma di lampadina che consente di aprire la funzionalità delle informazioni](../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Lista pagamenti fornitore** e quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="a1f6e-108">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Vendor Payments List**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="a1f6e-109">Nella Scheda dettaglio **Opzioni** compilare i campi come descritto nella tabella riportata di seguito.</span><span class="sxs-lookup"><span data-stu-id="a1f6e-109">On the **Options** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="a1f6e-110">Campo</span><span class="sxs-lookup"><span data-stu-id="a1f6e-110">Field</span></span>|<span data-ttu-id="a1f6e-111">Descrizione</span><span class="sxs-lookup"><span data-stu-id="a1f6e-111">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="a1f6e-112">**Ordinamento**</span><span class="sxs-lookup"><span data-stu-id="a1f6e-112">**Sorting**</span></span>|<span data-ttu-id="a1f6e-113">Specifica l'ordinamento.</span><span class="sxs-lookup"><span data-stu-id="a1f6e-113">Specifies the sort order.</span></span> <span data-ttu-id="a1f6e-114">È possibile eseguire l'ordinamento cronologicamente o per fornitore.</span><span class="sxs-lookup"><span data-stu-id="a1f6e-114">You can sort by vendor or chronologically.</span></span> <span data-ttu-id="a1f6e-115">Se si esegue l'ordinamento per fornitore, verrà visualizzato un subtotale per ogni fornitore.</span><span class="sxs-lookup"><span data-stu-id="a1f6e-115">If you sort by vendor, you will see a subtotal for each vendor.</span></span> <span data-ttu-id="a1f6e-116">Se si esegue l'ordinamento cronologicamente, non verrà visualizzato alcun subtotale.</span><span class="sxs-lookup"><span data-stu-id="a1f6e-116">If you sort chronologically, you will not see subtotals.</span></span>|  
    |<span data-ttu-id="a1f6e-117">**Layout**</span><span class="sxs-lookup"><span data-stu-id="a1f6e-117">**Layout**</span></span>|<span data-ttu-id="a1f6e-118">Specifica il layout del report.</span><span class="sxs-lookup"><span data-stu-id="a1f6e-118">Specifies the layout of the report.</span></span><br /><br /> <span data-ttu-id="a1f6e-119">I risultati possono essere visualizzati nei layout seguenti:</span><span class="sxs-lookup"><span data-stu-id="a1f6e-119">The results can be displayed in the following layouts:</span></span><br /><br /> <span data-ttu-id="a1f6e-120">**Standard**</span><span class="sxs-lookup"><span data-stu-id="a1f6e-120">**Standard**</span></span><br /> <span data-ttu-id="a1f6e-121">Visualizza il numero e il nome del fornitore, nonché i dettagli di registrazione, ad esempio il numero di documento e l'importo in valuta locale.</span><span class="sxs-lookup"><span data-stu-id="a1f6e-121">Displays the vendor number and vendor name, together with posting details, such as the document number and the amount in local currency.</span></span><br /><br /> <span data-ttu-id="a1f6e-122">**Importi VL**</span><span class="sxs-lookup"><span data-stu-id="a1f6e-122">**FCY Amounts**</span></span><br /> <span data-ttu-id="a1f6e-123">Visualizza il numero e il nome del fornitore, il numero del documento, lo stato del pagamento (A per aperto, PP per pagamento parziale e C per chiuso) e l'importo del pagamento.</span><span class="sxs-lookup"><span data-stu-id="a1f6e-123">Displays the vendor number, vendor name, document number, payment status (O for open, PP for partial payment, and C for closed), and payment amount.</span></span><br /><br /> <span data-ttu-id="a1f6e-124">**Informazioni di registrazione**</span><span class="sxs-lookup"><span data-stu-id="a1f6e-124">**Posting Info**</span></span><br /> <span data-ttu-id="a1f6e-125">Visualizza il numero e il nome del fornitore, il costo e l'oggetto di costo, l'ID utente e l'importo di pagamento.</span><span class="sxs-lookup"><span data-stu-id="a1f6e-125">Displays the vendor number, vendor name, cost center, cost object, user ID, and payment amount.</span></span>|  

 <span data-ttu-id="a1f6e-126">Alla fine del report viene visualizzato il numero di pagamenti elaborati.</span><span class="sxs-lookup"><span data-stu-id="a1f6e-126">At the end of the report, the number of processed payments is displayed.</span></span>  

## <a name="see-also"></a><span data-ttu-id="a1f6e-127">Vedere anche</span><span class="sxs-lookup"><span data-stu-id="a1f6e-127">See Also</span></span>  
[<span data-ttu-id="a1f6e-128">Effettuare i pagamenti</span><span class="sxs-lookup"><span data-stu-id="a1f6e-128">Making Payments</span></span>](../../payables-make-payments.md)
