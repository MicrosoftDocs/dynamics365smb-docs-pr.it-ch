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
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: f447e0c20081cf64709e14cbe524d80fd8075b1c
ms.contentlocale: it-ch
ms.lasthandoff: 11/26/2018

---
# <a name="process-an-lsv-collection"></a><span data-ttu-id="5f61a-104">Elaborare una riscossione LSV</span><span class="sxs-lookup"><span data-stu-id="5f61a-104">Process an LSV Collection</span></span>
<span data-ttu-id="5f61a-105">Utilizzare **Registrazioni LSV** per creare ed elaborare i pagamenti di clienti Lastschrift Verfahren (LSV+).</span><span class="sxs-lookup"><span data-stu-id="5f61a-105">You can use **LSV Journals** to create and process payments from Lastschrift Verfahren (LSV+) customers.</span></span> <span data-ttu-id="5f61a-106">È possibile registrare questi pagamenti nella registrazione incassi, creare un file LSV e stampare il RIBA.</span><span class="sxs-lookup"><span data-stu-id="5f61a-106">You can register these payments in the cash receipt journal, create an LSV file, and then print the collection order.</span></span> <span data-ttu-id="5f61a-107">Per ulteriori informazioni, vedere la pagina Registrazioni incassi e [Esportare pagamenti tramite LSV](how-to-export-payments-using-lsv.md).</span><span class="sxs-lookup"><span data-stu-id="5f61a-107">For more information, see the Cash Receipt Journal page and [Export Payments Using LSV](how-to-export-payments-using-lsv.md).</span></span>  

<span data-ttu-id="5f61a-108">Quando si esegue il processo batch **Riscossione suggerimenti LSV**, ogni riscossione suggerita viene registrata nella riga registrazioni LSV e le fatture aperte vengono trasferite nelle registrazioni LSV.</span><span class="sxs-lookup"><span data-stu-id="5f61a-108">When you run the **LSV Suggest Collection** batch job, each suggested collection is registered on an LSV journal line, and the open invoices are transferred to the LSV journals.</span></span> <span data-ttu-id="5f61a-109">Per ulteriori informazioni, vedere la tabella Registrazioni LSV.</span><span class="sxs-lookup"><span data-stu-id="5f61a-109">For more information, see the LSV Journal table.</span></span>  

<span data-ttu-id="5f61a-110">È possibile visualizzare, modificare o eliminare le righe pagamenti suggeriti.</span><span class="sxs-lookup"><span data-stu-id="5f61a-110">You can view, edit, or delete the suggested payment lines.</span></span> <span data-ttu-id="5f61a-111">Se si corregge l'importo suggerito, la differenza viene contrassegnata come uno sconto.</span><span class="sxs-lookup"><span data-stu-id="5f61a-111">If you correct the suggested amount, then the difference is marked as a discount.</span></span> <span data-ttu-id="5f61a-112">È possibile eseguire più volte il processo batch per diversi gruppi di clienti.</span><span class="sxs-lookup"><span data-stu-id="5f61a-112">You can run the batch job multiple times for different customer groups.</span></span> <span data-ttu-id="5f61a-113">Le linee di suggerimento possono essere collocate nelle stesse registrazioni.</span><span class="sxs-lookup"><span data-stu-id="5f61a-113">The suggestion lines can be placed in the same journal.</span></span>  

## <a name="to-create-an-lsv-collection"></a><span data-ttu-id="5f61a-114">Per creare una riscossione LSV</span><span class="sxs-lookup"><span data-stu-id="5f61a-114">To create an LSV collection</span></span>  

1.  <span data-ttu-id="5f61a-115">Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "Cerca pagina o report"), immettere **Lista registrazioni LSV**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="5f61a-115">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **LSV Journal List**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="5f61a-116">Scegliere l'azione **Nuovo**.</span><span class="sxs-lookup"><span data-stu-id="5f61a-116">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="5f61a-117">Nella pagina **Lista registrazioni LSV** compilare i campi obbligatori come indicato nella tabella riportata di seguito.</span><span class="sxs-lookup"><span data-stu-id="5f61a-117">On the **LSV Journal List** page, fill in the required fields as described in the following table.</span></span>  

    |<span data-ttu-id="5f61a-118">Campo</span><span class="sxs-lookup"><span data-stu-id="5f61a-118">Field</span></span>|<span data-ttu-id="5f61a-119">Descrizione</span><span class="sxs-lookup"><span data-stu-id="5f61a-119">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="5f61a-120">**Codice banca LSV**</span><span class="sxs-lookup"><span data-stu-id="5f61a-120">**LSV Bank Code**</span></span>|<span data-ttu-id="5f61a-121">Selezionare il codice banca LSV per la banca che eseguirà la riscossione.</span><span class="sxs-lookup"><span data-stu-id="5f61a-121">Select the LSV bank code for the bank that will perform the collection.</span></span>|  
    |<span data-ttu-id="5f61a-122">**Descrizione Registro LSV**</span><span class="sxs-lookup"><span data-stu-id="5f61a-122">**LSV Journal Description**</span></span>|<span data-ttu-id="5f61a-123">Immettere una descrizione per il movimento.</span><span class="sxs-lookup"><span data-stu-id="5f61a-123">Enter a description for the entry.</span></span>|

4.  <span data-ttu-id="5f61a-124">Selezionare il movimento registrazioni LSV e scegliere l'azione **Riscossione suggerimenti LSV** per creare i pagamenti da riscuotere automaticamente da LSV+.</span><span class="sxs-lookup"><span data-stu-id="5f61a-124">Select the required LSV journal entry, and then choose the **LSV Suggest Collection** action to create the payments to be collected automatically by LSV+.</span></span>  
5.  <span data-ttu-id="5f61a-125">Nella pagina **Riscossione suggerimenti LSV**, nella Scheda dettaglio **Opzioni** compilare i campi come descritto nella tabella seguente.</span><span class="sxs-lookup"><span data-stu-id="5f61a-125">On the **LSV Suggest Collection** page, on the **Options** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="5f61a-126">Campo</span><span class="sxs-lookup"><span data-stu-id="5f61a-126">Field</span></span>|<span data-ttu-id="5f61a-127">Descrizione</span><span class="sxs-lookup"><span data-stu-id="5f61a-127">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="5f61a-128">**Nr.**</span><span class="sxs-lookup"><span data-stu-id="5f61a-128">**No.**</span></span>|<span data-ttu-id="5f61a-129">Immettere il numero registrazioni LSV.</span><span class="sxs-lookup"><span data-stu-id="5f61a-129">Enter the LSV journal number.</span></span>|  
    |<span data-ttu-id="5f61a-130">**Scadenza dal**</span><span class="sxs-lookup"><span data-stu-id="5f61a-130">**From due date**</span></span>|<span data-ttu-id="5f61a-131">Specificare la data di scadenza iniziale per i movimenti aperti da suggerire per la riscossione.</span><span class="sxs-lookup"><span data-stu-id="5f61a-131">Specify the starting due date of open entries to be suggested for collection.</span></span>|  
    |<span data-ttu-id="5f61a-132">**Scadenza fino al**</span><span class="sxs-lookup"><span data-stu-id="5f61a-132">**To due date**</span></span>|<span data-ttu-id="5f61a-133">Specificare la data di scadenza finale per i movimenti aperti da suggerire per la riscossione.</span><span class="sxs-lookup"><span data-stu-id="5f61a-133">Specify the ending due date of open entries to be suggested for collection.</span></span>|  
    |<span data-ttu-id="5f61a-134">**Data incasso**</span><span class="sxs-lookup"><span data-stu-id="5f61a-134">**Collection date**</span></span>|<span data-ttu-id="5f61a-135">Specifica la data di chiusura della riscossione.</span><span class="sxs-lookup"><span data-stu-id="5f61a-135">Specify the date on which the collection closes.</span></span> <span data-ttu-id="5f61a-136">L'ordine LSV+ deve essere inviato almeno tre giorni lavorativi prima della data di riscossione.</span><span class="sxs-lookup"><span data-stu-id="5f61a-136">The LSV+ order must be submitted at least three banking days before the collection date.</span></span>|  

6.  <span data-ttu-id="5f61a-137">Scegliere il pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="5f61a-137">Choose the **OK** button.</span></span>  

<span data-ttu-id="5f61a-138">Tutte le righe correlate vengono trasferite alle registrazioni LSV.</span><span class="sxs-lookup"><span data-stu-id="5f61a-138">All related lines are transferred to the LSV journal.</span></span> <span data-ttu-id="5f61a-139">Dopo aver elaborato la riscossione LSV, è possibile visualizzare, controllare o modificare i pagamenti suggeriti nella pagina **Registrazioni LSV**.</span><span class="sxs-lookup"><span data-stu-id="5f61a-139">After processing the LSV collection, you can view, check, or edit the suggested payments on the **LSV Journal** page.</span></span> <span data-ttu-id="5f61a-140">Per ulteriori informazioni, vedere la tabella Riga delle registrazioni LSV.</span><span class="sxs-lookup"><span data-stu-id="5f61a-140">For more information, see the LSV Journal Line table.</span></span>  

## <a name="to-manage-suggested-payments"></a><span data-ttu-id="5f61a-141">Per gestire i pagamenti suggeriti</span><span class="sxs-lookup"><span data-stu-id="5f61a-141">To manage suggested payments</span></span>  

1.  <span data-ttu-id="5f61a-142">Nella pagina **Lista registrazioni LSV**, selezionare il movimento registrazioni richiesto e scegliere l'azione **Riga delle registrazioni LSV**.</span><span class="sxs-lookup"><span data-stu-id="5f61a-142">On the **LSV Journal List** page, select the required journal entry, and then choose the **LSV Journal Line** action.</span></span>  

    <span data-ttu-id="5f61a-143">È possibile visualizzare e modificare i pagamenti suggeriti in questa pagina.</span><span class="sxs-lookup"><span data-stu-id="5f61a-143">You can view and modify the suggested payments in this page.</span></span> <span data-ttu-id="5f61a-144">È possibile inserire manualmente i pagamenti richiesti.</span><span class="sxs-lookup"><span data-stu-id="5f61a-144">You can enter the required payments manually.</span></span> <span data-ttu-id="5f61a-145">Perle righe registrazioni nuove, il campo **Stato LSV** è impostato su **Aperto** per indicare che la fattura non è pagata.</span><span class="sxs-lookup"><span data-stu-id="5f61a-145">For new journal lines, the **LSV Status** field is set to **Open** to indicate that the invoice is unpaid.</span></span>  

3.  <span data-ttu-id="5f61a-146">Scegliere il pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="5f61a-146">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="5f61a-147">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="5f61a-147">See Also</span></span>  
 <span data-ttu-id="5f61a-148">[Pagamenti elettronici svizzeri tramite LSV+](swiss-electronic-payments-using-lsv-.md) </span><span class="sxs-lookup"><span data-stu-id="5f61a-148">[Swiss Electronic Payments Using LSV+](swiss-electronic-payments-using-lsv-.md) </span></span>  
 <span data-ttu-id="5f61a-149">[Chiudere una riscossione LSV](how-to-close-an-lsv-collection.md) </span><span class="sxs-lookup"><span data-stu-id="5f61a-149">[Close an LSV Collection](how-to-close-an-lsv-collection.md) </span></span>  
 <span data-ttu-id="5f61a-150">[Registrare pagamenti LSV+](how-to-post-lsv-payments.md) </span><span class="sxs-lookup"><span data-stu-id="5f61a-150">[Post LSV+ Payments](how-to-post-lsv-payments.md) </span></span>  
 [<span data-ttu-id="5f61a-151">Esportare pagamenti tramite LSV</span><span class="sxs-lookup"><span data-stu-id="5f61a-151">Export Payments Using LSV</span></span>](how-to-export-payments-using-lsv.md)

