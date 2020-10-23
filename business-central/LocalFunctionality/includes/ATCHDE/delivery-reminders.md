---
author: edupont04
ms.service: dynamics365-business-central
ms.topic: include
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 1e7cb126ea06d96bd130d644948d08fd7e2e1a11
ms.sourcegitcommit: 428f180604e5afcf94fa0e92a0615f58c88e13cd
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 10/02/2020
ms.locfileid: "3959661"
---
<span data-ttu-id="32e7c-101">I solleciti di consegna sono usati per tracciare le consegne scadute dei fornitori e per segnalare ai fornitori le consegne scadute.</span><span class="sxs-lookup"><span data-stu-id="32e7c-101">Delivery reminders are used to track overdue vendor shipments and to remind vendors about overdue deliveries.</span></span> <span data-ttu-id="32e7c-102">Per creare i solleciti di consegna è necessario impostare quanto segue:</span><span class="sxs-lookup"><span data-stu-id="32e7c-102">To create delivery reminders, you must set up the following:</span></span>

- <span data-ttu-id="32e7c-103">Termini di sollecito di consegna</span><span class="sxs-lookup"><span data-stu-id="32e7c-103">Delivery reminder terms</span></span>  

    <span data-ttu-id="32e7c-104">I termini di sollecito di consegna sono identificati da un codice che deve essere assegnato ai fornitori.</span><span class="sxs-lookup"><span data-stu-id="32e7c-104">Delivery reminder terms are identified by a code that must be assigned to vendors.</span></span> <span data-ttu-id="32e7c-105">Per utilizzare più di una combinazione delle impostazioni, è necessario impostare un codice per ciascuna di esse separatamente.</span><span class="sxs-lookup"><span data-stu-id="32e7c-105">To use more than one combination of settings, you must set up a code for each setting separately.</span></span> <span data-ttu-id="32e7c-106">È possibile impostare un numero qualsiasi di termini di sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="32e7c-106">You can set up any number of delivery reminder terms.</span></span>  

- <span data-ttu-id="32e7c-107">Livelli del sollecito di consegna</span><span class="sxs-lookup"><span data-stu-id="32e7c-107">Delivery reminder levels</span></span>  

    <span data-ttu-id="32e7c-108">Per ogni termine di sollecito di consegna, è necessario impostare i livelli di sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="32e7c-108">For every delivery reminder term, you must set up delivery reminder levels.</span></span> <span data-ttu-id="32e7c-109">Questi livelli determinano la frequenza di creazione dei promemoria di consegna per un determinato termine.</span><span class="sxs-lookup"><span data-stu-id="32e7c-109">These levels determine how often delivery reminders can be created for a specific term.</span></span> <span data-ttu-id="32e7c-110">Il livello 1 è il primo sollecito di consegna creato per una consegna scaduta.</span><span class="sxs-lookup"><span data-stu-id="32e7c-110">Level 1 is the first delivery reminder that you create for an overdue delivery.</span></span> <span data-ttu-id="32e7c-111">Il livello 2 è il secondo sollecito di consegna e così via.</span><span class="sxs-lookup"><span data-stu-id="32e7c-111">Level 2 is the second delivery reminder, and so on.</span></span> <span data-ttu-id="32e7c-112">Quando vengono creati i solleciti di consegna, viene considerato il numero di solleciti creati in precedenza e il numero corrente viene utilizzato per applicare i termini.</span><span class="sxs-lookup"><span data-stu-id="32e7c-112">When delivery reminders are created, the number of reminders that were created previously is considered, and the current number is used to apply terms.</span></span>  

- <span data-ttu-id="32e7c-113">Messaggi di testo di sollecito di consegna</span><span class="sxs-lookup"><span data-stu-id="32e7c-113">Delivery reminder texts messages</span></span>  

    <span data-ttu-id="32e7c-114">Per ogni livello di sollecito di consegna, è necessario impostare i messaggi di testo di sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="32e7c-114">You must set up delivery reminder text messages for every delivery reminder level.</span></span> <span data-ttu-id="32e7c-115">Sono disponibili due tipi di messaggi di testo di sollecito di consegna: iniziale e finale.</span><span class="sxs-lookup"><span data-stu-id="32e7c-115">There are two types of delivery reminder text messages: beginning and ending.</span></span> <span data-ttu-id="32e7c-116">Il messaggio di testo iniziale viene stampato sotto la sezione intestazione, prima dell'elenco delle voci contrassegnate per il sollecito.</span><span class="sxs-lookup"><span data-stu-id="32e7c-116">The beginning text message is printed under the header section, before the list of entries that are marked for reminder.</span></span> <span data-ttu-id="32e7c-117">Il messaggio di testo finale viene stampato dopo questo elenco.</span><span class="sxs-lookup"><span data-stu-id="32e7c-117">The ending text message is printed after this list.</span></span>  

<span data-ttu-id="32e7c-118">Dopo aver impostato i testi, i livelli e i termini di consegna, è necessario assegnare ai fornitori i codici del sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="32e7c-118">After you have set up the delivery terms, levels, and texts, you must assign the relevant delivery reminder codes to your vendors.</span></span>  

<span data-ttu-id="32e7c-119">È possibile creare i solleciti di consegna manualmente o automaticamente.</span><span class="sxs-lookup"><span data-stu-id="32e7c-119">You can create delivery reminders manually or automatically.</span></span> <span data-ttu-id="32e7c-120">È possibile usare il processo batch **Crea sollecito di consegna** per creare automaticamente i solleciti di consegna in modo da poter selezionare gli ordini di acquisto per i quali è necessario creare i solleciti di consegna.</span><span class="sxs-lookup"><span data-stu-id="32e7c-120">You can use the **Create Delivery Reminder** batch job to create delivery reminders automatically so that you can select the purchase orders for which delivery reminders must be created.</span></span>  

<span data-ttu-id="32e7c-121">È possibile anche tracciare i documenti in relazione alle righe degli ordini di vendita e di acquisto.</span><span class="sxs-lookup"><span data-stu-id="32e7c-121">You can also track documents in relation to purchase order lines and sales order lines.</span></span>  

[!INCLUDE[d365fin](../../../includes/d365fin_md.md)] <span data-ttu-id="32e7c-122">fornisce i seguenti report:</span><span class="sxs-lookup"><span data-stu-id="32e7c-122">provides the following reports:</span></span>  

- <span data-ttu-id="32e7c-123">**Sollecito di consegna inviato** - Per visualizzare i solleciti di consegna per i fornitori.</span><span class="sxs-lookup"><span data-stu-id="32e7c-123">**Issued Delivery Reminder** - To view the delivery reminders for vendors.</span></span>  
- <span data-ttu-id="32e7c-124">**Sollecito di consegna - Test** - Per verificare i solleciti di consegna prima dell'invio.</span><span class="sxs-lookup"><span data-stu-id="32e7c-124">**Delivery Reminder - Test** - To verify the delivery reminders before you issue them.</span></span>  
