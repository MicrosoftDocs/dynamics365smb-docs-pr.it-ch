---
author: edupont04
ms.service: dynamics365-business-central
ms.topic: include
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 923162f06045d13e37c80d31c27c8771eccf2f04
ms.sourcegitcommit: 428f180604e5afcf94fa0e92a0615f58c88e13cd
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 10/02/2020
ms.locfileid: "3959658"
---
<span data-ttu-id="40c31-101">In [!INCLUDE[d365fin](../../../includes/d365fin_md.md)], è possibile creare solleciti di consegna quando un acquisto non è stato consegnato come previsto.</span><span class="sxs-lookup"><span data-stu-id="40c31-101">In [!INCLUDE[d365fin](../../../includes/d365fin_md.md)], you can create delivery reminders when a purchase has not been delivered as expected.</span></span> <span data-ttu-id="40c31-102">È possibile creare un singolo sollecito di consegna manualmente o generare solleciti di consegna per tutte le consegne scadute.</span><span class="sxs-lookup"><span data-stu-id="40c31-102">You can create a single delivery reminder manually, or you can generate delivery reminders for all overdue deliveries.</span></span>  

> [!NOTE]
> <span data-ttu-id="40c31-103">Per creare solleciti di consegna, è necessario impostare i testi, i livelli e i termini del sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="40c31-103">To create delivery reminders, you must have set up the delivery reminder terms, levels, and texts.</span></span>

## <a name="to-create-a-delivery-reminder-manually"></a><span data-ttu-id="40c31-104">Per creare un sollecito di consegna manualmente</span><span class="sxs-lookup"><span data-stu-id="40c31-104">To create a delivery reminder manually</span></span>  

1. <span data-ttu-id="40c31-105">Scegliere l'icona ![L'icona a forma di lampadina che consente di aprire la funzionalità delle informazioni](../../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Sollecito consegna** e quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="40c31-105">Choose the ![The lightbulb icon that opens the Tell Me feature](../../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Delivery Reminder**, and then choose the related link.</span></span>  
2. <span data-ttu-id="40c31-106">Scegliere l'azione **Nuovo**.</span><span class="sxs-lookup"><span data-stu-id="40c31-106">Choose the **New** action.</span></span>  
3. <span data-ttu-id="40c31-107">Nella pagina **Sollecito di consegna**, compilare i campi come indicato nella tabella riportata di seguito.</span><span class="sxs-lookup"><span data-stu-id="40c31-107">On the **Delivery Reminder** page, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="40c31-108">Campo</span><span class="sxs-lookup"><span data-stu-id="40c31-108">Field</span></span>|<span data-ttu-id="40c31-109">Descrizione</span><span class="sxs-lookup"><span data-stu-id="40c31-109">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="40c31-110">**Nr.**</span><span class="sxs-lookup"><span data-stu-id="40c31-110">**No.**</span></span>|<span data-ttu-id="40c31-111">Numero di identificazione univoco del sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="40c31-111">The unique identification number for the delivery reminder.</span></span>|  
    |<span data-ttu-id="40c31-112">**N. fornitore**</span><span class="sxs-lookup"><span data-stu-id="40c31-112">**Vendor No.**</span></span>|<span data-ttu-id="40c31-113">Numero del fornitore per cui si desidera registrare il sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="40c31-113">The number of the vendor for whom you want to post the delivery reminder.</span></span><br /><br /> <span data-ttu-id="40c31-114">Quando si seleziona il numero fornitore, i campi **Nome**, **Indirizzo**, **NPA/Città** e **Contatto** vengono compilati automaticamente.</span><span class="sxs-lookup"><span data-stu-id="40c31-114">When you select the vendor number, the **Name**, **Address**, **Post Code/City**, and **Contact** fields are filled in automatically.</span></span>|  
    |<span data-ttu-id="40c31-115">**Data di Registrazione**</span><span class="sxs-lookup"><span data-stu-id="40c31-115">**Posting Date**</span></span>|<span data-ttu-id="40c31-116">Data di registrazione per il sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="40c31-116">The posting date for the delivery reminder.</span></span> <span data-ttu-id="40c31-117">Tale data viene copiata in tutti i movimenti contabili relativi al sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="40c31-117">This date is copied to all of the delivery reminder ledger entries.</span></span>|  
    |<span data-ttu-id="40c31-118">**Data Documento**</span><span class="sxs-lookup"><span data-stu-id="40c31-118">**Document Date**</span></span>|<span data-ttu-id="40c31-119">Data del documento per il sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="40c31-119">The document date for the delivery reminder.</span></span> <span data-ttu-id="40c31-120">Questa data è utilizzata anche per calcolare la data di scadenza per il sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="40c31-120">This date is also used to calculate the due date for the delivery reminder.</span></span> <span data-ttu-id="40c31-121">Se necessario, è possibile modificare la data di registrazione.</span><span class="sxs-lookup"><span data-stu-id="40c31-121">You can modify the posting date if required.</span></span>|  
    |<span data-ttu-id="40c31-122">**Livello di sollecito**</span><span class="sxs-lookup"><span data-stu-id="40c31-122">**Reminder Level**</span></span>|<span data-ttu-id="40c31-123">Livello del sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="40c31-123">The delivery reminder level.</span></span> <span data-ttu-id="40c31-124">Questo valore si basa sul numero di solleciti di consegna già inviati.</span><span class="sxs-lookup"><span data-stu-id="40c31-124">This value is based on the number of delivery reminders that have already been sent.</span></span>|  
    |<span data-ttu-id="40c31-125">**Cod. termini di sollecito**</span><span class="sxs-lookup"><span data-stu-id="40c31-125">**Reminder Terms Code**</span></span>|<span data-ttu-id="40c31-126">Specifica il codice dei termini del sollecito di consegna impostato per il fornitore.</span><span class="sxs-lookup"><span data-stu-id="40c31-126">Specify the delivery reminder terms code that is set up for the vendor.</span></span>|  
    |<span data-ttu-id="40c31-127">**Data scad.**</span><span class="sxs-lookup"><span data-stu-id="40c31-127">**Due Date**</span></span>|<span data-ttu-id="40c31-128">Data di scadenza per il sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="40c31-128">The due date for the delivery reminder.</span></span>|  

4. <span data-ttu-id="40c31-129">Scegliere l'azione selezionare **Suggerisci riga sollecito**.</span><span class="sxs-lookup"><span data-stu-id="40c31-129">Choose the **Suggest Reminder Lines** action.</span></span>  

    <span data-ttu-id="40c31-130">Se per il fornitore specificato sono presenti consegne scadute, queste vengono aggiunte al sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="40c31-130">If there are overdue deliveries from the specified vendor, these are added to the delivery reminder.</span></span>  

5. <span data-ttu-id="40c31-131">Scegliere il pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="40c31-131">Choose the **OK** button.</span></span>  

    <span data-ttu-id="40c31-132">Il sollecito di consegna viene creato.</span><span class="sxs-lookup"><span data-stu-id="40c31-132">The delivery reminder is created.</span></span> <span data-ttu-id="40c31-133">È ora possibile emettere e stampare il sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="40c31-133">You can now issue and print the delivery reminder.</span></span>  
