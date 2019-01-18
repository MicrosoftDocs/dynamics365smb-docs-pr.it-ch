---
title: Come creare solleciti di consegna manualmente
description: "In Business Central, è possibile creare solleciti di consegna quando un acquisto non è stato consegnato come previsto. È possibile creare un singolo sollecito di consegna manualmente o generare solleciti di consegna per tutte le consegne scadute."
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
ms.openlocfilehash: 47f646f21495951f1eb7382fb91e4b69e9dd6129
ms.contentlocale: it-ch
ms.lasthandoff: 11/26/2018

---
# <a name="create-delivery-reminders-manually"></a><span data-ttu-id="949cb-104">Creare solleciti di consegna manualmente</span><span class="sxs-lookup"><span data-stu-id="949cb-104">Create Delivery Reminders Manually</span></span>
<span data-ttu-id="949cb-105">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], è possibile creare solleciti di consegna quando un acquisto non è stato consegnato come previsto.</span><span class="sxs-lookup"><span data-stu-id="949cb-105">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you can create delivery reminders when a purchase has not been delivered as expected.</span></span> <span data-ttu-id="949cb-106">È possibile creare un singolo sollecito di consegna manualmente o generare solleciti di consegna per tutte le consegne scadute.</span><span class="sxs-lookup"><span data-stu-id="949cb-106">You can create a single delivery reminder manually, or you can generate delivery reminders for all overdue deliveries.</span></span> <span data-ttu-id="949cb-107">Per ulteriori informazioni, vedere [Generare solleciti di consegna](how-to-generate-delivery-reminders.md).</span><span class="sxs-lookup"><span data-stu-id="949cb-107">For more information, see [Generate Delivery Reminders](how-to-generate-delivery-reminders.md).</span></span>

> [!NOTE]
> <span data-ttu-id="949cb-108">Per creare solleciti di consegna, è necessario impostare le proprietà relative.</span><span class="sxs-lookup"><span data-stu-id="949cb-108">To create delivery reminders, you must set up the delivery reminder properties.</span></span> <span data-ttu-id="949cb-109">Per ulteriori informazioni, vedere [Impostare solleciti di consegna](how-to-set-up-delivery-reminders.md).</span><span class="sxs-lookup"><span data-stu-id="949cb-109">For more information, see [Set Up Delivery Reminders](how-to-set-up-delivery-reminders.md).</span></span>

## <a name="to-create-a-delivery-reminder-manually"></a><span data-ttu-id="949cb-110">Per creare un sollecito di consegna manualmente</span><span class="sxs-lookup"><span data-stu-id="949cb-110">To create a delivery reminder manually</span></span>  

1.  <span data-ttu-id="949cb-111">Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Sollecito di consegna**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="949cb-111">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Delivery Reminder**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="949cb-112">Scegliere l'azione **Nuovo**.</span><span class="sxs-lookup"><span data-stu-id="949cb-112">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="949cb-113">Nella Scheda dettaglio **Generale** della pagina **Sollecito di consegna** compilare i campi come descritto nella tabella seguente.</span><span class="sxs-lookup"><span data-stu-id="949cb-113">On the **Delivery Reminder** page, on the **General** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="949cb-114">Campo</span><span class="sxs-lookup"><span data-stu-id="949cb-114">Field</span></span>|<span data-ttu-id="949cb-115">Descrizione</span><span class="sxs-lookup"><span data-stu-id="949cb-115">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="949cb-116">**Nr.**</span><span class="sxs-lookup"><span data-stu-id="949cb-116">**No.**</span></span>|<span data-ttu-id="949cb-117">Numero di identificazione univoco del sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="949cb-117">The unique identification number for the delivery reminder.</span></span>|  
    |<span data-ttu-id="949cb-118">**N. fornitore**</span><span class="sxs-lookup"><span data-stu-id="949cb-118">**Vendor No.**</span></span>|<span data-ttu-id="949cb-119">Numero del fornitore per cui si desidera registrare il sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="949cb-119">The number of the vendor for whom you want to post the delivery reminder.</span></span><br /><br /> <span data-ttu-id="949cb-120">Quando si seleziona il numero fornitore, i campi **Nome**, **Indirizzo**, **NPA/Città** e **Contatto** vengono compilati automaticamente.</span><span class="sxs-lookup"><span data-stu-id="949cb-120">When you select the vendor number, the **Name**, **Address**, **Post Code/City**, and **Contact** fields are filled in automatically.</span></span>|  
    |<span data-ttu-id="949cb-121">**Data di Registrazione**</span><span class="sxs-lookup"><span data-stu-id="949cb-121">**Posting Date**</span></span>|<span data-ttu-id="949cb-122">Data di registrazione per il sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="949cb-122">The posting date for the delivery reminder.</span></span> <span data-ttu-id="949cb-123">Tale data viene copiata in tutti i movimenti contabili relativi al sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="949cb-123">This date is copied to all of the delivery reminder ledger entries.</span></span>|  
    |<span data-ttu-id="949cb-124">**Data Documento**</span><span class="sxs-lookup"><span data-stu-id="949cb-124">**Document Date**</span></span>|<span data-ttu-id="949cb-125">Data del documento per il sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="949cb-125">The document date for the delivery reminder.</span></span> <span data-ttu-id="949cb-126">Questa data è utilizzata anche per calcolare la data di scadenza per il sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="949cb-126">This date is also used to calculate the due date for the delivery reminder.</span></span> <span data-ttu-id="949cb-127">Se necessario, è possibile modificare la data di registrazione.</span><span class="sxs-lookup"><span data-stu-id="949cb-127">You can modify the posting date if required.</span></span>|  
    |<span data-ttu-id="949cb-128">**Livello di sollecito**</span><span class="sxs-lookup"><span data-stu-id="949cb-128">**Reminder Level**</span></span>|<span data-ttu-id="949cb-129">Livello del sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="949cb-129">The delivery reminder level.</span></span> <span data-ttu-id="949cb-130">Questo valore si basa sul numero di solleciti di consegna già inviati.</span><span class="sxs-lookup"><span data-stu-id="949cb-130">This value is based on the number of delivery reminders that have already been sent.</span></span> <span data-ttu-id="949cb-131">Per ulteriori informazioni, vedere [Impostare termini, livelli e testo dei solleciti di consegna](how-to-set-up-delivery-reminder-terms-levels-and-text.md).</span><span class="sxs-lookup"><span data-stu-id="949cb-131">For more information, see [Set Up Delivery Reminder Terms, Levels, and Text](how-to-set-up-delivery-reminder-terms-levels-and-text.md).</span></span>|  
    |<span data-ttu-id="949cb-132">**Cod. termini di sollecito**</span><span class="sxs-lookup"><span data-stu-id="949cb-132">**Reminder Terms Code**</span></span>|<span data-ttu-id="949cb-133">Specifica il codice dei termini del sollecito di consegna impostato per il fornitore.</span><span class="sxs-lookup"><span data-stu-id="949cb-133">Specify the delivery reminder terms code that is set up for the vendor.</span></span>|  
    |<span data-ttu-id="949cb-134">**Data scad.**</span><span class="sxs-lookup"><span data-stu-id="949cb-134">**Due Date**</span></span>|<span data-ttu-id="949cb-135">Data di scadenza per il sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="949cb-135">The due date for the delivery reminder.</span></span>|  

4.  <span data-ttu-id="949cb-136">Scegliere l'azione selezionare **Suggerisci riga sollecito**</span><span class="sxs-lookup"><span data-stu-id="949cb-136">Choose the **Suggest Reminder Lines** action</span></span>  

    <span data-ttu-id="949cb-137">Se per il fornitore specificato sono presenti consegne scadute, queste vengono aggiunte al sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="949cb-137">If there are overdue deliveries from the specified vendor, these are added to the deliver reminder.</span></span>  

5.  <span data-ttu-id="949cb-138">Scegliere il pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="949cb-138">Choose the **OK** button.</span></span>  

    <span data-ttu-id="949cb-139">Il sollecito di consegna viene creato.</span><span class="sxs-lookup"><span data-stu-id="949cb-139">The delivery reminder is created.</span></span> <span data-ttu-id="949cb-140">È ora possibile emettere e stampare il sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="949cb-140">You can now issue and print the delivery reminder.</span></span>  

## <a name="see-also"></a><span data-ttu-id="949cb-141">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="949cb-141">See Also</span></span>  
 <span data-ttu-id="949cb-142">[Solleciti consegna](delivery-reminders.md) </span><span class="sxs-lookup"><span data-stu-id="949cb-142">[Delivery Reminders](delivery-reminders.md) </span></span>  
 <span data-ttu-id="949cb-143">[Generare solleciti di consegna](how-to-generate-delivery-reminders.md) </span><span class="sxs-lookup"><span data-stu-id="949cb-143">[Generate Delivery Reminders](how-to-generate-delivery-reminders.md) </span></span>  
 <span data-ttu-id="949cb-144">[Impostare solleciti di consegna](how-to-set-up-delivery-reminders.md) </span><span class="sxs-lookup"><span data-stu-id="949cb-144">[Set Up Delivery Reminders](how-to-set-up-delivery-reminders.md) </span></span>  
 <span data-ttu-id="949cb-145">[Impostare i termini, i livelli e i testi di sollecito di consegna](how-to-set-up-delivery-reminder-terms-levels-and-text.md) </span><span class="sxs-lookup"><span data-stu-id="949cb-145">[Set Up Delivery Reminder Terms, Levels, and Text](how-to-set-up-delivery-reminder-terms-levels-and-text.md) </span></span>  
 <span data-ttu-id="949cb-146">[Assegnare codici di solleciti di consegna ai fornitori](how-to-assign-delivery-reminder-codes-to-vendors.md) </span><span class="sxs-lookup"><span data-stu-id="949cb-146">[Assign Delivery Reminder Codes to Vendors](how-to-assign-delivery-reminder-codes-to-vendors.md) </span></span>  
 <span data-ttu-id="949cb-147">[Emettere solleciti di consegna](how-to-issue-delivery-reminders.md) </span><span class="sxs-lookup"><span data-stu-id="949cb-147">[Issue Delivery Reminders](how-to-issue-delivery-reminders.md) </span></span>  
 [<span data-ttu-id="949cb-148">Stampare report di test per i solleciti di consegna</span><span class="sxs-lookup"><span data-stu-id="949cb-148">Print Test Reports for Delivery Reminders</span></span>](how-to-print-test-reports-for-delivery-reminders.md)

