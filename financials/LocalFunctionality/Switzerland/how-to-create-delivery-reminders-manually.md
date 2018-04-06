---
title: Come creare solleciti di consegna manualmente
description: In ADD INCLUDE<!--[!INCLUDE[navnow](../../includes/how-to-generate-delivery-reminders.md).
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
ms.openlocfilehash: 7e82038dc676da036419b47f9685b3678ce8d06e
ms.contentlocale: it-ch
ms.lasthandoff: 03/22/2018

---
# <a name="create-delivery-reminders-manually"></a><span data-ttu-id="2db4c-103">Creare solleciti di consegna manualmente</span><span class="sxs-lookup"><span data-stu-id="2db4c-103">Create Delivery Reminders Manually</span></span>
<span data-ttu-id="2db4c-104">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], è possibile creare solleciti di consegna quando un acquisto non è stato consegnato come previsto.</span><span class="sxs-lookup"><span data-stu-id="2db4c-104">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you can create delivery reminders when a purchase has not been delivered as expected.</span></span> <span data-ttu-id="2db4c-105">È possibile creare un singolo sollecito di consegna manualmente o generare solleciti di consegna per tutte le consegne scadute.</span><span class="sxs-lookup"><span data-stu-id="2db4c-105">You can create a single delivery reminder manually, or you can generate delivery reminders for all overdue deliveries.</span></span> <span data-ttu-id="2db4c-106">Per ulteriori informazioni, vedere [Generare solleciti di consegna](how-to-generate-delivery-reminders.md).</span><span class="sxs-lookup"><span data-stu-id="2db4c-106">For more information, see [Generate Delivery Reminders](how-to-generate-delivery-reminders.md).</span></span>

> [!NOTE]
> <span data-ttu-id="2db4c-107">Per creare solleciti di consegna, è necessario impostare le proprietà relative.</span><span class="sxs-lookup"><span data-stu-id="2db4c-107">To create delivery reminders, you must set up the delivery reminder properties.</span></span> <span data-ttu-id="2db4c-108">Per ulteriori informazioni, vedere [Impostare solleciti di consegna](how-to-set-up-delivery-reminders.md).</span><span class="sxs-lookup"><span data-stu-id="2db4c-108">For more information, see [Set Up Delivery Reminders](how-to-set-up-delivery-reminders.md).</span></span>

## <a name="to-create-a-delivery-reminder-manually"></a><span data-ttu-id="2db4c-109">Per creare un sollecito di consegna manualmente</span><span class="sxs-lookup"><span data-stu-id="2db4c-109">To create a delivery reminder manually</span></span>  

1.  <span data-ttu-id="2db4c-110">Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Sollecito di consegna**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="2db4c-110">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Delivery Reminder**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="2db4c-111">Scegliere l'azione **Nuovo**.</span><span class="sxs-lookup"><span data-stu-id="2db4c-111">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="2db4c-112">Nella Scheda dettaglio **Generale** della finestra **Sollecito di consegna** compilare i campi come descritto nella tabella seguente.</span><span class="sxs-lookup"><span data-stu-id="2db4c-112">In the **Delivery Reminder** window, on the **General** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="2db4c-113">Campo</span><span class="sxs-lookup"><span data-stu-id="2db4c-113">Field</span></span>|<span data-ttu-id="2db4c-114">Descrizione</span><span class="sxs-lookup"><span data-stu-id="2db4c-114">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="2db4c-115">**Nr.**</span><span class="sxs-lookup"><span data-stu-id="2db4c-115">**No.**</span></span>|<span data-ttu-id="2db4c-116">Numero di identificazione univoco del sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="2db4c-116">The unique identification number for the delivery reminder.</span></span>|  
    |<span data-ttu-id="2db4c-117">**N. fornitore**</span><span class="sxs-lookup"><span data-stu-id="2db4c-117">**Vendor No.**</span></span>|<span data-ttu-id="2db4c-118">Numero del fornitore per cui si desidera registrare il sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="2db4c-118">The number of the vendor for whom you want to post the delivery reminder.</span></span><br /><br /> <span data-ttu-id="2db4c-119">Quando si seleziona il numero fornitore, i campi **Nome**, **Indirizzo**, **NPA/Città** e **Contatto** vengono compilati automaticamente.</span><span class="sxs-lookup"><span data-stu-id="2db4c-119">When you select the vendor number, the **Name**, **Address**, **Post Code/City**, and **Contact** fields are filled in automatically.</span></span>|  
    |<span data-ttu-id="2db4c-120">**Data di Registrazione**</span><span class="sxs-lookup"><span data-stu-id="2db4c-120">**Posting Date**</span></span>|<span data-ttu-id="2db4c-121">Data di registrazione per il sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="2db4c-121">The posting date for the delivery reminder.</span></span> <span data-ttu-id="2db4c-122">Tale data viene copiata in tutti i movimenti contabili relativi al sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="2db4c-122">This date is copied to all of the delivery reminder ledger entries.</span></span>|  
    |<span data-ttu-id="2db4c-123">**Data Documento**</span><span class="sxs-lookup"><span data-stu-id="2db4c-123">**Document Date**</span></span>|<span data-ttu-id="2db4c-124">Data del documento per il sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="2db4c-124">The document date for the delivery reminder.</span></span> <span data-ttu-id="2db4c-125">Questa data è utilizzata anche per calcolare la data di scadenza per il sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="2db4c-125">This date is also used to calculate the due date for the delivery reminder.</span></span> <span data-ttu-id="2db4c-126">Se necessario, è possibile modificare la data di registrazione.</span><span class="sxs-lookup"><span data-stu-id="2db4c-126">You can modify the posting date if required.</span></span>|  
    |<span data-ttu-id="2db4c-127">**Livello di sollecito**</span><span class="sxs-lookup"><span data-stu-id="2db4c-127">**Reminder Level**</span></span>|<span data-ttu-id="2db4c-128">Livello del sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="2db4c-128">The delivery reminder level.</span></span> <span data-ttu-id="2db4c-129">Questo valore si basa sul numero di solleciti di consegna già inviati.</span><span class="sxs-lookup"><span data-stu-id="2db4c-129">This value is based on the number of delivery reminders that have already been sent.</span></span> <span data-ttu-id="2db4c-130">Per ulteriori informazioni, vedere [Impostare termini, livelli e testo dei solleciti di consegna](how-to-set-up-delivery-reminder-terms-levels-and-text.md).</span><span class="sxs-lookup"><span data-stu-id="2db4c-130">For more information, see [Set Up Delivery Reminder Terms, Levels, and Text](how-to-set-up-delivery-reminder-terms-levels-and-text.md).</span></span>|  
    |<span data-ttu-id="2db4c-131">**Cod. termini di sollecito**</span><span class="sxs-lookup"><span data-stu-id="2db4c-131">**Reminder Terms Code**</span></span>|<span data-ttu-id="2db4c-132">Specifica il codice dei termini del sollecito di consegna impostato per il fornitore.</span><span class="sxs-lookup"><span data-stu-id="2db4c-132">Specify the delivery reminder terms code that is set up for the vendor.</span></span>|  
    |<span data-ttu-id="2db4c-133">**Data scad.**</span><span class="sxs-lookup"><span data-stu-id="2db4c-133">**Due Date**</span></span>|<span data-ttu-id="2db4c-134">Data di scadenza per il sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="2db4c-134">The due date for the delivery reminder.</span></span>|  

4.  <span data-ttu-id="2db4c-135">Scegliere l'azione selezionare **Suggerisci riga sollecito**</span><span class="sxs-lookup"><span data-stu-id="2db4c-135">Choose the **Suggest Reminder Lines** action</span></span>  

    <span data-ttu-id="2db4c-136">Se per il fornitore specificato sono presenti consegne scadute, queste vengono aggiunte al sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="2db4c-136">If there are overdue deliveries from the specified vendor, these are added to the deliver reminder.</span></span>  

5.  <span data-ttu-id="2db4c-137">Scegliere il pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="2db4c-137">Choose the **OK** button.</span></span>  

    <span data-ttu-id="2db4c-138">Il sollecito di consegna viene creato.</span><span class="sxs-lookup"><span data-stu-id="2db4c-138">The delivery reminder is created.</span></span> <span data-ttu-id="2db4c-139">È ora possibile emettere e stampare il sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="2db4c-139">You can now issue and print the delivery reminder.</span></span>  

## <a name="see-also"></a><span data-ttu-id="2db4c-140">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="2db4c-140">See Also</span></span>  
 <span data-ttu-id="2db4c-141">[Solleciti consegna](delivery-reminders.md) </span><span class="sxs-lookup"><span data-stu-id="2db4c-141">[Delivery Reminders](delivery-reminders.md) </span></span>  
 <span data-ttu-id="2db4c-142">[Generare solleciti di consegna](how-to-generate-delivery-reminders.md) </span><span class="sxs-lookup"><span data-stu-id="2db4c-142">[Generate Delivery Reminders](how-to-generate-delivery-reminders.md) </span></span>  
 <span data-ttu-id="2db4c-143">[Impostare solleciti di consegna](how-to-set-up-delivery-reminders.md) </span><span class="sxs-lookup"><span data-stu-id="2db4c-143">[Set Up Delivery Reminders](how-to-set-up-delivery-reminders.md) </span></span>  
 <span data-ttu-id="2db4c-144">[Impostare i termini, i livelli e i testi di sollecito di consegna](how-to-set-up-delivery-reminder-terms-levels-and-text.md) </span><span class="sxs-lookup"><span data-stu-id="2db4c-144">[Set Up Delivery Reminder Terms, Levels, and Text](how-to-set-up-delivery-reminder-terms-levels-and-text.md) </span></span>  
 <span data-ttu-id="2db4c-145">[Assegnare codici di solleciti di consegna ai fornitori](how-to-assign-delivery-reminder-codes-to-vendors.md) </span><span class="sxs-lookup"><span data-stu-id="2db4c-145">[Assign Delivery Reminder Codes to Vendors](how-to-assign-delivery-reminder-codes-to-vendors.md) </span></span>  
 <span data-ttu-id="2db4c-146">[Emettere solleciti di consegna](how-to-issue-delivery-reminders.md) </span><span class="sxs-lookup"><span data-stu-id="2db4c-146">[Issue Delivery Reminders](how-to-issue-delivery-reminders.md) </span></span>  
 [<span data-ttu-id="2db4c-147">Stampare report di test per i solleciti di consegna</span><span class="sxs-lookup"><span data-stu-id="2db4c-147">Print Test Reports for Delivery Reminders</span></span>](how-to-print-test-reports-for-delivery-reminders.md)

