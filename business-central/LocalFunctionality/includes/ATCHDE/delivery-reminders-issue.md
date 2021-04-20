---
author: edupont04
ms.service: dynamics365-business-central
ms.topic: include
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 7cab5533c038dda6082a0455bf480779f143854e
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 03/31/2021
ms.locfileid: "5777577"
---
<span data-ttu-id="894e4-101">Dopo aver creato i solleciti di consegna, è necessario rilasciarli e stamparli in modo da poter inviare i solleciti ai fornitori.</span><span class="sxs-lookup"><span data-stu-id="894e4-101">After you have created delivery reminders, you must issue and print them so that you can send reminders to vendors.</span></span> <span data-ttu-id="894e4-102">È possibile stampare un report di test prima di rilasciare i solleciti di consegna.</span><span class="sxs-lookup"><span data-stu-id="894e4-102">Before you issue the delivery reminders, you can print a test report.</span></span>  

<span data-ttu-id="894e4-103">Quando si rilasciano i solleciti di consegna, vengono creati movimenti contabili sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="894e4-103">When you issue the delivery reminders, delivery reminder ledger entries are created.</span></span> <span data-ttu-id="894e4-104">È possibile visualizzare i movimenti contabili creati nella pagina **Movimenti contabili sollecito di consegna**.</span><span class="sxs-lookup"><span data-stu-id="894e4-104">You can view the created ledger entries on the **Deliv. Reminder Ledger Entries** page.</span></span>  

## <a name="to-issue-delivery-reminders"></a><span data-ttu-id="894e4-105">Per emettere solleciti di consegna</span><span class="sxs-lookup"><span data-stu-id="894e4-105">To issue delivery reminders</span></span>  

1. <span data-ttu-id="894e4-106">Scegliere l'![icona a forma di lampadina che consente di aprire la funzionalità delle informazioni](../../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Sollecito consegna** e quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="894e4-106">Choose the ![Lightbulb that opens the Tell Me feature](../../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Delivery Reminder**, and then choose the related link.</span></span>  
2. <span data-ttu-id="894e4-107">Nella pagina **Sollecito di consegna**, selezionare il sollecito di consegna da rilasciare quindi selezionare l'azione **Modifica**.</span><span class="sxs-lookup"><span data-stu-id="894e4-107">On the **Delivery Reminder** page, select the delivery reminder that you want to issue, and then choose the **Edit** action.</span></span>  
3. <span data-ttu-id="894e4-108">Scegliere l'azione **Emetti**.</span><span class="sxs-lookup"><span data-stu-id="894e4-108">Choose the **Issue** action.</span></span>  
4. <span data-ttu-id="894e4-109">Nella pagina **Emettere sollecito di consegna**, compilare i campi come indicato nella tabella riportata di seguito.</span><span class="sxs-lookup"><span data-stu-id="894e4-109">On the **Issue Delivery Reminder** page, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="894e4-110">Campo</span><span class="sxs-lookup"><span data-stu-id="894e4-110">Field</span></span>|<span data-ttu-id="894e4-111">Descrizione</span><span class="sxs-lookup"><span data-stu-id="894e4-111">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="894e4-112">**Stampa**</span><span class="sxs-lookup"><span data-stu-id="894e4-112">**Print**</span></span>|<span data-ttu-id="894e4-113">Selezionare la stampa dei solleciti di consegna quando vengono emessi.</span><span class="sxs-lookup"><span data-stu-id="894e4-113">Select to print the delivery reminders when they are issued.</span></span>|  
    |<span data-ttu-id="894e4-114">**Sostituisci data registrazione**</span><span class="sxs-lookup"><span data-stu-id="894e4-114">**Replace Posting Date**</span></span>|<span data-ttu-id="894e4-115">Selezionare la sostituzione della data di registrazione esistente per il sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="894e4-115">Select to replace the existing posting date for the delivery reminder.</span></span>|  
    |<span data-ttu-id="894e4-116">**Data di Registrazione**</span><span class="sxs-lookup"><span data-stu-id="894e4-116">**Posting Date**</span></span>|<span data-ttu-id="894e4-117">Data di registrazione per il sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="894e4-117">The posting date for the delivery reminder.</span></span><br /><br /> <span data-ttu-id="894e4-118">Questa data di registrazione viene utilizzata per tutti i solleciti di consegna se è stata selezionata la casella di controllo **Sostituisci data registrazione**.</span><span class="sxs-lookup"><span data-stu-id="894e4-118">This posting date is used for all delivery reminders if you have selected the **Replace Posting Date** check box.</span></span> <span data-ttu-id="894e4-119">Se la casella di controllo **Sostituisci data registrazione** è deselezionata, questa data verrà utilizzata solo per i solleciti di consegna per i quali una data di registrazione non è disponibile.</span><span class="sxs-lookup"><span data-stu-id="894e4-119">If the **Replace Posting Date** check box is cleared, this date will be used for only those delivery reminders for which a posting date is not available.</span></span>|  

5. <span data-ttu-id="894e4-120">Facoltativamente, nella Scheda dettaglio **Intestazione sollecito di consegna** selezionare i filtri appropriati.</span><span class="sxs-lookup"><span data-stu-id="894e4-120">Optionally, on the **Delivery Reminder Header** FastTab, select the appropriate filters.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="894e4-121">È possibile rimuovere i filtri ed emettere contemporaneamente tutti i solleciti di consegna.</span><span class="sxs-lookup"><span data-stu-id="894e4-121">You can remove filters and issue all delivery reminders at the same time.</span></span>  

6. <span data-ttu-id="894e4-122">Scegliere il pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="894e4-122">Choose the **OK** button.</span></span>  

<span data-ttu-id="894e4-123">È possibile visualizzare il solleciti di consegna nella pagina **Sollecito di consegna inviato**.</span><span class="sxs-lookup"><span data-stu-id="894e4-123">You can view the issued reminders on the **Issued Delivery Reminder** page.</span></span> <span data-ttu-id="894e4-124">Facoltativamente è possibile stampare un sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="894e4-124">Optionally, you can now print a delivery reminder.</span></span>  

## <a name="to-view-delivery-reminder-ledger-entries"></a><span data-ttu-id="894e4-125">Per visualizzare i movimenti contabili solleciti di consegna</span><span class="sxs-lookup"><span data-stu-id="894e4-125">To view delivery reminder ledger entries</span></span>  

1. <span data-ttu-id="894e4-126">Scegliere l'![icona a forma di lampadina che consente di aprire la funzionalità delle informazioni](../../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Ordini acquisto** e quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="894e4-126">Choose the ![Lightbulb that opens the Tell Me feature](../../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Orders**, and then choose the related link.</span></span>  
2. <span data-ttu-id="894e4-127">Selezionare l'ordine di acquisto per cui si desidera visualizzare lo stato del sollecito, quindi scegliere l'azione **Modifica**.</span><span class="sxs-lookup"><span data-stu-id="894e4-127">Select the purchase order for which you want to view the reminder status, and then choose the **Edit** action.</span></span>  
3. <span data-ttu-id="894e4-128">Scegliere l'azione **Movimenti contabili sollecito di consegna**.</span><span class="sxs-lookup"><span data-stu-id="894e4-128">Choose the **Deliv. Reminder Ledger Entries** action.</span></span>  

<span data-ttu-id="894e4-129">Nella pagina **Movimenti contabili sollecito di consegna**, è possibile visualizzare i movimenti contabili sollecito di consegna per l'ordine di acquisto selezionato.</span><span class="sxs-lookup"><span data-stu-id="894e4-129">On the **Deliv. Reminder Ledger Entries** page, you can view the delivery reminder ledger entries for the selected purchase order.</span></span>  
