---
title: Gestione del magazzino per la Svizzera
description: I miglioramenti svizzeri includono funzioni speciali di gestione magazzino.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 31830644e2de5878b5e5b383aade8ef4864b0291
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 02/15/2021
ms.locfileid: "5382687"
---
# <a name="swiss-inventory-management"></a><span data-ttu-id="ba313-103">Gestione del magazzino per la Svizzera</span><span class="sxs-lookup"><span data-stu-id="ba313-103">Swiss Inventory Management</span></span>
[!INCLUDE[prod_short](../../includes/prod_short.md)] <span data-ttu-id="ba313-104">include i miglioramenti svizzeri per la gestione magazzino.</span><span class="sxs-lookup"><span data-stu-id="ba313-104">includes Swiss enhancements to inventory management.</span></span> <span data-ttu-id="ba313-105">È incluso quanto segue:</span><span class="sxs-lookup"><span data-stu-id="ba313-105">This includes the following:</span></span>  

- <span data-ttu-id="ba313-106">Dichiarazione dettagliata.</span><span class="sxs-lookup"><span data-stu-id="ba313-106">Detailed reporting.</span></span>  <span data-ttu-id="ba313-107">Per ulteriori informazioni vedere il report Magazzino - Statistiche di vendita e il report Magazzino - Lista.</span><span class="sxs-lookup"><span data-stu-id="ba313-107">For more information, see the Inventory - Sales Statistics report and the Inventory - List report.</span></span>  
- <span data-ttu-id="ba313-108">La capacità di monitorare una fattura con più spedizioni.</span><span class="sxs-lookup"><span data-stu-id="ba313-108">The ability to track an invoice with multiple shipments.</span></span>  
- <span data-ttu-id="ba313-109">L'inclusione di un codice ubicazione scheda articolo come il codice ubicazione predefinito per le righe di vendita e le registrazioni articoli.</span><span class="sxs-lookup"><span data-stu-id="ba313-109">Including an item card location code as the default location code for sales lines and item journals.</span></span> <span data-ttu-id="ba313-110">Per ulteriori informazioni, vedere [Impostare le ubicazioni](../../inventory-how-setup-locations.md).</span><span class="sxs-lookup"><span data-stu-id="ba313-110">For more information, see [Set Up Locations](../../inventory-how-setup-locations.md).</span></span>

## <a name="managing-item-details"></a><span data-ttu-id="ba313-111">Gestione dettagli articolo</span><span class="sxs-lookup"><span data-stu-id="ba313-111">Managing Item Details</span></span>  
<span data-ttu-id="ba313-112">Le aziende possono disporre di magazzini diversi per categorie di prodotti diversi.</span><span class="sxs-lookup"><span data-stu-id="ba313-112">Companies can have different warehouses for different product categories.</span></span> <span data-ttu-id="ba313-113">In questi casi, è necessario utilizzare il codice ubicazione predefinito recuperato dalla scheda articolo.</span><span class="sxs-lookup"><span data-stu-id="ba313-113">In such cases, you must use the default location code retrieved from the item card.</span></span> <span data-ttu-id="ba313-114">Quando si definisce un codice ubicazione per un articolo, questo viene trasferito nelle righe di vendita e nelle registrazioni articoli come codice di ubicazione articoli predefinito.</span><span class="sxs-lookup"><span data-stu-id="ba313-114">When you define a location code for an item, it is transferred to the sales lines and item journals as a default item location code.</span></span> <span data-ttu-id="ba313-115">Per ulteriori informazioni, vedere le tabelle Righe vendite e Righe reg. magazzino.</span><span class="sxs-lookup"><span data-stu-id="ba313-115">For more information, see the Sales Line and the Item Journal Line table.</span></span>  

<span data-ttu-id="ba313-116">Ulteriori informazioni, come il numero cliente, il codice dell'indirizzo di spedizione e il codice venditore del cliente, vengono memorizzate nei movimenti contabili articoli.</span><span class="sxs-lookup"><span data-stu-id="ba313-116">Additional information, such as customer number, ship-to address code, and customer sales person code, is stored in item ledger entries.</span></span> <span data-ttu-id="ba313-117">Queste informazioni consentono di creare criteri di dichiarazione personalizzati, come i ricavi per cliente e gli accantonamenti per articoli o vendite per i venditori.</span><span class="sxs-lookup"><span data-stu-id="ba313-117">This information helps you to create customized reporting criteria, such as revenue per customer, and item or sales provisions for sales people.</span></span> <span data-ttu-id="ba313-118">Per ulteriori informazioni, vedere la tabella Mov. contabili articoli.</span><span class="sxs-lookup"><span data-stu-id="ba313-118">For more information, see the Item Ledger Entry table.</span></span>  

## <a name="invoices-with-multiple-shipments"></a><span data-ttu-id="ba313-119">Fatture con più spedizioni</span><span class="sxs-lookup"><span data-stu-id="ba313-119">Invoices with Multiple Shipments</span></span>  
<span data-ttu-id="ba313-120">Se sono state registrate più spedizioni per un cliente, è possibile creare una fattura combinata con la funzione **Prendi righe di spedizione**.</span><span class="sxs-lookup"><span data-stu-id="ba313-120">If multiple shipments have been posted for a customer, then you can create a combined invoice with the **Get Shipment Lines** function.</span></span> <span data-ttu-id="ba313-121">Per ulteriori informazioni, vedere la pagina Prendi righe di spedizione.</span><span class="sxs-lookup"><span data-stu-id="ba313-121">For more information, see the Get Shipment Lines page.</span></span> <span data-ttu-id="ba313-122">Quando si utilizza questa funzione, il testo creato nelle righe della fattura include informazioni sul numero di spedizione e sulla data di spedizione.</span><span class="sxs-lookup"><span data-stu-id="ba313-122">When you use this function, the text created on the invoice lines includes information about the shipment number and the shipment date.</span></span> <span data-ttu-id="ba313-123">Ad esempio, il testo potrebbe essere Nr. spedizione</span><span class="sxs-lookup"><span data-stu-id="ba313-123">For example, the text could appear as Shipment No.</span></span> <span data-ttu-id="ba313-124">102040 di 25.01.01.</span><span class="sxs-lookup"><span data-stu-id="ba313-124">102040 of 25.01.01.</span></span> <span data-ttu-id="ba313-125">Ciò consente di tracciare facilmente le fatture con più spedizioni.</span><span class="sxs-lookup"><span data-stu-id="ba313-125">This allows you to easily track invoices with multiple shipments.</span></span>  

## <a name="see-also"></a><span data-ttu-id="ba313-126">Vedere anche</span><span class="sxs-lookup"><span data-stu-id="ba313-126">See Also</span></span>  
 <span data-ttu-id="ba313-127">[Funzionalità locale per la Svizzera](switzerland-local-functionality.md) </span><span class="sxs-lookup"><span data-stu-id="ba313-127">[Switzerland Local Functionality](switzerland-local-functionality.md) </span></span>  
 [<span data-ttu-id="ba313-128">Impostare le ubicazioni</span><span class="sxs-lookup"><span data-stu-id="ba313-128">Set Up Locations</span></span>](../../inventory-how-setup-locations.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]