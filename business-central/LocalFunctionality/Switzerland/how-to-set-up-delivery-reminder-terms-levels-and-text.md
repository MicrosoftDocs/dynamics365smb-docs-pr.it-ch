---
title: 'Procedura: Impostare termini, livelli e testo dei solleciti di consegna'
description: Per creare i solleciti di consegna, è necessario impostare i termini, i livelli e i testi dei solleciti di consegna. messaggi
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
ms.openlocfilehash: 5d24b0ac49fe227c5f39c8d880463c302c37cc63
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 04/29/2019
ms.locfileid: "1241270"
---
# <a name="set-up-delivery-reminder-terms-levels-and-text"></a><span data-ttu-id="63795-104">Impostare i termini, i livelli e i testi di sollecito di consegna</span><span class="sxs-lookup"><span data-stu-id="63795-104">Set Up Delivery Reminder Terms, Levels, and Text</span></span>
<span data-ttu-id="63795-105">Per creare i solleciti di consegna è necessario impostare quanto segue:</span><span class="sxs-lookup"><span data-stu-id="63795-105">To create delivery reminders, you must set up the following:</span></span>  

- <span data-ttu-id="63795-106">Termini di sollecito di consegna</span><span class="sxs-lookup"><span data-stu-id="63795-106">Delivery reminder terms</span></span>  
- <span data-ttu-id="63795-107">Livelli del sollecito di consegna</span><span class="sxs-lookup"><span data-stu-id="63795-107">Delivery reminder levels</span></span>  
- <span data-ttu-id="63795-108">Messaggi di testo di sollecito di consegna</span><span class="sxs-lookup"><span data-stu-id="63795-108">Delivery reminder text messages</span></span>  

<span data-ttu-id="63795-109">Ogni termine di sollecito di consegna ha due o più livelli di sollecito di consegna e per ogni livello di sollecito di consegna è possibile specificare il testo che fa parte del sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="63795-109">Each delivery reminder term has two or more delivery reminder levels, and for each delivery reminder level, you can specify text that will be part of the delivery reminder.</span></span>  

<span data-ttu-id="63795-110">Per ulteriori informazioni, vedere [Solleciti di consegna](delivery-reminders.md).</span><span class="sxs-lookup"><span data-stu-id="63795-110">For more information, see [Delivery Reminders](delivery-reminders.md).</span></span>  

## <a name="to-set-up-delivery-reminder-terms"></a><span data-ttu-id="63795-111">Per impostare i termini di sollecito di consegna</span><span class="sxs-lookup"><span data-stu-id="63795-111">To set up delivery reminder terms</span></span>  

1.  <span data-ttu-id="63795-112">Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Termini di sollecito di consegna**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="63795-112">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Delivery Reminder Terms**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="63795-113">Scegliere l'azione **Nuovo**.</span><span class="sxs-lookup"><span data-stu-id="63795-113">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="63795-114">Compilare i campi come indicato nella tabella seguente.</span><span class="sxs-lookup"><span data-stu-id="63795-114">Fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="63795-115">Campo</span><span class="sxs-lookup"><span data-stu-id="63795-115">Field</span></span>|<span data-ttu-id="63795-116">Descrizione</span><span class="sxs-lookup"><span data-stu-id="63795-116">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="63795-117">**Codice**</span><span class="sxs-lookup"><span data-stu-id="63795-117">**Code**</span></span>|<span data-ttu-id="63795-118">Codice per i termini di sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="63795-118">The code for the delivery reminder term.</span></span> <span data-ttu-id="63795-119">È possibile immettere un massimo di 10 caratteri alfanumerici.</span><span class="sxs-lookup"><span data-stu-id="63795-119">You can enter a maximum of 10 alphanumeric characters.</span></span>|  
    |<span data-ttu-id="63795-120">**Descrizione**</span><span class="sxs-lookup"><span data-stu-id="63795-120">**Description**</span></span>|<span data-ttu-id="63795-121">Descrizione per i termini di sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="63795-121">The description for the delivery reminder term.</span></span> <span data-ttu-id="63795-122">È possibile immettere un massimo di 30 caratteri alfanumerici.</span><span class="sxs-lookup"><span data-stu-id="63795-122">You can enter a maximum of 30 alphanumeric characters.</span></span>|  
    |<span data-ttu-id="63795-123">**Nr. Max di Solleciti Consegna**</span><span class="sxs-lookup"><span data-stu-id="63795-123">**Max. No. of Delivery Reminders**</span></span>|<span data-ttu-id="63795-124">Numero massimo di solleciti di consegna che è possibile creare per un ordine.</span><span class="sxs-lookup"><span data-stu-id="63795-124">The maximum number of delivery reminders that can be created for an order.</span></span><br /><br /> <span data-ttu-id="63795-125">**NOTA:** questo è il numero massimo per tutti i livelli di sollecito per questo termine di sollecito.</span><span class="sxs-lookup"><span data-stu-id="63795-125">**NOTE:** This is the maximum number across all reminder levels for this reminder term.</span></span> <span data-ttu-id="63795-126">Ad esempio, se si impostano tre livelli e si imposta **Numero massimo di solleciti di consegna** su 5, il primo sollecito viene creato al livello 1, il secondo al livello 2 e gli ultimi tre al livello 3.</span><span class="sxs-lookup"><span data-stu-id="63795-126">For example, if you have set up three levels, and you set **Max. No. of Delivery Reminders** to 5, the first reminder is created at level 1, the second at level 2, and the last three at level 3.</span></span>|  

4.  <span data-ttu-id="63795-127">Scegliere il pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="63795-127">Choose the **OK** button.</span></span>  

## <a name="to-add-delivery-reminder-levels-to-a-delivery-reminder-term"></a><span data-ttu-id="63795-128">Per aggiungere livelli di sollecito di consegna a un termine di sollecito di consegna</span><span class="sxs-lookup"><span data-stu-id="63795-128">To add delivery reminder levels to a delivery reminder term</span></span>  

1.  <span data-ttu-id="63795-129">Nella pagina **Termini di sollecito di consegna** selezionare il termine di sollecito di consegna per cui si desidera impostare i livelli e scegliere l'azione **Livelli**.</span><span class="sxs-lookup"><span data-stu-id="63795-129">On the **Delivery Reminder Terms** page, select the delivery reminder term for which you want to set up levels, and then choose the **Levels** action.</span></span>  
2.  <span data-ttu-id="63795-130">Scegliere l'azione **Nuovo**.</span><span class="sxs-lookup"><span data-stu-id="63795-130">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="63795-131">Compilare i campi come indicato nella tabella seguente.</span><span class="sxs-lookup"><span data-stu-id="63795-131">Fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="63795-132">Campo</span><span class="sxs-lookup"><span data-stu-id="63795-132">Field</span></span>|<span data-ttu-id="63795-133">Descrizione</span><span class="sxs-lookup"><span data-stu-id="63795-133">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="63795-134">**Nr.**</span><span class="sxs-lookup"><span data-stu-id="63795-134">**No.**</span></span>|<span data-ttu-id="63795-135">Numero del livello del sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="63795-135">The delivery reminder level number.</span></span> <span data-ttu-id="63795-136">Questo campo viene compilato automaticamente.</span><span class="sxs-lookup"><span data-stu-id="63795-136">This field is filled in automatically.</span></span>|  
    |<span data-ttu-id="63795-137">**Calcolo data di scadenza**</span><span class="sxs-lookup"><span data-stu-id="63795-137">**Due Date Calculation**</span></span>|<span data-ttu-id="63795-138">Formula per il calcolo della data di scadenza per il sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="63795-138">The formula for the due date calculation for the delivery reminder.</span></span> <span data-ttu-id="63795-139">È possibile immettere una combinazione di numeri da 0 a 9999 e codici di data (G per giorno, GS per il giorno della settimana, S per settimana, M per mese, T per trimestre o A per anno).</span><span class="sxs-lookup"><span data-stu-id="63795-139">You can enter a combination of numbers from 0 to 9999, and date codes (D for day, WD for weekday, W for week, M for month, Q for quarter, or Y for year).</span></span> <span data-ttu-id="63795-140">I codici di data indicano il calcolo della data di scadenza per il sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="63795-140">The date codes denote the calculation for the delivery reminder due date.</span></span> <span data-ttu-id="63795-141">È possibile inserire un massimo di 20 caratteri per la formula di calcolo della data di scadenza.</span><span class="sxs-lookup"><span data-stu-id="63795-141">You can enter a maximum of 20 characters for the due date calculation formula.</span></span>|  

4.  <span data-ttu-id="63795-142">Scegliere il pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="63795-142">Choose the **OK** button.</span></span>  

<span data-ttu-id="63795-143">Per ciascun livello di sollecito di consegna è possibile definire messaggi di testo che vengono aggiunti al sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="63795-143">For each delivery reminder level, you can define text messages that are added to the delivery reminder.</span></span> <span data-ttu-id="63795-144">Definire il testo iniziale che viene aggiunto prima della descrizione dell'ordine di acquisto scaduto e il testo finale che viene aggiunto dopo la descrizione dell'ordine di acquisto scaduto.</span><span class="sxs-lookup"><span data-stu-id="63795-144">You can define beginning text that is added before the description of the overdue purchase order, and ending text that is added after the description of the overdue purchase order.</span></span>  

<span data-ttu-id="63795-145">La procedura seguente descrive come impostare i messaggi di testo iniziali, ma gli stessi passaggi si applicano per impostare i messaggi di testo finali.</span><span class="sxs-lookup"><span data-stu-id="63795-145">The following procedure describes how to set up beginning text messages, but the same steps apply for setting up ending text messages.</span></span>  

## <a name="to-set-up-delivery-reminder-text-messages"></a><span data-ttu-id="63795-146">Per impostare i messaggi di testo di sollecito di consegna</span><span class="sxs-lookup"><span data-stu-id="63795-146">To set up delivery reminder text messages</span></span>  

1.  <span data-ttu-id="63795-147">Nella pagina **Livelli del sollecito di consegna** selezionare un livello e scegliere l'azione **Testo iniziale**.</span><span class="sxs-lookup"><span data-stu-id="63795-147">On the **Delivery Reminder Levels** page, select a level, and then choose the **Beginning Text** action.</span></span>  
2.  <span data-ttu-id="63795-148">Scegliere l'azione **Nuovo**.</span><span class="sxs-lookup"><span data-stu-id="63795-148">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="63795-149">Nel campo **Descrizione** inserire il messaggio di testo iniziale per il sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="63795-149">In the **Description** field, enter the beginning text message for the delivery reminder.</span></span>  
4.  <span data-ttu-id="63795-150">Scegliere il pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="63795-150">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="63795-151">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="63795-151">See Also</span></span>  
 <span data-ttu-id="63795-152">[Solleciti consegna](delivery-reminders.md) </span><span class="sxs-lookup"><span data-stu-id="63795-152">[Delivery Reminders](delivery-reminders.md) </span></span>  
 <span data-ttu-id="63795-153">[Impostare solleciti di consegna](how-to-set-up-delivery-reminders.md) </span><span class="sxs-lookup"><span data-stu-id="63795-153">[Set Up Delivery Reminders](how-to-set-up-delivery-reminders.md) </span></span>  
 <span data-ttu-id="63795-154">[Assegnare codici di solleciti di consegna ai fornitori](how-to-assign-delivery-reminder-codes-to-vendors.md) </span><span class="sxs-lookup"><span data-stu-id="63795-154">[Assign Delivery Reminder Codes to Vendors](how-to-assign-delivery-reminder-codes-to-vendors.md) </span></span>  
 <span data-ttu-id="63795-155">[Creare solleciti di consegna manualmente](how-to-create-delivery-reminders-manually.md) </span><span class="sxs-lookup"><span data-stu-id="63795-155">[Create Delivery Reminders Manually](how-to-create-delivery-reminders-manually.md) </span></span>  
 [<span data-ttu-id="63795-156">Emettere solleciti di consegna</span><span class="sxs-lookup"><span data-stu-id="63795-156">Issue Delivery Reminders</span></span>](how-to-issue-delivery-reminders.md)
