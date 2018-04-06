---
title: 'Procedura: Emettere solleciti di consegna'
description: "Dopo aver creato i solleciti di consegna, è necessario rilasciarli e stamparli in modo da poter inviare i solleciti ai fornitori. È possibile stampare un report di test prima di rilasciare i solleciti di consegna."
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
ms.openlocfilehash: 6abf8039442d60bcf379db823907ff24296b05cb
ms.contentlocale: it-ch
ms.lasthandoff: 03/22/2018

---
# <a name="issue-delivery-reminders"></a><span data-ttu-id="913c0-104">Emettere solleciti di consegna</span><span class="sxs-lookup"><span data-stu-id="913c0-104">Issue Delivery Reminders</span></span>
<span data-ttu-id="913c0-105">Dopo aver creato i solleciti di consegna, è necessario rilasciarli e stamparli in modo da poter inviare i solleciti ai fornitori.</span><span class="sxs-lookup"><span data-stu-id="913c0-105">After you have created delivery reminders, you must issue and print them so that you can send reminders to vendors.</span></span> <span data-ttu-id="913c0-106">È possibile stampare un report di test prima di rilasciare i solleciti di consegna.</span><span class="sxs-lookup"><span data-stu-id="913c0-106">Before you issue the delivery reminders, you can print a test report.</span></span> <span data-ttu-id="913c0-107">Per ulteriori informazioni, vedere [Stampare report di test per i solleciti di consegna](how-to-print-test-reports-for-delivery-reminders.md).</span><span class="sxs-lookup"><span data-stu-id="913c0-107">For more information, see [Print Test Reports for Delivery Reminders](how-to-print-test-reports-for-delivery-reminders.md).</span></span>  

<span data-ttu-id="913c0-108">Quando si rilasciano i solleciti di consegna, vengono creati movimenti contabili sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="913c0-108">When you issue the delivery reminders, delivery reminder ledger entries are created.</span></span> <span data-ttu-id="913c0-109">È possibile visualizzare i movimenti contabili creati nella finestra **Movimenti contabili sollecito di consegna**.</span><span class="sxs-lookup"><span data-stu-id="913c0-109">You can view the created ledger entries in the **Deliv. Reminder Ledger Entries** window.</span></span>  

## <a name="to-issue-delivery-reminders"></a><span data-ttu-id="913c0-110">Per emettere solleciti di consegna</span><span class="sxs-lookup"><span data-stu-id="913c0-110">To issue delivery reminders</span></span>  

1.  <span data-ttu-id="913c0-111">Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Sollecito di consegna**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="913c0-111">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Delivery Reminder**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="913c0-112">Nella finestra **Sollecito di consegna**, selezionare il sollecito di consegna da rilasciare quindi selezionare l'azione **Modifica**.</span><span class="sxs-lookup"><span data-stu-id="913c0-112">In the **Delivery Reminder** window, select the delivery reminder that you want to issue, and then choose the **Edit** action.</span></span>  
3.  <span data-ttu-id="913c0-113">Scegliere l'azione **Emetti**.</span><span class="sxs-lookup"><span data-stu-id="913c0-113">Choose the **Issue** action.</span></span>  
4.  <span data-ttu-id="913c0-114">Nella Scheda dettaglio **Opzioni** della finestra **Emettere sollecito di consegna** compilare i campi come descritto nella tabella seguente.</span><span class="sxs-lookup"><span data-stu-id="913c0-114">In the **Issue Delivery Reminder** window, on the **Options** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="913c0-115">Campo</span><span class="sxs-lookup"><span data-stu-id="913c0-115">Field</span></span>|<span data-ttu-id="913c0-116">Descrizione</span><span class="sxs-lookup"><span data-stu-id="913c0-116">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="913c0-117">**Stampa**</span><span class="sxs-lookup"><span data-stu-id="913c0-117">**Print**</span></span>|<span data-ttu-id="913c0-118">Selezionare la stampa dei solleciti di consegna quando vengono emessi.</span><span class="sxs-lookup"><span data-stu-id="913c0-118">Select to print the delivery reminders when they are issued.</span></span>|  
    |<span data-ttu-id="913c0-119">**Sostituisci data registrazione**</span><span class="sxs-lookup"><span data-stu-id="913c0-119">**Replace Posting Date**</span></span>|<span data-ttu-id="913c0-120">Selezionare la sostituzione della data di registrazione esistente per il sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="913c0-120">Select to replace the existing posting date for the delivery reminder.</span></span>|  
    |<span data-ttu-id="913c0-121">**Data di Registrazione**</span><span class="sxs-lookup"><span data-stu-id="913c0-121">**Posting Date**</span></span>|<span data-ttu-id="913c0-122">Data di registrazione per il sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="913c0-122">The posting date for the delivery reminder.</span></span><br /><br /> <span data-ttu-id="913c0-123">Questa data di registrazione viene utilizzata per tutti i solleciti di consegna se è stata selezionata la casella di controllo **Sostituisci data registrazione**.</span><span class="sxs-lookup"><span data-stu-id="913c0-123">This posting date is used for all delivery reminders if you have selected the **Replace Posting Date** check box.</span></span> <span data-ttu-id="913c0-124">Se la casella di controllo **Sostituisci data registrazione** è deselezionata, questa data verrà utilizzata solo per i solleciti di consegna per i quali una data di registrazione non è disponibile.</span><span class="sxs-lookup"><span data-stu-id="913c0-124">If the **Replace Posting Date** check box is cleared, this date will be used for only those delivery reminders for which a posting date is not available.</span></span>|  

5.  <span data-ttu-id="913c0-125">Facoltativamente, nella Scheda dettaglio **Intestazione sollecito di consegna** selezionare i filtri appropriati.</span><span class="sxs-lookup"><span data-stu-id="913c0-125">Optionally, on the **Delivery Reminder Header** FastTab, select the appropriate filters.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="913c0-126">È possibile rimuovere i filtri ed emettere contemporaneamente tutti i solleciti di consegna.</span><span class="sxs-lookup"><span data-stu-id="913c0-126">You can remove filters and issue all delivery reminders at the same time.</span></span>  

6.  <span data-ttu-id="913c0-127">Scegliere il pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="913c0-127">Choose the **OK** button.</span></span>  

<span data-ttu-id="913c0-128">È possibile visualizzare il solleciti di consegna nella finestra **Sollecito di consegna inviato**.</span><span class="sxs-lookup"><span data-stu-id="913c0-128">You can view the issued reminders in the **Issued Delivery Reminder** window.</span></span> <span data-ttu-id="913c0-129">Facoltativamente è possibile stampare un sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="913c0-129">Optionally, you can now print a delivery reminder.</span></span>  

## <a name="to-view-delivery-reminder-ledger-entries"></a><span data-ttu-id="913c0-130">Per visualizzare i movimenti contabili solleciti di consegna</span><span class="sxs-lookup"><span data-stu-id="913c0-130">To view delivery reminder ledger entries</span></span>  

1.  <span data-ttu-id="913c0-131">Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "Cerca pagina o report"), immettere **Ordini acquisto**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="913c0-131">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchase Orders**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="913c0-132">Selezionare l'ordine di acquisto per cui si desidera visualizzare lo stato del sollecito, quindi scegliere l'azione **Modifica**.</span><span class="sxs-lookup"><span data-stu-id="913c0-132">Select the purchase order for which you want to view the reminder status, and then choose the **Edit** action.</span></span>  
3.  <span data-ttu-id="913c0-133">Scegliere l'azione **Movimenti contabili sollecito di consegna**.</span><span class="sxs-lookup"><span data-stu-id="913c0-133">Choose the **Deliv. Reminder Ledger Entries** action.</span></span>  

<span data-ttu-id="913c0-134">Nella finestra Movimenti contabili sollecito di consegna, è possibile visualizzare i movimenti contabili sollecito di consegna per l'ordine di acquisto selezionato.</span><span class="sxs-lookup"><span data-stu-id="913c0-134">In the Deliv. Reminder Ledger Entries window, you can view the delivery reminder ledger entries for the selected purchase order.</span></span>  

## <a name="see-also"></a><span data-ttu-id="913c0-135">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="913c0-135">See Also</span></span>  
 <span data-ttu-id="913c0-136">[Solleciti consegna](delivery-reminders.md) </span><span class="sxs-lookup"><span data-stu-id="913c0-136">[Delivery Reminders](delivery-reminders.md) </span></span>  
 <span data-ttu-id="913c0-137">[Generare solleciti di consegna](how-to-generate-delivery-reminders.md) </span><span class="sxs-lookup"><span data-stu-id="913c0-137">[Generate Delivery Reminders](how-to-generate-delivery-reminders.md) </span></span>  
 [<span data-ttu-id="913c0-138">Creare solleciti di consegna manualmente</span><span class="sxs-lookup"><span data-stu-id="913c0-138">Create Delivery Reminders Manually</span></span>](how-to-create-delivery-reminders-manually.md)

