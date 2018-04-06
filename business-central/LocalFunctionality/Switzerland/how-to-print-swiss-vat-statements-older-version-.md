---
title: Come stampare dichiarazioni IVA svizzere (versione precedente)
description: "La **dichiarazione IVA svizzera** è il rapporto di calcolo standard per la realizzazione dell'IVA. È possibile stampare questo rapporto e utilizzarlo per le dichiarazioni fiscali trimestrali."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 7fd4ae7c8b4e2edd9d46a0f306bac4a182a52f83
ms.contentlocale: it-ch
ms.lasthandoff: 03/22/2018

---
# <a name="print-swiss-vat-statements-older-version"></a><span data-ttu-id="e45f5-104">Stampare dichiarazioni IVA svizzere (versione precedente)</span><span class="sxs-lookup"><span data-stu-id="e45f5-104">Print Swiss VAT Statements (older version)</span></span>

> [!NOTE]  
>  <span data-ttu-id="e45f5-105">Questo argomento è mantenuto per la compatibilità con le versioni precedenti del report **Dichiarazione IVA svizzera**.</span><span class="sxs-lookup"><span data-stu-id="e45f5-105">This topic is retained for backward compatibility with the **Swiss VAT Statement** report.</span></span> <span data-ttu-id="e45f5-106">Per informazioni sull'utilizzo della più recente dichiarazione IVA svizzera, vedere Dichiarazione IVA svizzera.</span><span class="sxs-lookup"><span data-stu-id="e45f5-106">For information about using the newer Swiss VAT Statement, see Swiss VAT Statement.</span></span>  

<span data-ttu-id="e45f5-107">La **dichiarazione IVA svizzera** è il rapporto di calcolo standard per la realizzazione dell'IVA.</span><span class="sxs-lookup"><span data-stu-id="e45f5-107">The **Swiss VAT Statement** is the standard calculation report for realizing VAT.</span></span> <span data-ttu-id="e45f5-108">È possibile stampare questo rapporto e utilizzarlo per le dichiarazioni fiscali trimestrali.</span><span class="sxs-lookup"><span data-stu-id="e45f5-108">You can print this report, and use it for quarterly tax reporting.</span></span> <span data-ttu-id="e45f5-109">Nella **dichiarazione IVA svizzera** vengono incluse le seguenti informazioni:</span><span class="sxs-lookup"><span data-stu-id="e45f5-109">The **Swiss VAT Statement** includes the following:</span></span>  

- <span data-ttu-id="e45f5-110">Un movimento IVA.</span><span class="sxs-lookup"><span data-stu-id="e45f5-110">A VAT entry.</span></span>  
- <span data-ttu-id="e45f5-111">I movimenti di rettifica IVA.</span><span class="sxs-lookup"><span data-stu-id="e45f5-111">VAT adjusting entries.</span></span>  
- <span data-ttu-id="e45f5-112">Una scheda contabile.</span><span class="sxs-lookup"><span data-stu-id="e45f5-112">An accounting sheet.</span></span>  

## <a name="to-print-the-swiss-vat-statement"></a><span data-ttu-id="e45f5-113">Per stampare la dichiarazione IVA svizzera</span><span class="sxs-lookup"><span data-stu-id="e45f5-113">To print the Swiss VAT statement</span></span>  

1.  <span data-ttu-id="e45f5-114">Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Dichiarazione IVA svizzera**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="e45f5-114">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Swiss VAT Statement**, and then choose the related link.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="e45f5-115">Verrà ricevuto un messaggio indicante che la **dichiarazione IVA svizzera** viene aperta nella lingua locale.</span><span class="sxs-lookup"><span data-stu-id="e45f5-115">You will receive a message stating that the **Swiss VAT Statement** will open in the local language.</span></span>  

2.  <span data-ttu-id="e45f5-116">Nella Scheda dettaglio **Opzioni** compilare i campi come descritto nella tabella riportata di seguito.</span><span class="sxs-lookup"><span data-stu-id="e45f5-116">On the **Options** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="e45f5-117">Campo</span><span class="sxs-lookup"><span data-stu-id="e45f5-117">Field</span></span>|<span data-ttu-id="e45f5-118">Descrizione</span><span class="sxs-lookup"><span data-stu-id="e45f5-118">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="e45f5-119">**Chiusi con nr. di registrazione**</span><span class="sxs-lookup"><span data-stu-id="e45f5-119">**Closed with Journal no.**</span></span>|<span data-ttu-id="e45f5-120">Selezionare le registrazioni di contabilità generale che contengono l'origine di registrazione dei movimenti di rettifica IVA.</span><span class="sxs-lookup"><span data-stu-id="e45f5-120">Select the general ledger journals that contain the posting source of the VAT adjusting entries.</span></span> <span data-ttu-id="e45f5-121">Questo campo valuta i periodi contabili già liquidati.</span><span class="sxs-lookup"><span data-stu-id="e45f5-121">This field evaluates accounting periods that have already been settled.</span></span>|  
    |<span data-ttu-id="e45f5-122">**Aperti fino alla data**</span><span class="sxs-lookup"><span data-stu-id="e45f5-122">**Open until date**</span></span>|<span data-ttu-id="e45f5-123">Seleziona l'ultima data per la liquidazione di movimenti IVA aperti o non liquidati.</span><span class="sxs-lookup"><span data-stu-id="e45f5-123">Select the last date for settling open or unsettled VAT entries.</span></span>|  
    |<span data-ttu-id="e45f5-124">**Mostrare registrazioni**</span><span class="sxs-lookup"><span data-stu-id="e45f5-124">**Show Postings**</span></span>|<span data-ttu-id="e45f5-125">Specifica se verranno stampati tutti i movimenti IVA per ciascun gruppo.</span><span class="sxs-lookup"><span data-stu-id="e45f5-125">Specifies if all of the VAT entries for each group will be printed.</span></span>|  
    |<span data-ttu-id="e45f5-126">**Mostrare registrazioni di conguaglio**</span><span class="sxs-lookup"><span data-stu-id="e45f5-126">**Show Chargeback**</span></span>|<span data-ttu-id="e45f5-127">Specifica se verranno stampati i movimenti IVA e i movimenti di contabilità generale con riepiloghi chiusi o imposta registrata.</span><span class="sxs-lookup"><span data-stu-id="e45f5-127">Specifies if VAT entries and general ledger entries with closed summaries or reposted tax will be printed.</span></span>|  
    |<span data-ttu-id="e45f5-128">**Aliquota normale IVA %**</span><span class="sxs-lookup"><span data-stu-id="e45f5-128">**Normal rate VAT %**</span></span>|<span data-ttu-id="e45f5-129">Selezionare le aliquote IVA tipiche correnti utilizzate per assegnare le aliquote corrette ai gruppi di attività e prodotti definiti nelle impostazioni IVA.</span><span class="sxs-lookup"><span data-stu-id="e45f5-129">Select the current typical VAT rates used to assign the correct rates to the business and product groups defined in the VAT settings.</span></span>|  
    |<span data-ttu-id="e45f5-130">**Aliquota ridotta IVA %**</span><span class="sxs-lookup"><span data-stu-id="e45f5-130">**Reduced rate VAT %**</span></span>|<span data-ttu-id="e45f5-131">Selezionare le aliquote di imposta ridotte correnti utilizzate per assegnare le aliquote corrette ai gruppi di attività e prodotti definiti nelle impostazioni IVA.</span><span class="sxs-lookup"><span data-stu-id="e45f5-131">Select the current reduced tax rates used to assign the correct rates to the business and product groups defined in the VAT settings.</span></span>|  
    |<span data-ttu-id="e45f5-132">**% IVA aliquota speciale**</span><span class="sxs-lookup"><span data-stu-id="e45f5-132">**Special rate VAT %**</span></span>|<span data-ttu-id="e45f5-133">Selezionare le aliquote di imposta speciali correnti utilizzate per assegnare le aliquote corrette ai gruppi di attività e prodotti definiti nelle impostazioni IVA.</span><span class="sxs-lookup"><span data-stu-id="e45f5-133">Select the current special tax rates used to assign the correct rates to the business and product groups defined in the VAT settings.</span></span>|  
    |<span data-ttu-id="e45f5-134">**Conto C/G IVA investimenti/costi d'esercizio**</span><span class="sxs-lookup"><span data-stu-id="e45f5-134">**Investment/Operating Purchase VAT G/L Account**</span></span>|<span data-ttu-id="e45f5-135">Selezionare il conto di contabilità generale per l'IVA.</span><span class="sxs-lookup"><span data-stu-id="e45f5-135">Select the VAT general ledger account.</span></span>|  
    |<span data-ttu-id="e45f5-136">**Consumo proprio cat. reg. bus. IVA**</span><span class="sxs-lookup"><span data-stu-id="e45f5-136">**Own Consumption Bus. Group**</span></span>|<span data-ttu-id="e45f5-137">Seleziona il gruppo di attività e prodotti per il proprio consumo.</span><span class="sxs-lookup"><span data-stu-id="e45f5-137">Select the business and product group for own consumptions.</span></span>|  
    |<span data-ttu-id="e45f5-138">**Categoria reg. business servizi esteri**</span><span class="sxs-lookup"><span data-stu-id="e45f5-138">**Service Foreign Bus. Group**</span></span>|<span data-ttu-id="e45f5-139">Seleziona il gruppo di attività e prodotti per il servizio estero.</span><span class="sxs-lookup"><span data-stu-id="e45f5-139">Select the foreign service business and product group.</span></span>|  
    |<span data-ttu-id="e45f5-140">**Esportazioni cat. reg. bus.**</span><span class="sxs-lookup"><span data-stu-id="e45f5-140">**Export Bus. Group**</span></span>|<span data-ttu-id="e45f5-141">Seleziona il gruppo di attività e prodotti per le esportazioni.</span><span class="sxs-lookup"><span data-stu-id="e45f5-141">Select the business and product group for exports.</span></span>|  

3.  <span data-ttu-id="e45f5-142">Scegliere il pulsante **Stampa** per stampare la dichiarazione IVA oppure scegliere il pulsante **Anteprima** per visualizzarla sullo schermo.</span><span class="sxs-lookup"><span data-stu-id="e45f5-142">Choose the **Print** button to print the VAT statement or choose the **Preview** button to view it on the screen.</span></span>  

## <a name="see-also"></a><span data-ttu-id="e45f5-143">Vedere anche</span><span class="sxs-lookup"><span data-stu-id="e45f5-143">See Also</span></span>  
 <span data-ttu-id="e45f5-144">[IVA svizzera](swiss-value-added-tax.md) </span><span class="sxs-lookup"><span data-stu-id="e45f5-144">[Swiss Value Added Tax](swiss-value-added-tax.md) </span></span>  
 [<span data-ttu-id="e45f5-145">Aliquote IVA per la Svizzera</span><span class="sxs-lookup"><span data-stu-id="e45f5-145">VAT Rates for Switzerland</span></span>](vat-rates-for-switzerland.md)

