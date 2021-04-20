---
author: edupont04
ms.service: dynamics365-business-central
ms.topic: include
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 34d9ddd0c3afc97beb19c6c4c9441770656ef6e9
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 03/31/2021
ms.locfileid: "5771510"
---
<span data-ttu-id="518d3-101">In [!INCLUDE[prod_short](../../../includes/prod_short.md)], è possibile usare solleciti di consegna per segnalare ai fornitori le consegne scadute.</span><span class="sxs-lookup"><span data-stu-id="518d3-101">In [!INCLUDE[prod_short](../../../includes/prod_short.md)], you can use purchase delivery reminders to remind vendors about overdue deliveries.</span></span> <span data-ttu-id="518d3-102">Per creare solleciti di consegna per i fornitori, è necessario impostare dati di base per la creazione di solleciti di consegna e numerazioni per i solleciti di consegna nella pagina **Setup contabilità fornitori e acquisti**.</span><span class="sxs-lookup"><span data-stu-id="518d3-102">To create delivery reminders for vendors, you must set up base data for delivery reminder creation and number series for the delivery reminders on the **Purchases & Payables Setup** page.</span></span>  

## <a name="to-set-up-delivery-reminders"></a><span data-ttu-id="518d3-103">Per impostare solleciti di consegna</span><span class="sxs-lookup"><span data-stu-id="518d3-103">To set up delivery reminders</span></span>  

1. <span data-ttu-id="518d3-104">Scegliere l'![icona a forma di lampadina che consente di aprire la funzionalità delle informazioni](../../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Setup contabilità fornitori e acquisti** e quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="518d3-104">Choose the ![Lightbulb that opens the Tell Me feature](../../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchases & Payables Setup**, and then choose the related link.</span></span>  
2. <span data-ttu-id="518d3-105">Nel campo **Data sollecito eliminato di default** specificare una delle opzioni come descritto nella seguente tabella.</span><span class="sxs-lookup"><span data-stu-id="518d3-105">In the **Default Del. Rem. Date Field** field, specify one of the options described in the following table.</span></span>  

    |<span data-ttu-id="518d3-106">Opzione</span><span class="sxs-lookup"><span data-stu-id="518d3-106">Option</span></span>|<span data-ttu-id="518d3-107">Description</span><span class="sxs-lookup"><span data-stu-id="518d3-107">Description</span></span>|  
    |----------------------------------|---------------------------------------|  
    |<span data-ttu-id="518d3-108">**Data di carico richiesta**</span><span class="sxs-lookup"><span data-stu-id="518d3-108">**Requested Receipt Date**</span></span>|<span data-ttu-id="518d3-109">Specifica che il valore della data nel campo **Data di carico richiesta** sulla riga ordine di acquisto verrà usato come data di default per la creazione di solleciti di consegna.</span><span class="sxs-lookup"><span data-stu-id="518d3-109">Specifies that the date value in the **Requested Receipt Date** field on the purchase order line will be used as the default date for creating delivery reminders.</span></span>|  
    |<span data-ttu-id="518d3-110">**Data di carico promessa**</span><span class="sxs-lookup"><span data-stu-id="518d3-110">**Promised Receipt Date**</span></span>|<span data-ttu-id="518d3-111">Specifica che il valore della data nel campo **Data di carico promessa** sulla riga ordine di acquisto verrà usato come data di default per la creazione di solleciti di consegna.</span><span class="sxs-lookup"><span data-stu-id="518d3-111">Specifies that the date value in the **Promised Receipt Date** field on the purchase order line will be used as the default date for creating delivery reminders.</span></span>|  
    |<span data-ttu-id="518d3-112">**Data carico prevista**</span><span class="sxs-lookup"><span data-stu-id="518d3-112">**Expected Receipt Date**</span></span>|<span data-ttu-id="518d3-113">Specifica che il valore della data nel campo **Data carico prevista** sulla riga ordine di acquisto verrà usato come data di default per la creazione di solleciti di consegna.</span><span class="sxs-lookup"><span data-stu-id="518d3-113">Specifies that the date value in the **Expected Receipt Date** field on the purchase order line will be used as the default date for creating delivery reminders.</span></span>|  

3. <span data-ttu-id="518d3-114">Compilare i campi aggiuntivi come indicato nella tabella seguente.</span><span class="sxs-lookup"><span data-stu-id="518d3-114">Fill in additional fields as described in the following table.</span></span>  

    |<span data-ttu-id="518d3-115">Campo</span><span class="sxs-lookup"><span data-stu-id="518d3-115">Field</span></span>|<span data-ttu-id="518d3-116">Description</span><span class="sxs-lookup"><span data-stu-id="518d3-116">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="518d3-117">**Nr. Solleciti Consegna**</span><span class="sxs-lookup"><span data-stu-id="518d3-117">**Delivery Reminder Nos.**</span></span>|<span data-ttu-id="518d3-118">Codice numerazione per i solleciti di consegna.</span><span class="sxs-lookup"><span data-stu-id="518d3-118">The number series code for delivery reminders.</span></span>|  
    |<span data-ttu-id="518d3-119">**Nr. Solleciti Consegna Emessi**</span><span class="sxs-lookup"><span data-stu-id="518d3-119">**Issued Delivery Reminder Nos.**</span></span>|<span data-ttu-id="518d3-120">Codice numerazione per i solleciti di consegna inviati.</span><span class="sxs-lookup"><span data-stu-id="518d3-120">The number series code for issued delivery reminders.</span></span>|  

4. <span data-ttu-id="518d3-121">Scegliere il pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="518d3-121">Choose the **OK** button.</span></span>  
