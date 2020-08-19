---
title: Come emettere solleciti di consegna nella versione svizzera
description: Dopo aver creato i solleciti di consegna, è necessario rilasciarli e stamparli in modo da poter inviare i solleciti ai fornitori. È possibile stampare un report di test prima di rilasciare i solleciti di consegna.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 07/23/2020
ms.author: sgroespe
ms.openlocfilehash: 38ba9e803f765ba08dd0d7424bdfe0fe9b10702f
ms.sourcegitcommit: 007b331b6974983ee614db0406f00777da359ecb
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 08/10/2020
ms.locfileid: "3677204"
---
# <a name="issue-delivery-reminders-in-the-swiss-version"></a><span data-ttu-id="4772a-104">Emettere solleciti di consegna nella versione svizzera</span><span class="sxs-lookup"><span data-stu-id="4772a-104">Issue Delivery Reminders in the Swiss Version</span></span>

<span data-ttu-id="4772a-105">Dopo aver creato i solleciti di consegna, è necessario rilasciarli e stamparli in modo da poter inviare i solleciti ai fornitori.</span><span class="sxs-lookup"><span data-stu-id="4772a-105">After you have created delivery reminders, you must issue and print them so that you can send reminders to vendors.</span></span> <span data-ttu-id="4772a-106">È possibile stampare un report di test prima di rilasciare i solleciti di consegna.</span><span class="sxs-lookup"><span data-stu-id="4772a-106">Before you issue the delivery reminders, you can print a test report.</span></span> <span data-ttu-id="4772a-107">Per ulteriori informazioni, vedere [Stampare report di test per i solleciti di consegna](how-to-print-test-reports-for-delivery-reminders.md).</span><span class="sxs-lookup"><span data-stu-id="4772a-107">For more information, see [Print Test Reports for Delivery Reminders](how-to-print-test-reports-for-delivery-reminders.md).</span></span>  

<span data-ttu-id="4772a-108">Quando si rilasciano i solleciti di consegna, vengono creati movimenti contabili sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="4772a-108">When you issue the delivery reminders, delivery reminder ledger entries are created.</span></span> <span data-ttu-id="4772a-109">È possibile visualizzare i movimenti contabili creati nella pagina **Movimenti contabili sollecito di consegna**.</span><span class="sxs-lookup"><span data-stu-id="4772a-109">You can view the created ledger entries on the **Deliv. Reminder Ledger Entries** page.</span></span>  

## <a name="to-issue-delivery-reminders"></a><span data-ttu-id="4772a-110">Per emettere solleciti di consegna</span><span class="sxs-lookup"><span data-stu-id="4772a-110">To issue delivery reminders</span></span>  

1.  <span data-ttu-id="4772a-111">Scegliere l'![icona a forma di lampadina che consente di aprire la funzionalità delle informazioni](../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Sollecito consegna** e quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="4772a-111">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Delivery Reminder**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="4772a-112">Nella pagina **Sollecito di consegna**, selezionare il sollecito di consegna da rilasciare quindi selezionare l'azione **Modifica**.</span><span class="sxs-lookup"><span data-stu-id="4772a-112">On the **Delivery Reminder** page, select the delivery reminder that you want to issue, and then choose the **Edit** action.</span></span>  
3.  <span data-ttu-id="4772a-113">Scegliere l'azione **Emetti**.</span><span class="sxs-lookup"><span data-stu-id="4772a-113">Choose the **Issue** action.</span></span>  
4.  <span data-ttu-id="4772a-114">Nella Scheda dettaglio **Opzioni** della pagina **Emettere sollecito di consegna** compilare i campi come descritto nella tabella seguente.</span><span class="sxs-lookup"><span data-stu-id="4772a-114">On the **Issue Delivery Reminder** page, on the **Options** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="4772a-115">Campo</span><span class="sxs-lookup"><span data-stu-id="4772a-115">Field</span></span>|<span data-ttu-id="4772a-116">Descrizione</span><span class="sxs-lookup"><span data-stu-id="4772a-116">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="4772a-117">**Stampa**</span><span class="sxs-lookup"><span data-stu-id="4772a-117">**Print**</span></span>|<span data-ttu-id="4772a-118">Selezionare la stampa dei solleciti di consegna quando vengono emessi.</span><span class="sxs-lookup"><span data-stu-id="4772a-118">Select to print the delivery reminders when they are issued.</span></span>|  
    |<span data-ttu-id="4772a-119">**Sostituisci data registrazione**</span><span class="sxs-lookup"><span data-stu-id="4772a-119">**Replace Posting Date**</span></span>|<span data-ttu-id="4772a-120">Selezionare la sostituzione della data di registrazione esistente per il sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="4772a-120">Select to replace the existing posting date for the delivery reminder.</span></span>|  
    |<span data-ttu-id="4772a-121">**Data di Registrazione**</span><span class="sxs-lookup"><span data-stu-id="4772a-121">**Posting Date**</span></span>|<span data-ttu-id="4772a-122">Data di registrazione per il sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="4772a-122">The posting date for the delivery reminder.</span></span><br /><br /> <span data-ttu-id="4772a-123">Questa data di registrazione viene utilizzata per tutti i solleciti di consegna se è stata selezionata la casella di controllo **Sostituisci data registrazione**.</span><span class="sxs-lookup"><span data-stu-id="4772a-123">This posting date is used for all delivery reminders if you have selected the **Replace Posting Date** check box.</span></span> <span data-ttu-id="4772a-124">Se la casella di controllo **Sostituisci data registrazione** è deselezionata, questa data verrà utilizzata solo per i solleciti di consegna per i quali una data di registrazione non è disponibile.</span><span class="sxs-lookup"><span data-stu-id="4772a-124">If the **Replace Posting Date** check box is cleared, this date will be used for only those delivery reminders for which a posting date is not available.</span></span>|  

5.  <span data-ttu-id="4772a-125">Facoltativamente, nella Scheda dettaglio **Intestazione sollecito di consegna** selezionare i filtri appropriati.</span><span class="sxs-lookup"><span data-stu-id="4772a-125">Optionally, on the **Delivery Reminder Header** FastTab, select the appropriate filters.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="4772a-126">È possibile rimuovere i filtri ed emettere contemporaneamente tutti i solleciti di consegna.</span><span class="sxs-lookup"><span data-stu-id="4772a-126">You can remove filters and issue all delivery reminders at the same time.</span></span>  

6.  <span data-ttu-id="4772a-127">Scegliere il pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="4772a-127">Choose the **OK** button.</span></span>  

<span data-ttu-id="4772a-128">È possibile visualizzare il solleciti di consegna nella pagina **Sollecito di consegna inviato**.</span><span class="sxs-lookup"><span data-stu-id="4772a-128">You can view the issued reminders on the **Issued Delivery Reminder** page.</span></span> <span data-ttu-id="4772a-129">Facoltativamente è possibile stampare un sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="4772a-129">Optionally, you can now print a delivery reminder.</span></span>  

## <a name="to-view-delivery-reminder-ledger-entries"></a><span data-ttu-id="4772a-130">Per visualizzare i movimenti contabili solleciti di consegna</span><span class="sxs-lookup"><span data-stu-id="4772a-130">To view delivery reminder ledger entries</span></span>  

1.  <span data-ttu-id="4772a-131">Scegliere l'![icona a forma di lampadina che consente di aprire la funzionalità delle informazioni](../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Ordini acquisto** e quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="4772a-131">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Orders**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="4772a-132">Selezionare l'ordine di acquisto per cui si desidera visualizzare lo stato del sollecito, quindi scegliere l'azione **Modifica**.</span><span class="sxs-lookup"><span data-stu-id="4772a-132">Select the purchase order for which you want to view the reminder status, and then choose the **Edit** action.</span></span>  
3.  <span data-ttu-id="4772a-133">Scegliere l'azione **Movimenti contabili sollecito di consegna**.</span><span class="sxs-lookup"><span data-stu-id="4772a-133">Choose the **Deliv. Reminder Ledger Entries** action.</span></span>  

<span data-ttu-id="4772a-134">Nella pagina Movimenti contabili sollecito di consegna, è possibile visualizzare i movimenti contabili sollecito di consegna per l'ordine di acquisto selezionato.</span><span class="sxs-lookup"><span data-stu-id="4772a-134">In the Deliv. Reminder Ledger Entries page, you can view the delivery reminder ledger entries for the selected purchase order.</span></span>  

## <a name="see-also"></a><span data-ttu-id="4772a-135">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="4772a-135">See Also</span></span>  
 <span data-ttu-id="4772a-136">[Solleciti consegna](delivery-reminders.md) </span><span class="sxs-lookup"><span data-stu-id="4772a-136">[Delivery Reminders](delivery-reminders.md) </span></span>  
 <span data-ttu-id="4772a-137">[Generare solleciti di consegna](how-to-generate-delivery-reminders.md) </span><span class="sxs-lookup"><span data-stu-id="4772a-137">[Generate Delivery Reminders](how-to-generate-delivery-reminders.md) </span></span>  
 [<span data-ttu-id="4772a-138">Creare solleciti di consegna manualmente</span><span class="sxs-lookup"><span data-stu-id="4772a-138">Create Delivery Reminders Manually</span></span>](how-to-create-delivery-reminders-manually.md)
