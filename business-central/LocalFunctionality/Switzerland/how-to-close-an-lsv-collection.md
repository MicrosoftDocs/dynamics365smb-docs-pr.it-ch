---
title: Come chiudere una riscossione LSV
description: "Per scrivere file LSV che possono essere inviati alla banca per la riscossione dei pagamenti, è necessario chiudere le riscossioni Lastchrift Verfahren (LSV+). Quando si chiude una riscossione, questa risulta completata e vengono combinati gli inserimenti nelle registrazioni LSV."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 4772aa7177e1c0bea6efbb3dc2cbbadf223f954d
ms.contentlocale: it-ch
ms.lasthandoff: 03/22/2018

---
# <a name="close-an-lsv-collection"></a><span data-ttu-id="f63df-104">Chiudere una riscossione LSV</span><span class="sxs-lookup"><span data-stu-id="f63df-104">Close an LSV Collection</span></span>
<span data-ttu-id="f63df-105">Per scrivere file LSV che possono essere inviati alla banca per la riscossione dei pagamenti, è necessario chiudere le riscossioni Lastchrift Verfahren (LSV+).</span><span class="sxs-lookup"><span data-stu-id="f63df-105">You must close Lastschrift Verfahren (LSV+) collections to write LSV files that can be sent to the bank for payment collection.</span></span> <span data-ttu-id="f63df-106">Quando si chiude una riscossione, questa risulta completata e vengono combinati gli inserimenti nelle registrazioni LSV.</span><span class="sxs-lookup"><span data-stu-id="f63df-106">When you close a collection, the collection is complete, and the postings in the LSV journal are combined.</span></span>  

<span data-ttu-id="f63df-107">Quando la riscossione è completata, il numero di riscossione corrente viene assegnato nelle registrazioni LSV, in base all'ultima riscossione.</span><span class="sxs-lookup"><span data-stu-id="f63df-107">When the collection is complete, the current collection number is assigned in the LSV journal, based on the last collection.</span></span> <span data-ttu-id="f63df-108">Tale numero LSV viene trasferito ai movimenti clienti per tutte le fatture inevase.</span><span class="sxs-lookup"><span data-stu-id="f63df-108">This LSV number is transferred to the customer entries for all outstanding invoices.</span></span> <span data-ttu-id="f63df-109">Il file di riscossione può essere ricostruito in qualsiasi momento tramite il numero LSV.</span><span class="sxs-lookup"><span data-stu-id="f63df-109">The collection file can be reconstructed at any time using the LSV number.</span></span> <span data-ttu-id="f63df-110">Il campo **In sospeso** viene inoltre popolato con il valore **LSV** nei movimenti clienti per evitare la duplicazione dei movimenti aperti.</span><span class="sxs-lookup"><span data-stu-id="f63df-110">The **On Hold** field is also populated with **LSV** in the customer entries to avoid the duplication of open entries.</span></span> <span data-ttu-id="f63df-111">Per ulteriori informazioni, vedere le tabelle **Registrazioni LSV** e **Mov. contabili clienti**.</span><span class="sxs-lookup"><span data-stu-id="f63df-111">For more information, see the **LSV Journal** table and the **Cust. Ledger Entry** table.</span></span> <span data-ttu-id="f63df-112">È inoltre possibile riaprire una riscossione chiusa.</span><span class="sxs-lookup"><span data-stu-id="f63df-112">You can also reopen a closed collection.</span></span>  

## <a name="to-close-an-lsv-collection"></a><span data-ttu-id="f63df-113">Per chiudere una riscossione LSV</span><span class="sxs-lookup"><span data-stu-id="f63df-113">To close an LSV collection</span></span>  

1.  <span data-ttu-id="f63df-114">Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "Cerca pagina o report"), immettere **Lista registrazioni LSV**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="f63df-114">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **LSV Journal List**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="f63df-115">Selezionare la riga delle registrazioni richiesta e scegliere l'azione **Modifica data di registrazione**.</span><span class="sxs-lookup"><span data-stu-id="f63df-115">Select the required journal line, and then choose the **Modify Posting Date** action.</span></span> <span data-ttu-id="f63df-116">In questo modo verrà modificato il valore nel campo **Data movimento Avere** usando il valore suggerito durante la riscossione LSV.</span><span class="sxs-lookup"><span data-stu-id="f63df-116">This will modify the value in the **Credit Date** field by using the value suggested during the LSV collection.</span></span>  
3.  <span data-ttu-id="f63df-117">Nel campo **Nuova data** immettere la nuova data.</span><span class="sxs-lookup"><span data-stu-id="f63df-117">In the **New Date** field, enter the new date.</span></span>  
4.  <span data-ttu-id="f63df-118">Scegliere l'azione **Chiudi riscossione**.</span><span class="sxs-lookup"><span data-stu-id="f63df-118">Choose the **Close Collection* action*.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="f63df-119">I campi nella Scheda dettaglio **Opzioni** per il processo batch **Chiudi riscossione LSV** non possono essere modificati e corrispondono alla riga di registrazioni selezionata.</span><span class="sxs-lookup"><span data-stu-id="f63df-119">The fields on the **Options** FastTab for the **LSV Close Collection** batch job cannot be modified, and correspond to the selected journal line.</span></span>  

5.  <span data-ttu-id="f63df-120">Scegliere il pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="f63df-120">Choose the **OK** button.</span></span>  

    <span data-ttu-id="f63df-121">Nella finestra **Lista registrazioni LSV** il valore del campo **Stato LSV** viene modificato da **Modifica** a **Rilasciato**.</span><span class="sxs-lookup"><span data-stu-id="f63df-121">In the **LSV Journal List** window, the value in the **LSV Status** field is changed from **Edit** to **Released**.</span></span> <span data-ttu-id="f63df-122">Le righe di registrazioni non possono più essere modificate.</span><span class="sxs-lookup"><span data-stu-id="f63df-122">The journal lines can no longer be modified.</span></span>  

## <a name="to-reopen-an-lsv-collection"></a><span data-ttu-id="f63df-123">Per riaprire una riscossione LSV</span><span class="sxs-lookup"><span data-stu-id="f63df-123">To reopen an LSV collection</span></span>  

1.  <span data-ttu-id="f63df-124">Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "Cerca pagina o report"), immettere **Lista registrazioni LSV**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="f63df-124">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **LSV Journal List**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="f63df-125">Selezionare la riga di registrazioni per cui si desidera riaprire la riscossione, quindi scegliere l'azione **Riapri riscossione**.</span><span class="sxs-lookup"><span data-stu-id="f63df-125">Select the required journal line for which you want to reopen the collection, on then choose the **Reopen Collection** action.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="f63df-126">È possibile riaprire la riscossione solo se il file LSV+ non è ancora stato inviato alla banca.</span><span class="sxs-lookup"><span data-stu-id="f63df-126">You can only reopen the collection if you have not yet submitted the LSV+ file to the bank.</span></span>  

3.  <span data-ttu-id="f63df-127">Scegliere il pulsante **Sì** per confermare la riapertura della riscossione.</span><span class="sxs-lookup"><span data-stu-id="f63df-127">Choose the **Yes** button to confirm the reopening of the collection.</span></span>  

## <a name="see-also"></a><span data-ttu-id="f63df-128">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="f63df-128">See Also</span></span>  
 <span data-ttu-id="f63df-129">[Pagamenti elettronici svizzeri tramite LSV+](swiss-electronic-payments-using-lsv-.md) </span><span class="sxs-lookup"><span data-stu-id="f63df-129">[Swiss Electronic Payments Using LSV+](swiss-electronic-payments-using-lsv-.md) </span></span>  
 <span data-ttu-id="f63df-130">[Elaborare una riscossione LSV](how-to-process-an-lsv-collection.md) </span><span class="sxs-lookup"><span data-stu-id="f63df-130">[Process an LSV Collection](how-to-process-an-lsv-collection.md) </span></span>  
 <span data-ttu-id="f63df-131">[Registrare pagamenti LSV+](how-to-post-lsv-payments.md) </span><span class="sxs-lookup"><span data-stu-id="f63df-131">[Post LSV+ Payments](how-to-post-lsv-payments.md) </span></span>  
 [<span data-ttu-id="f63df-132">Esportare pagamenti tramite LSV</span><span class="sxs-lookup"><span data-stu-id="f63df-132">Export Payments Using LSV</span></span>](how-to-export-payments-using-lsv.md)

