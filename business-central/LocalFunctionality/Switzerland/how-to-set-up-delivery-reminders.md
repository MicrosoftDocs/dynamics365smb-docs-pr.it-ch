---
title: Come impostare solleciti di consegna
description: In Business Central, è possibile usare solleciti di consegna per segnalare ai fornitori le consegne scadute.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2018
ms.author: sgroespe
ms.openlocfilehash: fc2945da396d69ea190bf49ff1242b1aba7aa71e
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 03/08/2019
ms.locfileid: "827376"
---
# <a name="set-up-delivery-reminders"></a><span data-ttu-id="2790a-103">Impostare solleciti di consegna</span><span class="sxs-lookup"><span data-stu-id="2790a-103">Set Up Delivery Reminders</span></span>
<span data-ttu-id="2790a-104">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], è possibile usare solleciti di consegna per segnalare ai fornitori le consegne scadute.</span><span class="sxs-lookup"><span data-stu-id="2790a-104">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you can use purchase delivery reminders to remind vendors about overdue deliveries.</span></span> <span data-ttu-id="2790a-105">Per creare solleciti di consegna per i fornitori, è necessario impostare dati di base per la creazione di solleciti di consegna e numerazioni per i solleciti di consegna nella pagina **Setup contabilità fornitori e acquisti**.</span><span class="sxs-lookup"><span data-stu-id="2790a-105">To create delivery reminders for vendors, you must set up base data for delivery reminder creation and number series for the delivery reminders on the **Purchases & Payables Setup** page.</span></span>  

## <a name="to-set-up-delivery-reminders"></a><span data-ttu-id="2790a-106">Per impostare solleciti di consegna</span><span class="sxs-lookup"><span data-stu-id="2790a-106">To set up delivery reminders</span></span>  

1.  <span data-ttu-id="2790a-107">Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Setup contabilità fornitori e acquisti**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="2790a-107">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchases & Payables Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="2790a-108">Nella Scheda dettaglio **Generale**, nel campo **Data sollecito eliminato di default** specificare una delle opzioni seguenti come descritto in questa tabella.</span><span class="sxs-lookup"><span data-stu-id="2790a-108">On the **General** FastTab, in the **Default Del. Rem. Date Field** field, specify one of the following options as described in the following table.</span></span>  

    |<span data-ttu-id="2790a-109">Opzione</span><span class="sxs-lookup"><span data-stu-id="2790a-109">Option</span></span>|<span data-ttu-id="2790a-110">Descrizione</span><span class="sxs-lookup"><span data-stu-id="2790a-110">Description</span></span>|  
    |----------------------------------|---------------------------------------|  
    |<span data-ttu-id="2790a-111">**Data di carico richiesta**</span><span class="sxs-lookup"><span data-stu-id="2790a-111">**Requested Receipt Date**</span></span>|<span data-ttu-id="2790a-112">Specifica che il valore della data nel campo **Data di carico richiesta** sulla riga ordine di acquisto verrà usato come data di default per la creazione di solleciti di consegna.</span><span class="sxs-lookup"><span data-stu-id="2790a-112">To specify that the date value in the **Requested Receipt Date** field on the purchase order line will be used as the default date for creating delivery reminders.</span></span>|  
    |<span data-ttu-id="2790a-113">**Data di carico promessa**</span><span class="sxs-lookup"><span data-stu-id="2790a-113">**Promised Receipt Date**</span></span>|<span data-ttu-id="2790a-114">Specifica che il valore della data nel campo **Data di carico promessa** sulla riga ordine di acquisto verrà usato come data di default per la creazione di solleciti di consegna.</span><span class="sxs-lookup"><span data-stu-id="2790a-114">To specify that the date value in the **Promised Receipt Date** field on the purchase order line will be used as the default date for creating delivery reminders.</span></span>|  
    |<span data-ttu-id="2790a-115">**Data carico prevista**</span><span class="sxs-lookup"><span data-stu-id="2790a-115">**Expected Receipt Date**</span></span>|<span data-ttu-id="2790a-116">Specifica che il valore della data nel campo **Data carico prevista** sulla riga ordine di acquisto verrà usato come data di default per la creazione di solleciti di consegna.</span><span class="sxs-lookup"><span data-stu-id="2790a-116">To specify that the date value in the **Expected Receipt Date** field on the purchase order line will be used as the default date for creating delivery reminders.</span></span>|  

3.  <span data-ttu-id="2790a-117">Nella Scheda Dettaglio **Numerazione** compilare i campi come indicato nella tabella seguente.</span><span class="sxs-lookup"><span data-stu-id="2790a-117">On the **Numbering** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="2790a-118">Campo</span><span class="sxs-lookup"><span data-stu-id="2790a-118">Field</span></span>|<span data-ttu-id="2790a-119">Descrizione</span><span class="sxs-lookup"><span data-stu-id="2790a-119">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="2790a-120">**Nr. Solleciti Consegna**</span><span class="sxs-lookup"><span data-stu-id="2790a-120">**Delivery Reminder Nos.**</span></span>|<span data-ttu-id="2790a-121">Codice numerazione per i solleciti di consegna.</span><span class="sxs-lookup"><span data-stu-id="2790a-121">The number series code for delivery reminders.</span></span>|  
    |<span data-ttu-id="2790a-122">**Nr. Solleciti Consegna Emessi**</span><span class="sxs-lookup"><span data-stu-id="2790a-122">**Issued Delivery Reminder Nos.**</span></span>|<span data-ttu-id="2790a-123">Codice numerazione per i solleciti di consegna inviati.</span><span class="sxs-lookup"><span data-stu-id="2790a-123">The number series code for issued delivery reminders.</span></span>|  

4.  <span data-ttu-id="2790a-124">Scegliere il pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="2790a-124">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="2790a-125">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="2790a-125">See Also</span></span>  
 <span data-ttu-id="2790a-126">[Solleciti consegna](delivery-reminders.md) </span><span class="sxs-lookup"><span data-stu-id="2790a-126">[Delivery Reminders](delivery-reminders.md) </span></span>  
 <span data-ttu-id="2790a-127">[Impostare i termini, i livelli e i testi di sollecito di consegna](how-to-set-up-delivery-reminder-terms-levels-and-text.md) </span><span class="sxs-lookup"><span data-stu-id="2790a-127">[Set Up Delivery Reminder Terms, Levels, and Text](how-to-set-up-delivery-reminder-terms-levels-and-text.md) </span></span>  
 <span data-ttu-id="2790a-128">[Assegnare codici di solleciti di consegna ai fornitori](how-to-assign-delivery-reminder-codes-to-vendors.md) </span><span class="sxs-lookup"><span data-stu-id="2790a-128">[Assign Delivery Reminder Codes to Vendors](how-to-assign-delivery-reminder-codes-to-vendors.md) </span></span>  
 [<span data-ttu-id="2790a-129">Creare solleciti di consegna manualmente</span><span class="sxs-lookup"><span data-stu-id="2790a-129">Create Delivery Reminders Manually</span></span>](how-to-create-delivery-reminders-manually.md)
