---
author: edupont04
ms.service: dynamics365-business-central
ms.topic: include
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 5609b99f8d05402b79c22fee8f7a70dc7e82b22c
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 03/31/2021
ms.locfileid: "5771537"
---
<span data-ttu-id="f086f-101">I solleciti di consegna sono usati per tracciare le consegne scadute dei fornitori e per segnalare ai fornitori le consegne scadute.</span><span class="sxs-lookup"><span data-stu-id="f086f-101">Delivery reminders are used to track overdue vendor shipments and to remind vendors about overdue deliveries.</span></span> <span data-ttu-id="f086f-102">Per creare i solleciti di consegna è necessario impostare quanto segue:</span><span class="sxs-lookup"><span data-stu-id="f086f-102">To create delivery reminders, you must set up the following:</span></span>

- <span data-ttu-id="f086f-103">Termini di sollecito di consegna</span><span class="sxs-lookup"><span data-stu-id="f086f-103">Delivery reminder terms</span></span>  

    <span data-ttu-id="f086f-104">I termini di sollecito di consegna sono identificati da un codice che deve essere assegnato ai fornitori.</span><span class="sxs-lookup"><span data-stu-id="f086f-104">Delivery reminder terms are identified by a code that must be assigned to vendors.</span></span> <span data-ttu-id="f086f-105">Per utilizzare più di una combinazione delle impostazioni, è necessario impostare un codice per ciascuna di esse separatamente.</span><span class="sxs-lookup"><span data-stu-id="f086f-105">To use more than one combination of settings, you must set up a code for each setting separately.</span></span> <span data-ttu-id="f086f-106">È possibile impostare un numero qualsiasi di termini di sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="f086f-106">You can set up any number of delivery reminder terms.</span></span>  

- <span data-ttu-id="f086f-107">Livelli del sollecito di consegna</span><span class="sxs-lookup"><span data-stu-id="f086f-107">Delivery reminder levels</span></span>  

    <span data-ttu-id="f086f-108">Per ogni termine di sollecito di consegna, è necessario impostare i livelli di sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="f086f-108">For every delivery reminder term, you must set up delivery reminder levels.</span></span> <span data-ttu-id="f086f-109">Questi livelli determinano la frequenza di creazione dei promemoria di consegna per un determinato termine.</span><span class="sxs-lookup"><span data-stu-id="f086f-109">These levels determine how often delivery reminders can be created for a specific term.</span></span> <span data-ttu-id="f086f-110">Il livello 1 è il primo sollecito di consegna creato per una consegna scaduta.</span><span class="sxs-lookup"><span data-stu-id="f086f-110">Level 1 is the first delivery reminder that you create for an overdue delivery.</span></span> <span data-ttu-id="f086f-111">Il livello 2 è il secondo sollecito di consegna e così via.</span><span class="sxs-lookup"><span data-stu-id="f086f-111">Level 2 is the second delivery reminder, and so on.</span></span> <span data-ttu-id="f086f-112">Quando vengono creati i solleciti di consegna, viene considerato il numero di solleciti creati in precedenza e il numero corrente viene utilizzato per applicare i termini.</span><span class="sxs-lookup"><span data-stu-id="f086f-112">When delivery reminders are created, the number of reminders that were created previously is considered, and the current number is used to apply terms.</span></span>  

- <span data-ttu-id="f086f-113">Messaggi di testo di sollecito di consegna</span><span class="sxs-lookup"><span data-stu-id="f086f-113">Delivery reminder texts messages</span></span>  

    <span data-ttu-id="f086f-114">Per ogni livello di sollecito di consegna, è necessario impostare i messaggi di testo di sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="f086f-114">You must set up delivery reminder text messages for every delivery reminder level.</span></span> <span data-ttu-id="f086f-115">Sono disponibili due tipi di messaggi di testo di sollecito di consegna: iniziale e finale.</span><span class="sxs-lookup"><span data-stu-id="f086f-115">There are two types of delivery reminder text messages: beginning and ending.</span></span> <span data-ttu-id="f086f-116">Il messaggio di testo iniziale viene stampato sotto la sezione intestazione, prima dell'elenco delle voci contrassegnate per il sollecito.</span><span class="sxs-lookup"><span data-stu-id="f086f-116">The beginning text message is printed under the header section, before the list of entries that are marked for reminder.</span></span> <span data-ttu-id="f086f-117">Il messaggio di testo finale viene stampato dopo questo elenco.</span><span class="sxs-lookup"><span data-stu-id="f086f-117">The ending text message is printed after this list.</span></span>  

<span data-ttu-id="f086f-118">Dopo aver impostato i testi, i livelli e i termini di consegna, è necessario assegnare ai fornitori i codici del sollecito di consegna.</span><span class="sxs-lookup"><span data-stu-id="f086f-118">After you have set up the delivery terms, levels, and texts, you must assign the relevant delivery reminder codes to your vendors.</span></span>  

<span data-ttu-id="f086f-119">È possibile creare i solleciti di consegna manualmente o automaticamente.</span><span class="sxs-lookup"><span data-stu-id="f086f-119">You can create delivery reminders manually or automatically.</span></span> <span data-ttu-id="f086f-120">È possibile usare il processo batch **Crea sollecito di consegna** per creare automaticamente i solleciti di consegna in modo da poter selezionare gli ordini di acquisto per i quali è necessario creare i solleciti di consegna.</span><span class="sxs-lookup"><span data-stu-id="f086f-120">You can use the **Create Delivery Reminder** batch job to create delivery reminders automatically so that you can select the purchase orders for which delivery reminders must be created.</span></span>  

<span data-ttu-id="f086f-121">È possibile anche tracciare i documenti in relazione alle righe degli ordini di vendita e di acquisto.</span><span class="sxs-lookup"><span data-stu-id="f086f-121">You can also track documents in relation to purchase order lines and sales order lines.</span></span>  

[!INCLUDE[prod_short](../../../includes/prod_short.md)] <span data-ttu-id="f086f-122">fornisce i seguenti report:</span><span class="sxs-lookup"><span data-stu-id="f086f-122">provides the following reports:</span></span>  

- <span data-ttu-id="f086f-123">**Sollecito di consegna inviato** - Per visualizzare i solleciti di consegna per i fornitori.</span><span class="sxs-lookup"><span data-stu-id="f086f-123">**Issued Delivery Reminder** - To view the delivery reminders for vendors.</span></span>  
- <span data-ttu-id="f086f-124">**Sollecito di consegna - Test** - Per verificare i solleciti di consegna prima dell'invio.</span><span class="sxs-lookup"><span data-stu-id="f086f-124">**Delivery Reminder - Test** - To verify the delivery reminders before you issue them.</span></span>  
