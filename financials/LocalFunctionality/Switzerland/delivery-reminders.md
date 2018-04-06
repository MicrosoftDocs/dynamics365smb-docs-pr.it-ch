---
title: Solleciti consegna
description: I solleciti di consegna sono usati per tracciare le consegne scadute dei fornitori e per segnalare ai fornitori le consegne scadute.
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
ms.openlocfilehash: 24b3525a5bd39298dd874657f7d7940e8ecd8cfb
ms.contentlocale: it-ch
ms.lasthandoff: 03/22/2018

---
# <a name="delivery-reminders"></a><span data-ttu-id="cf19d-103">Solleciti consegna</span><span class="sxs-lookup"><span data-stu-id="cf19d-103">Delivery Reminders</span></span>
<span data-ttu-id="cf19d-104">I solleciti di consegna sono usati per tracciare le consegne scadute dei fornitori e per segnalare ai fornitori le consegne scadute.</span><span class="sxs-lookup"><span data-stu-id="cf19d-104">Delivery reminders are used to track overdue vendor shipments, and to remind vendors about overdue deliveries.</span></span> <span data-ttu-id="cf19d-105">Per creare i solleciti di consegna è necessario impostare quanto segue:</span><span class="sxs-lookup"><span data-stu-id="cf19d-105">To create delivery reminders, you must set up the following:</span></span>  

- <span data-ttu-id="cf19d-106">Termini di sollecito di consegna</span><span class="sxs-lookup"><span data-stu-id="cf19d-106">Delivery reminder terms</span></span>  

    <span data-ttu-id="cf19d-107">I termini di sollecito di consegna sono identificati da un codice che deve essere assegnato ai fornitori.</span><span class="sxs-lookup"><span data-stu-id="cf19d-107">Delivery reminder terms are identified by a code that must be assigned to vendors.</span></span> <span data-ttu-id="cf19d-108">Per utilizzare più di una combinazione delle impostazioni, è necessario impostare un codice per ciascuna di esse separatamente.</span><span class="sxs-lookup"><span data-stu-id="cf19d-108">To use more than one combination of settings, you must set up a code for each setting separately.</span></span> <span data-ttu-id="cf19d-109">È possibile impostare un numero qualsiasi di termini di sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="cf19d-109">You can set up any number of delivery reminder terms.</span></span>  

- <span data-ttu-id="cf19d-110">Livelli del sollecito di consegna</span><span class="sxs-lookup"><span data-stu-id="cf19d-110">Delivery reminder levels</span></span>  

    <span data-ttu-id="cf19d-111">Per ogni termine di sollecito di consegna, è necessario impostare i livelli di sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="cf19d-111">For every delivery reminder term, you must set up delivery reminder levels.</span></span> <span data-ttu-id="cf19d-112">Questi livelli determinano la frequenza di creazione dei promemoria di consegna per un determinato termine.</span><span class="sxs-lookup"><span data-stu-id="cf19d-112">These levels determine how often delivery reminders can be created for a specific term.</span></span> <span data-ttu-id="cf19d-113">Il livello 1 è il primo sollecito di consegna creato per una consegna scaduta.</span><span class="sxs-lookup"><span data-stu-id="cf19d-113">Level 1 is the first delivery reminder that you create for an overdue delivery.</span></span> <span data-ttu-id="cf19d-114">Il livello 2 è il secondo sollecito di consegna e così via.</span><span class="sxs-lookup"><span data-stu-id="cf19d-114">Level 2 is the second delivery reminder, and so on.</span></span> <span data-ttu-id="cf19d-115">Quando vengono creati i solleciti di consegna, viene considerato il numero di solleciti creati in precedenza e il numero corrente viene utilizzato per applicare i termini.</span><span class="sxs-lookup"><span data-stu-id="cf19d-115">When delivery reminders are created, the number of reminders that were created previously is considered, and the current number is used to apply terms.</span></span>  

- <span data-ttu-id="cf19d-116">Messaggi di testo di sollecito di consegna</span><span class="sxs-lookup"><span data-stu-id="cf19d-116">Delivery reminder texts messages</span></span>  

    <span data-ttu-id="cf19d-117">Per ogni livello di sollecito di consegna, è necessario impostare i messaggi di testo di sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="cf19d-117">You must set up delivery reminder text messages for every delivery reminder level.</span></span> <span data-ttu-id="cf19d-118">Sono disponibili due tipi di messaggi di testo di sollecito di consegna: iniziale e finale.</span><span class="sxs-lookup"><span data-stu-id="cf19d-118">There are two types of delivery reminder text messages: beginning and ending.</span></span> <span data-ttu-id="cf19d-119">Il messaggio di testo iniziale viene stampato sotto la sezione intestazione, prima dell'elenco delle voci contrassegnate per il sollecito.</span><span class="sxs-lookup"><span data-stu-id="cf19d-119">The beginning text message is printed under the header section, before the list of entries that are marked for reminder.</span></span> <span data-ttu-id="cf19d-120">Il messaggio di testo finale viene stampato dopo questo elenco.</span><span class="sxs-lookup"><span data-stu-id="cf19d-120">The ending text message is printed after this list.</span></span>  

<span data-ttu-id="cf19d-121">Per ulteriori informazioni, vedere [Impostare termini, livelli e testo dei solleciti di consegna](how-to-set-up-delivery-reminder-terms-levels-and-text.md).</span><span class="sxs-lookup"><span data-stu-id="cf19d-121">For more information, see [Set Up Delivery Reminder Terms, Levels, and Text](how-to-set-up-delivery-reminder-terms-levels-and-text.md).</span></span>  

<span data-ttu-id="cf19d-122">Dopo aver impostato i termini di consegna, è necessario assegnare ai fornitori i codici del termine di sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="cf19d-122">After you have set up the delivery terms, you must assign the delivery reminder term codes to vendors.</span></span> <span data-ttu-id="cf19d-123">Per ulteriori informazioni, vedere [Assegnare codici di solleciti di consegna ai fornitori](how-to-assign-delivery-reminder-codes-to-vendors.md).</span><span class="sxs-lookup"><span data-stu-id="cf19d-123">For more information, see [Assign Delivery Reminder Codes to Vendors](how-to-assign-delivery-reminder-codes-to-vendors.md).</span></span>  

<span data-ttu-id="cf19d-124">È possibile creare i solleciti di consegna manualmente o automaticamente.</span><span class="sxs-lookup"><span data-stu-id="cf19d-124">You can create delivery reminders manually or automatically.</span></span> <span data-ttu-id="cf19d-125">È possibile usare il processo batch **Crea sollecito di consegna** per creare automaticamente i solleciti di consegna.</span><span class="sxs-lookup"><span data-stu-id="cf19d-125">You can use the **Create Delivery Reminder** batch job to create delivery reminders automatically.</span></span> <span data-ttu-id="cf19d-126">Questo processo batch consente di selezionare gli ordini di acquisto per i quali devono essere creati i solleciti di consegna.</span><span class="sxs-lookup"><span data-stu-id="cf19d-126">This batch job allows you to select the purchase orders for which delivery reminders must be created.</span></span> <span data-ttu-id="cf19d-127">Per ulteriori informazioni, vedere [Generare solleciti di consegna](how-to-issue-delivery-reminders.md).</span><span class="sxs-lookup"><span data-stu-id="cf19d-127">For more information, see [Generate Delivery Reminders](how-to-issue-delivery-reminders.md).</span></span>  

<span data-ttu-id="cf19d-128">È possibile anche tracciare i documenti in relazione alle righe degli ordini di vendita e di acquisto.</span><span class="sxs-lookup"><span data-stu-id="cf19d-128">You can also track documents in relation to purchase order lines and sales order lines.</span></span>  

[!INCLUDE[d365fin](../../includes/d365fin_md.md)]<span data-ttu-id="cf19d-129"> fornisce i seguenti report:</span><span class="sxs-lookup"><span data-stu-id="cf19d-129"> provides the following reports:</span></span>  

- <span data-ttu-id="cf19d-130">**Sollecito di consegna inviato** - Per visualizzare i solleciti di consegna per i fornitori.</span><span class="sxs-lookup"><span data-stu-id="cf19d-130">**Issued Delivery Reminder** - To view the delivery reminders for vendors.</span></span>  
- <span data-ttu-id="cf19d-131">**Sollecito di consegna - Test** - Per verificare i solleciti di consegna prima dell'invio.</span><span class="sxs-lookup"><span data-stu-id="cf19d-131">**Delivery Reminder - Test** - To verify the delivery reminders before you issue them.</span></span>  

<span data-ttu-id="cf19d-132">Per ulteriori informazioni, vedere [Stampare report di test per i solleciti di consegna](how-to-print-test-reports-for-delivery-reminders.md).</span><span class="sxs-lookup"><span data-stu-id="cf19d-132">For more information, see [Print Test Reports for Delivery Reminders](how-to-print-test-reports-for-delivery-reminders.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="cf19d-133">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="cf19d-133">See Also</span></span>  
 <span data-ttu-id="cf19d-134">[Impostare solleciti di consegna](how-to-set-up-delivery-reminders.md) </span><span class="sxs-lookup"><span data-stu-id="cf19d-134">[Set Up Delivery Reminders](how-to-set-up-delivery-reminders.md) </span></span>  
 <span data-ttu-id="cf19d-135">[Impostare i termini, i livelli e i testi di sollecito di consegna](how-to-set-up-delivery-reminder-terms-levels-and-text.md) </span><span class="sxs-lookup"><span data-stu-id="cf19d-135">[Set Up Delivery Reminder Terms, Levels, and Text](how-to-set-up-delivery-reminder-terms-levels-and-text.md) </span></span>  
 <span data-ttu-id="cf19d-136">[Assegnare codici di solleciti di consegna ai fornitori](how-to-assign-delivery-reminder-codes-to-vendors.md) </span><span class="sxs-lookup"><span data-stu-id="cf19d-136">[Assign Delivery Reminder Codes to Vendors](how-to-assign-delivery-reminder-codes-to-vendors.md) </span></span>  
 <span data-ttu-id="cf19d-137">[Generare solleciti di consegna](how-to-generate-delivery-reminders.md) </span><span class="sxs-lookup"><span data-stu-id="cf19d-137">[Generate Delivery Reminders](how-to-generate-delivery-reminders.md) </span></span>  
 <span data-ttu-id="cf19d-138">[Creare solleciti di consegna manualmente](how-to-create-delivery-reminders-manually.md) </span><span class="sxs-lookup"><span data-stu-id="cf19d-138">[Create Delivery Reminders Manually](how-to-create-delivery-reminders-manually.md) </span></span>  
 <span data-ttu-id="cf19d-139">[Emettere solleciti di consegna](how-to-issue-delivery-reminders.md) </span><span class="sxs-lookup"><span data-stu-id="cf19d-139">[Issue Delivery Reminders](how-to-issue-delivery-reminders.md) </span></span>  
 [<span data-ttu-id="cf19d-140">Stampare report di test per i solleciti di consegna</span><span class="sxs-lookup"><span data-stu-id="cf19d-140">Print Test Reports for Delivery Reminders</span></span>](how-to-print-test-reports-for-delivery-reminders.md)

