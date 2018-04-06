---
title: Come elaborare una riscossione LSV
description: "Utilizzare **Registrazioni LSV** per creare ed elaborare i pagamenti di clienti Lastschrift Verfahren (LSV+). È possibile registrare questi pagamenti nella registrazione incassi, creare un file LSV e stampare il RIBA."
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
ms.openlocfilehash: f68c2c4b2b3747d341e7d99372b2e8f056a06bf1
ms.contentlocale: it-ch
ms.lasthandoff: 03/22/2018

---
# <a name="process-an-lsv-collection"></a><span data-ttu-id="c6c4c-104">Elaborare una riscossione LSV</span><span class="sxs-lookup"><span data-stu-id="c6c4c-104">Process an LSV Collection</span></span>
<span data-ttu-id="c6c4c-105">Utilizzare **Registrazioni LSV** per creare ed elaborare i pagamenti di clienti Lastschrift Verfahren (LSV+).</span><span class="sxs-lookup"><span data-stu-id="c6c4c-105">You can use **LSV Journals** to create and process payments from Lastschrift Verfahren (LSV+) customers.</span></span> <span data-ttu-id="c6c4c-106">È possibile registrare questi pagamenti nella registrazione incassi, creare un file LSV e stampare il RIBA.</span><span class="sxs-lookup"><span data-stu-id="c6c4c-106">You can register these payments in the cash receipt journal, create an LSV file, and then print the collection order.</span></span> <span data-ttu-id="c6c4c-107">Per ulteriori informazioni, vedere la finestra Registrazioni incassi e [Esportare pagamenti tramite LSV](how-to-export-payments-using-lsv.md).</span><span class="sxs-lookup"><span data-stu-id="c6c4c-107">For more information, see the Cash Receipt Journal window and [Export Payments Using LSV](how-to-export-payments-using-lsv.md).</span></span>  

<span data-ttu-id="c6c4c-108">Quando si esegue il processo batch **Riscossione suggerimenti LSV**, ogni riscossione suggerita viene registrata nella riga registrazioni LSV e le fatture aperte vengono trasferite nelle registrazioni LSV.</span><span class="sxs-lookup"><span data-stu-id="c6c4c-108">When you run the **LSV Suggest Collection** batch job, each suggested collection is registered on an LSV journal line, and the open invoices are transferred to the LSV journals.</span></span> <span data-ttu-id="c6c4c-109">Per ulteriori informazioni, vedere la tabella Registrazioni LSV.</span><span class="sxs-lookup"><span data-stu-id="c6c4c-109">For more information, see the LSV Journal table.</span></span>  

<span data-ttu-id="c6c4c-110">È possibile visualizzare, modificare o eliminare le righe pagamenti suggeriti.</span><span class="sxs-lookup"><span data-stu-id="c6c4c-110">You can view, edit, or delete the suggested payment lines.</span></span> <span data-ttu-id="c6c4c-111">Se si corregge l'importo suggerito, la differenza viene contrassegnata come uno sconto.</span><span class="sxs-lookup"><span data-stu-id="c6c4c-111">If you correct the suggested amount, then the difference is marked as a discount.</span></span> <span data-ttu-id="c6c4c-112">È possibile eseguire più volte il processo batch per diversi gruppi di clienti.</span><span class="sxs-lookup"><span data-stu-id="c6c4c-112">You can run the batch job multiple times for different customer groups.</span></span> <span data-ttu-id="c6c4c-113">Le linee di suggerimento possono essere collocate nelle stesse registrazioni.</span><span class="sxs-lookup"><span data-stu-id="c6c4c-113">The suggestion lines can be placed in the same journal.</span></span>  

## <a name="to-create-an-lsv-collection"></a><span data-ttu-id="c6c4c-114">Per creare una riscossione LSV</span><span class="sxs-lookup"><span data-stu-id="c6c4c-114">To create an LSV collection</span></span>  

1.  <span data-ttu-id="c6c4c-115">Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "Cerca pagina o report"), immettere **Lista registrazioni LSV**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="c6c4c-115">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **LSV Journal List**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="c6c4c-116">Scegliere l'azione **Nuovo**.</span><span class="sxs-lookup"><span data-stu-id="c6c4c-116">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="c6c4c-117">Nella finestra **Lista registrazioni LSV** compilare i campi obbligatori come indicato nella tabella riportata di seguito.</span><span class="sxs-lookup"><span data-stu-id="c6c4c-117">In the **LSV Journal List** window, fill in the required fields as described in the following table.</span></span>  

    |<span data-ttu-id="c6c4c-118">Campo</span><span class="sxs-lookup"><span data-stu-id="c6c4c-118">Field</span></span>|<span data-ttu-id="c6c4c-119">Descrizione</span><span class="sxs-lookup"><span data-stu-id="c6c4c-119">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="c6c4c-120">**Codice banca LSV**</span><span class="sxs-lookup"><span data-stu-id="c6c4c-120">**LSV Bank Code**</span></span>|<span data-ttu-id="c6c4c-121">Selezionare il codice banca LSV per la banca che eseguirà la riscossione.</span><span class="sxs-lookup"><span data-stu-id="c6c4c-121">Select the LSV bank code for the bank that will perform the collection.</span></span>|  
    |<span data-ttu-id="c6c4c-122">**Descrizione Registro LSV**</span><span class="sxs-lookup"><span data-stu-id="c6c4c-122">**LSV Journal Description**</span></span>|<span data-ttu-id="c6c4c-123">Immettere una descrizione per il movimento.</span><span class="sxs-lookup"><span data-stu-id="c6c4c-123">Enter a description for the entry.</span></span>|

4.  <span data-ttu-id="c6c4c-124">Selezionare il movimento registrazioni LSV e scegliere l'azione **Riscossione suggerimenti LSV** per creare i pagamenti da riscuotere automaticamente da LSV+.</span><span class="sxs-lookup"><span data-stu-id="c6c4c-124">Select the required LSV journal entry, and then choose the **LSV Suggest Collection** action to create the payments to be collected automatically by LSV+.</span></span>  
5.  <span data-ttu-id="c6c4c-125">Nella finestra **Riscossione suggerimenti LSV**, nella Scheda dettaglio **Opzioni** compilare i campi come descritto nella tabella seguente.</span><span class="sxs-lookup"><span data-stu-id="c6c4c-125">In the **LSV Suggest Collection** window, on the **Options** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="c6c4c-126">Campo</span><span class="sxs-lookup"><span data-stu-id="c6c4c-126">Field</span></span>|<span data-ttu-id="c6c4c-127">Descrizione</span><span class="sxs-lookup"><span data-stu-id="c6c4c-127">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="c6c4c-128">**Nr.**</span><span class="sxs-lookup"><span data-stu-id="c6c4c-128">**No.**</span></span>|<span data-ttu-id="c6c4c-129">Immettere il numero registrazioni LSV.</span><span class="sxs-lookup"><span data-stu-id="c6c4c-129">Enter the LSV journal number.</span></span>|  
    |<span data-ttu-id="c6c4c-130">**Scadenza dal**</span><span class="sxs-lookup"><span data-stu-id="c6c4c-130">**From due date**</span></span>|<span data-ttu-id="c6c4c-131">Specificare la data di scadenza iniziale per i movimenti aperti da suggerire per la riscossione.</span><span class="sxs-lookup"><span data-stu-id="c6c4c-131">Specify the starting due date of open entries to be suggested for collection.</span></span>|  
    |<span data-ttu-id="c6c4c-132">**Scadenza fino al**</span><span class="sxs-lookup"><span data-stu-id="c6c4c-132">**To due date**</span></span>|<span data-ttu-id="c6c4c-133">Specificare la data di scadenza finale per i movimenti aperti da suggerire per la riscossione.</span><span class="sxs-lookup"><span data-stu-id="c6c4c-133">Specify the ending due date of open entries to be suggested for collection.</span></span>|  
    |<span data-ttu-id="c6c4c-134">**Data incasso**</span><span class="sxs-lookup"><span data-stu-id="c6c4c-134">**Collection date**</span></span>|<span data-ttu-id="c6c4c-135">Specifica la data di chiusura della riscossione.</span><span class="sxs-lookup"><span data-stu-id="c6c4c-135">Specify the date on which the collection closes.</span></span> <span data-ttu-id="c6c4c-136">L'ordine LSV+ deve essere inviato almeno tre giorni lavorativi prima della data di riscossione.</span><span class="sxs-lookup"><span data-stu-id="c6c4c-136">The LSV+ order must be submitted at least three banking days before the collection date.</span></span>|  

6.  <span data-ttu-id="c6c4c-137">Scegliere il pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="c6c4c-137">Choose the **OK** button.</span></span>  

<span data-ttu-id="c6c4c-138">Tutte le righe correlate vengono trasferite alle registrazioni LSV.</span><span class="sxs-lookup"><span data-stu-id="c6c4c-138">All related lines are transferred to the LSV journal.</span></span> <span data-ttu-id="c6c4c-139">Dopo aver elaborato la riscossione LSV, è possibile visualizzare, controllare o modificare i pagamenti suggeriti nella finestra **Registrazioni LSV**.</span><span class="sxs-lookup"><span data-stu-id="c6c4c-139">After processing the LSV collection, you can view, check, or edit the suggested payments in the **LSV Journal** window.</span></span> <span data-ttu-id="c6c4c-140">Per ulteriori informazioni, vedere la tabella Riga delle registrazioni LSV.</span><span class="sxs-lookup"><span data-stu-id="c6c4c-140">For more information, see the LSV Journal Line table.</span></span>  

## <a name="to-manage-suggested-payments"></a><span data-ttu-id="c6c4c-141">Per gestire i pagamenti suggeriti</span><span class="sxs-lookup"><span data-stu-id="c6c4c-141">To manage suggested payments</span></span>  

1.  <span data-ttu-id="c6c4c-142">Nella finestra **Lista registrazioni LSV**, selezionare il movimento registrazioni richiesto e scegliere l'azione **Riga delle registrazioni LSV**.</span><span class="sxs-lookup"><span data-stu-id="c6c4c-142">In the **LSV Journal List** window, select the required journal entry, and then choose the **LSV Journal Line** action.</span></span>  

    <span data-ttu-id="c6c4c-143">È possibile visualizzare e modificare i pagamenti suggeriti in questa finestra.</span><span class="sxs-lookup"><span data-stu-id="c6c4c-143">You can view and modify the suggested payments in this window.</span></span> <span data-ttu-id="c6c4c-144">È possibile inserire manualmente i pagamenti richiesti.</span><span class="sxs-lookup"><span data-stu-id="c6c4c-144">You can enter the required payments manually.</span></span> <span data-ttu-id="c6c4c-145">Perle righe registrazioni nuove, il campo **Stato LSV** è impostato su **Aperto** per indicare che la fattura non è pagata.</span><span class="sxs-lookup"><span data-stu-id="c6c4c-145">For new journal lines, the **LSV Status** field is set to **Open** to indicate that the invoice is unpaid.</span></span>  

3.  <span data-ttu-id="c6c4c-146">Scegliere il pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="c6c4c-146">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="c6c4c-147">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="c6c4c-147">See Also</span></span>  
 <span data-ttu-id="c6c4c-148">[Pagamenti elettronici svizzeri tramite LSV+](swiss-electronic-payments-using-lsv-.md) </span><span class="sxs-lookup"><span data-stu-id="c6c4c-148">[Swiss Electronic Payments Using LSV+](swiss-electronic-payments-using-lsv-.md) </span></span>  
 <span data-ttu-id="c6c4c-149">[Chiudere una riscossione LSV](how-to-close-an-lsv-collection.md) </span><span class="sxs-lookup"><span data-stu-id="c6c4c-149">[Close an LSV Collection](how-to-close-an-lsv-collection.md) </span></span>  
 <span data-ttu-id="c6c4c-150">[Registrare pagamenti LSV+](how-to-post-lsv-payments.md) </span><span class="sxs-lookup"><span data-stu-id="c6c4c-150">[Post LSV+ Payments](how-to-post-lsv-payments.md) </span></span>  
 [<span data-ttu-id="c6c4c-151">Esportare pagamenti tramite LSV</span><span class="sxs-lookup"><span data-stu-id="c6c4c-151">Export Payments Using LSV</span></span>](how-to-export-payments-using-lsv.md)

