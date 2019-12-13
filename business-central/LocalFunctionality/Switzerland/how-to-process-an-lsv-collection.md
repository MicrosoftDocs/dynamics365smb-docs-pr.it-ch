---
title: Come elaborare una riscossione LSV
description: Utilizzare registrazioni LSV per creare ed elaborare i pagamenti di clienti Lastschrift Verfahren (LSV+). È possibile registrare questi pagamenti nella registrazione incassi, creare un file LSV e stampare il RIBA.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: a12c4fd1f8d5576d25be1487e0dae002161c1766
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 12/03/2019
ms.locfileid: "2881303"
---
# <a name="process-an-lsv-collection"></a><span data-ttu-id="ef3ce-104">Elaborare una riscossione LSV</span><span class="sxs-lookup"><span data-stu-id="ef3ce-104">Process an LSV Collection</span></span>
<span data-ttu-id="ef3ce-105">Utilizzare la pagina **Registrazioni LSV** per creare ed elaborare i pagamenti di clienti Lastschrift Verfahren (LSV+).</span><span class="sxs-lookup"><span data-stu-id="ef3ce-105">You can use the **LSV Journal** page to create and process payments from Lastschrift Verfahren (LSV+) customers.</span></span> <span data-ttu-id="ef3ce-106">È possibile registrare questi pagamenti nella registrazione incassi, creare un file LSV e stampare il RIBA.</span><span class="sxs-lookup"><span data-stu-id="ef3ce-106">You can register these payments in the cash receipt journal, create an LSV file, and then print the collection order.</span></span> <span data-ttu-id="ef3ce-107">Per ulteriori informazioni, vedere la pagina Registrazioni incassi e [Esportare pagamenti tramite LSV](how-to-export-payments-using-lsv.md).</span><span class="sxs-lookup"><span data-stu-id="ef3ce-107">For more information, see the Cash Receipt Journal page and [Export Payments Using LSV](how-to-export-payments-using-lsv.md).</span></span>  

<span data-ttu-id="ef3ce-108">Quando si esegue il processo batch **Riscossione suggerimenti LSV**, ogni riscossione suggerita viene registrata nella riga registrazioni LSV e le fatture aperte vengono trasferite nelle registrazioni LSV.</span><span class="sxs-lookup"><span data-stu-id="ef3ce-108">When you run the **LSV Suggest Collection** batch job, each suggested collection is registered on an LSV journal line, and the open invoices are transferred to the LSV journals.</span></span> <span data-ttu-id="ef3ce-109">Per ulteriori informazioni, vedere la tabella Registrazioni LSV.</span><span class="sxs-lookup"><span data-stu-id="ef3ce-109">For more information, see the LSV Journal table.</span></span>  

<span data-ttu-id="ef3ce-110">È possibile visualizzare, modificare o eliminare le righe pagamenti suggeriti.</span><span class="sxs-lookup"><span data-stu-id="ef3ce-110">You can view, edit, or delete the suggested payment lines.</span></span> <span data-ttu-id="ef3ce-111">Se si corregge l'importo suggerito, la differenza viene contrassegnata come uno sconto.</span><span class="sxs-lookup"><span data-stu-id="ef3ce-111">If you correct the suggested amount, then the difference is marked as a discount.</span></span> <span data-ttu-id="ef3ce-112">È possibile eseguire più volte il processo batch per diversi gruppi di clienti.</span><span class="sxs-lookup"><span data-stu-id="ef3ce-112">You can run the batch job multiple times for different customer groups.</span></span> <span data-ttu-id="ef3ce-113">Le linee di suggerimento possono essere collocate nelle stesse registrazioni.</span><span class="sxs-lookup"><span data-stu-id="ef3ce-113">The suggestion lines can be placed in the same journal.</span></span>  

## <a name="to-create-an-lsv-collection"></a><span data-ttu-id="ef3ce-114">Per creare una riscossione LSV</span><span class="sxs-lookup"><span data-stu-id="ef3ce-114">To create an LSV collection</span></span>  

1.  <span data-ttu-id="ef3ce-115">Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "Icona della funzionalità Cerca pagina o report"), immettere **Lista registrazioni LSV**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="ef3ce-115">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **LSV Journal List**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="ef3ce-116">Scegliere l'azione **Nuovo**.</span><span class="sxs-lookup"><span data-stu-id="ef3ce-116">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="ef3ce-117">Nella pagina **Lista registrazioni LSV** compilare i campi obbligatori come indicato nella tabella riportata di seguito.</span><span class="sxs-lookup"><span data-stu-id="ef3ce-117">On the **LSV Journal List** page, fill in the required fields as described in the following table.</span></span>  

    |<span data-ttu-id="ef3ce-118">Campo</span><span class="sxs-lookup"><span data-stu-id="ef3ce-118">Field</span></span>|<span data-ttu-id="ef3ce-119">Descrizione</span><span class="sxs-lookup"><span data-stu-id="ef3ce-119">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="ef3ce-120">**Codice banca LSV**</span><span class="sxs-lookup"><span data-stu-id="ef3ce-120">**LSV Bank Code**</span></span>|<span data-ttu-id="ef3ce-121">Selezionare il codice banca LSV per la banca che eseguirà la riscossione.</span><span class="sxs-lookup"><span data-stu-id="ef3ce-121">Select the LSV bank code for the bank that will perform the collection.</span></span>|  
    |<span data-ttu-id="ef3ce-122">**Descrizione Registro LSV**</span><span class="sxs-lookup"><span data-stu-id="ef3ce-122">**LSV Journal Description**</span></span>|<span data-ttu-id="ef3ce-123">Immettere una descrizione per il movimento.</span><span class="sxs-lookup"><span data-stu-id="ef3ce-123">Enter a description for the entry.</span></span>|

4.  <span data-ttu-id="ef3ce-124">Selezionare il movimento registrazioni LSV e scegliere l'azione **Riscossione suggerimenti LSV** per creare i pagamenti da riscuotere automaticamente da LSV+.</span><span class="sxs-lookup"><span data-stu-id="ef3ce-124">Select the required LSV journal entry, and then choose the **LSV Suggest Collection** action to create the payments to be collected automatically by LSV+.</span></span>  
5.  <span data-ttu-id="ef3ce-125">Nella pagina **Riscossione suggerimenti LSV**, nella Scheda dettaglio **Opzioni** compilare i campi come descritto nella tabella seguente.</span><span class="sxs-lookup"><span data-stu-id="ef3ce-125">On the **LSV Suggest Collection** page, on the **Options** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="ef3ce-126">Campo</span><span class="sxs-lookup"><span data-stu-id="ef3ce-126">Field</span></span>|<span data-ttu-id="ef3ce-127">Descrizione</span><span class="sxs-lookup"><span data-stu-id="ef3ce-127">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="ef3ce-128">**Nr.**</span><span class="sxs-lookup"><span data-stu-id="ef3ce-128">**No.**</span></span>|<span data-ttu-id="ef3ce-129">Immettere il numero registrazioni LSV.</span><span class="sxs-lookup"><span data-stu-id="ef3ce-129">Enter the LSV journal number.</span></span>|  
    |<span data-ttu-id="ef3ce-130">**Scadenza dal**</span><span class="sxs-lookup"><span data-stu-id="ef3ce-130">**From due date**</span></span>|<span data-ttu-id="ef3ce-131">Specificare la data di scadenza iniziale per i movimenti aperti da suggerire per la riscossione.</span><span class="sxs-lookup"><span data-stu-id="ef3ce-131">Specify the starting due date of open entries to be suggested for collection.</span></span>|  
    |<span data-ttu-id="ef3ce-132">**Scadenza fino al**</span><span class="sxs-lookup"><span data-stu-id="ef3ce-132">**To due date**</span></span>|<span data-ttu-id="ef3ce-133">Specificare la data di scadenza finale per i movimenti aperti da suggerire per la riscossione.</span><span class="sxs-lookup"><span data-stu-id="ef3ce-133">Specify the ending due date of open entries to be suggested for collection.</span></span>|  
    |<span data-ttu-id="ef3ce-134">**Data incasso**</span><span class="sxs-lookup"><span data-stu-id="ef3ce-134">**Collection date**</span></span>|<span data-ttu-id="ef3ce-135">Specifica la data di chiusura della riscossione.</span><span class="sxs-lookup"><span data-stu-id="ef3ce-135">Specify the date on which the collection closes.</span></span> <span data-ttu-id="ef3ce-136">L'ordine LSV+ deve essere inviato almeno tre giorni lavorativi prima della data di riscossione.</span><span class="sxs-lookup"><span data-stu-id="ef3ce-136">The LSV+ order must be submitted at least three banking days before the collection date.</span></span>|  

6.  <span data-ttu-id="ef3ce-137">Scegliere il pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="ef3ce-137">Choose the **OK** button.</span></span>  

<span data-ttu-id="ef3ce-138">Tutte le righe correlate vengono trasferite alle registrazioni LSV.</span><span class="sxs-lookup"><span data-stu-id="ef3ce-138">All related lines are transferred to the LSV journal.</span></span> <span data-ttu-id="ef3ce-139">Dopo aver elaborato la riscossione LSV, è possibile visualizzare, controllare o modificare i pagamenti suggeriti nella pagina **Registrazioni LSV**.</span><span class="sxs-lookup"><span data-stu-id="ef3ce-139">After processing the LSV collection, you can view, check, or edit the suggested payments on the **LSV Journal** page.</span></span> <span data-ttu-id="ef3ce-140">Per ulteriori informazioni, vedere la tabella Riga delle registrazioni LSV.</span><span class="sxs-lookup"><span data-stu-id="ef3ce-140">For more information, see the LSV Journal Line table.</span></span>  

## <a name="to-manage-suggested-payments"></a><span data-ttu-id="ef3ce-141">Per gestire i pagamenti suggeriti</span><span class="sxs-lookup"><span data-stu-id="ef3ce-141">To manage suggested payments</span></span>  

1.  <span data-ttu-id="ef3ce-142">Nella pagina **Lista registrazioni LSV**, selezionare il movimento registrazioni richiesto e scegliere l'azione **Riga delle registrazioni LSV**.</span><span class="sxs-lookup"><span data-stu-id="ef3ce-142">On the **LSV Journal List** page, select the required journal entry, and then choose the **LSV Journal Line** action.</span></span>  

    <span data-ttu-id="ef3ce-143">È possibile visualizzare e modificare i pagamenti suggeriti in questa pagina.</span><span class="sxs-lookup"><span data-stu-id="ef3ce-143">You can view and modify the suggested payments in this page.</span></span> <span data-ttu-id="ef3ce-144">È possibile inserire manualmente i pagamenti richiesti.</span><span class="sxs-lookup"><span data-stu-id="ef3ce-144">You can enter the required payments manually.</span></span> <span data-ttu-id="ef3ce-145">Perle righe registrazioni nuove, il campo **Stato LSV** è impostato su **Aperto** per indicare che la fattura non è pagata.</span><span class="sxs-lookup"><span data-stu-id="ef3ce-145">For new journal lines, the **LSV Status** field is set to **Open** to indicate that the invoice is unpaid.</span></span>  

3.  <span data-ttu-id="ef3ce-146">Scegliere il pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="ef3ce-146">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="ef3ce-147">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="ef3ce-147">See Also</span></span>  
 <span data-ttu-id="ef3ce-148">[Pagamenti elettronici svizzeri tramite LSV+](swiss-electronic-payments-using-lsv-.md) </span><span class="sxs-lookup"><span data-stu-id="ef3ce-148">[Swiss Electronic Payments Using LSV+](swiss-electronic-payments-using-lsv-.md) </span></span>  
 <span data-ttu-id="ef3ce-149">[Chiudere una riscossione LSV](how-to-close-an-lsv-collection.md) </span><span class="sxs-lookup"><span data-stu-id="ef3ce-149">[Close an LSV Collection](how-to-close-an-lsv-collection.md) </span></span>  
 <span data-ttu-id="ef3ce-150">[Registrare pagamenti LSV+](how-to-post-lsv-payments.md) </span><span class="sxs-lookup"><span data-stu-id="ef3ce-150">[Post LSV+ Payments](how-to-post-lsv-payments.md) </span></span>  
 [<span data-ttu-id="ef3ce-151">Esportare pagamenti tramite LSV</span><span class="sxs-lookup"><span data-stu-id="ef3ce-151">Export Payments Using LSV</span></span>](how-to-export-payments-using-lsv.md)
