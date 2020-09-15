---
title: Come impostare solleciti di consegna
description: In Business Central, è possibile usare solleciti di consegna per segnalare ai fornitori le consegne scadute.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 07/23/2020
ms.author: edupont
ms.openlocfilehash: 4db91ff9973a1ad63bc651c2e2c07c16630d4d73
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 09/09/2020
ms.locfileid: "3778192"
---
# <a name="set-up-delivery-reminders"></a><span data-ttu-id="1c0e9-103">Impostare solleciti di consegna</span><span class="sxs-lookup"><span data-stu-id="1c0e9-103">Set Up Delivery Reminders</span></span>

<span data-ttu-id="1c0e9-104">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], è possibile usare solleciti di consegna per segnalare ai fornitori le consegne scadute.</span><span class="sxs-lookup"><span data-stu-id="1c0e9-104">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you can use purchase delivery reminders to remind vendors about overdue deliveries.</span></span> <span data-ttu-id="1c0e9-105">Per creare solleciti di consegna per i fornitori, è necessario impostare dati di base per la creazione di solleciti di consegna e numerazioni per i solleciti di consegna nella pagina **Setup contabilità fornitori e acquisti**.</span><span class="sxs-lookup"><span data-stu-id="1c0e9-105">To create delivery reminders for vendors, you must set up base data for delivery reminder creation and number series for the delivery reminders on the **Purchases & Payables Setup** page.</span></span>  

## <a name="to-set-up-delivery-reminders"></a><span data-ttu-id="1c0e9-106">Per impostare solleciti di consegna</span><span class="sxs-lookup"><span data-stu-id="1c0e9-106">To set up delivery reminders</span></span>  

1. <span data-ttu-id="1c0e9-107">Scegliere l'![icona a forma di lampadina che consente di aprire la funzionalità delle informazioni](../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Setup contabilità fornitori e acquisti** e quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="1c0e9-107">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchases & Payables Setup**, and then choose the related link.</span></span>  
2. <span data-ttu-id="1c0e9-108">Nella Scheda dettaglio **Generale**, nel campo **Data sollecito eliminato di default** specificare una delle opzioni seguenti come descritto in questa tabella.</span><span class="sxs-lookup"><span data-stu-id="1c0e9-108">On the **General** FastTab, in the **Default Del. Rem. Date Field** field, specify one of the following options as described in the following table.</span></span>  

    |<span data-ttu-id="1c0e9-109">Opzione</span><span class="sxs-lookup"><span data-stu-id="1c0e9-109">Option</span></span>|<span data-ttu-id="1c0e9-110">Descrizione</span><span class="sxs-lookup"><span data-stu-id="1c0e9-110">Description</span></span>|  
    |----------------------------------|---------------------------------------|  
    |<span data-ttu-id="1c0e9-111">**Data di carico richiesta**</span><span class="sxs-lookup"><span data-stu-id="1c0e9-111">**Requested Receipt Date**</span></span>|<span data-ttu-id="1c0e9-112">Specifica che il valore della data nel campo **Data di carico richiesta** sulla riga ordine di acquisto verrà usato come data di default per la creazione di solleciti di consegna.</span><span class="sxs-lookup"><span data-stu-id="1c0e9-112">To specify that the date value in the **Requested Receipt Date** field on the purchase order line will be used as the default date for creating delivery reminders.</span></span>|  
    |<span data-ttu-id="1c0e9-113">**Data di carico promessa**</span><span class="sxs-lookup"><span data-stu-id="1c0e9-113">**Promised Receipt Date**</span></span>|<span data-ttu-id="1c0e9-114">Specifica che il valore della data nel campo **Data di carico promessa** sulla riga ordine di acquisto verrà usato come data di default per la creazione di solleciti di consegna.</span><span class="sxs-lookup"><span data-stu-id="1c0e9-114">To specify that the date value in the **Promised Receipt Date** field on the purchase order line will be used as the default date for creating delivery reminders.</span></span>|  
    |<span data-ttu-id="1c0e9-115">**Data carico prevista**</span><span class="sxs-lookup"><span data-stu-id="1c0e9-115">**Expected Receipt Date**</span></span>|<span data-ttu-id="1c0e9-116">Specifica che il valore della data nel campo **Data carico prevista** sulla riga ordine di acquisto verrà usato come data di default per la creazione di solleciti di consegna.</span><span class="sxs-lookup"><span data-stu-id="1c0e9-116">To specify that the date value in the **Expected Receipt Date** field on the purchase order line will be used as the default date for creating delivery reminders.</span></span>|  

3. <span data-ttu-id="1c0e9-117">Nella Scheda Dettaglio **Numerazione** compilare i campi come indicato nella tabella seguente.</span><span class="sxs-lookup"><span data-stu-id="1c0e9-117">On the **Numbering** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="1c0e9-118">Campo</span><span class="sxs-lookup"><span data-stu-id="1c0e9-118">Field</span></span>|<span data-ttu-id="1c0e9-119">Descrizione</span><span class="sxs-lookup"><span data-stu-id="1c0e9-119">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="1c0e9-120">**Nr. Solleciti Consegna**</span><span class="sxs-lookup"><span data-stu-id="1c0e9-120">**Delivery Reminder Nos.**</span></span>|<span data-ttu-id="1c0e9-121">Codice numerazione per i solleciti di consegna.</span><span class="sxs-lookup"><span data-stu-id="1c0e9-121">The number series code for delivery reminders.</span></span>|  
    |<span data-ttu-id="1c0e9-122">**Nr. Solleciti Consegna Emessi**</span><span class="sxs-lookup"><span data-stu-id="1c0e9-122">**Issued Delivery Reminder Nos.**</span></span>|<span data-ttu-id="1c0e9-123">Codice numerazione per i solleciti di consegna inviati.</span><span class="sxs-lookup"><span data-stu-id="1c0e9-123">The number series code for issued delivery reminders.</span></span>|  

4. <span data-ttu-id="1c0e9-124">Scegliere il pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="1c0e9-124">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="1c0e9-125">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="1c0e9-125">See Also</span></span>

[<span data-ttu-id="1c0e9-126">Solleciti consegna</span><span class="sxs-lookup"><span data-stu-id="1c0e9-126">Delivery Reminders</span></span>](delivery-reminders.md)  
[<span data-ttu-id="1c0e9-127">Impostare i termini, i livelli e i testi di sollecito di consegna</span><span class="sxs-lookup"><span data-stu-id="1c0e9-127">Set Up Delivery Reminder Terms, Levels, and Text</span></span>](how-to-set-up-delivery-reminder-terms-levels-and-text.md)  
[<span data-ttu-id="1c0e9-128">Assegnare codici di solleciti di consegna ai fornitori</span><span class="sxs-lookup"><span data-stu-id="1c0e9-128">Assign Delivery Reminder Codes to Vendors</span></span>](how-to-assign-delivery-reminder-codes-to-vendors.md)  
[<span data-ttu-id="1c0e9-129">Creare solleciti di consegna manualmente</span><span class="sxs-lookup"><span data-stu-id="1c0e9-129">Create Delivery Reminders Manually</span></span>](how-to-create-delivery-reminders-manually.md)
