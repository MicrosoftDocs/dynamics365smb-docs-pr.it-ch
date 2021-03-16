---
title: Come rettificare i tassi di cambio
description: Se è presente una vendita imponibile in una valuta estera, è necessario usare il tasso ufficiale per la conversione di valuta IVA, come definito dall'ente Federal Tax Administration.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 2602da964ece7e2b5c9d2563ef7807dbe2d2cc3b
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 02/15/2021
ms.locfileid: "5384015"
---
# <a name="adjust-exchange-rates"></a><span data-ttu-id="e307c-103">Rettifica tassi di cambio</span><span class="sxs-lookup"><span data-stu-id="e307c-103">Adjust Exchange Rates</span></span>
<span data-ttu-id="e307c-104">Se è presente una vendita imponibile in una valuta estera, è necessario usare il tasso ufficiale per la conversione di valuta IVA, come definito dall'ente Federal Tax Administration.</span><span class="sxs-lookup"><span data-stu-id="e307c-104">If you have taxable sales in a foreign currency, you must use the official rate for VAT currency conversion as set by the Federal Tax Administration.</span></span>  

<span data-ttu-id="e307c-105">Se tali tassi non corrispondono ai tassi di valuta usati nelle fatture di acquisto o di vendita, in seguito sarà necessario rettificare le aliquote IVA con un processo batch.</span><span class="sxs-lookup"><span data-stu-id="e307c-105">If these rates do not match the currency rates used in the purchase or sales invoices, you will have to adjust the VAT rates with a batch job later.</span></span> <span data-ttu-id="e307c-106">Tali rettifiche possono essere eseguite solo tramite un'aliquota IVA autorizzata.</span><span class="sxs-lookup"><span data-stu-id="e307c-106">These adjustments can only be run using an authorized VAT rate.</span></span>  

<span data-ttu-id="e307c-107">È possibile eseguire questo processo batch ogni volta che si desidera, purché si verifichi di eseguirlo sempre prima di creare una dichiarazione IVA.</span><span class="sxs-lookup"><span data-stu-id="e307c-107">You can run this batch job as often as you like, however make sure that you always run it before creating a VAT statement.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="e307c-108">Quando si usa una valuta contabile, verificare che il campo **Rettif. tasso di cambio IVA** nella pagina **Setup contabilità generale** sia impostato su **Nessuna rettifica**.</span><span class="sxs-lookup"><span data-stu-id="e307c-108">When using a report currency, make sure that the **VAT Exchange Rate Adjustment** field on the **General Ledger Setup** page is set to **No Adjustment**.</span></span>  

<span data-ttu-id="e307c-109">Per ulteriori informazioni sulla valute IVA ed estere, vedere il sito Web [ESTV](https://go.microsoft.com/fwlink/?LinkId=285999).</span><span class="sxs-lookup"><span data-stu-id="e307c-109">For more information about VAT and foreign currencies, see the [ESTV](https://go.microsoft.com/fwlink/?LinkId=285999) website.</span></span>  

## <a name="to-adjust-an-exchange-rate"></a><span data-ttu-id="e307c-110">Per rettificare un tasso di cambio</span><span class="sxs-lookup"><span data-stu-id="e307c-110">To adjust an exchange rate</span></span>  

1.  <span data-ttu-id="e307c-111">Scegliere l'![icona a forma di lampadina che consente di aprire la funzionalità delle informazioni](../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Valute** e quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="e307c-111">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Currencies**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="e307c-112">Scegliere l'azione **Tassi di cambio**.</span><span class="sxs-lookup"><span data-stu-id="e307c-112">Choose the **Exch. Rates** action.</span></span>  
3.  <span data-ttu-id="e307c-113">Nella pagina **Tassi di cambio valuta** immettere l'aliquota IVA ufficiale per periodo per ogni valuta nei campi **Importo tasso di cambio IVA** e **Importo tasso di cambio IVA relazionale**.</span><span class="sxs-lookup"><span data-stu-id="e307c-113">On the **Currency Exchange Rates** page, enter the official VAT rate per period for each currency in the **VAT Exch. Rate Amount** and the **Relational VAT Exch. Rate Amt** fields.</span></span>  
4.  <span data-ttu-id="e307c-114">Scegliere il pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="e307c-114">Choose the **OK** button.</span></span>  
5.  <span data-ttu-id="e307c-115">Scegliere l'![icona a forma di lampadina che consente di aprire la funzionalità delle informazioni](../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Rettifica tassi di cambio** e quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="e307c-115">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Adjust Exchange Rates**, and then choose the related link.</span></span>  
6.  <span data-ttu-id="e307c-116">Nella Scheda dettaglio **Opzioni** compilare i campi come descritto nella tabella riportata di seguito.</span><span class="sxs-lookup"><span data-stu-id="e307c-116">On the **Options** FastTab, fill in the fields as described in the following table.</span></span>   

    |<span data-ttu-id="e307c-117">Campo</span><span class="sxs-lookup"><span data-stu-id="e307c-117">Field</span></span>|<span data-ttu-id="e307c-118">Descrizione</span><span class="sxs-lookup"><span data-stu-id="e307c-118">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="e307c-119">**Data inizio**</span><span class="sxs-lookup"><span data-stu-id="e307c-119">**Starting Date**</span></span>|<span data-ttu-id="e307c-120">Immettere una data per specificare l'inizio del periodo per cui verranno rettificati i movimenti.</span><span class="sxs-lookup"><span data-stu-id="e307c-120">Enter a date to specify the beginning of the period for which entries will be adjusted.</span></span>|  
    |<span data-ttu-id="e307c-121">**Data fine**</span><span class="sxs-lookup"><span data-stu-id="e307c-121">**Ending Date**</span></span>|<span data-ttu-id="e307c-122">Immettere la data finale per la quale i movimenti verranno rettificati.</span><span class="sxs-lookup"><span data-stu-id="e307c-122">Enter the last date for which entries will be adjusted.</span></span> <span data-ttu-id="e307c-123">Solitamente questa data equivale alla data di registrazione indicata nel campo **Data di registrazione**.</span><span class="sxs-lookup"><span data-stu-id="e307c-123">This date is typically the same as the posting date in the **Posting Date** field.</span></span>|  
    |<span data-ttu-id="e307c-124">**Rettifica cambio per ammin. IVA**</span><span class="sxs-lookup"><span data-stu-id="e307c-124">**Adjust VAT exch. rate**</span></span>|<span data-ttu-id="e307c-125">Specificare se si desidera rettificare il tasso di cambio IVA.</span><span class="sxs-lookup"><span data-stu-id="e307c-125">Specify if you want to adjust the VAT exchange rate.</span></span>|  

7.  <span data-ttu-id="e307c-126">Scegliere **Stampa** per avviare il processo batch.</span><span class="sxs-lookup"><span data-stu-id="e307c-126">Choose the **Print** button to start the batch job.</span></span> <span data-ttu-id="e307c-127">Il processo batch controlla se i movimenti IVA devono essere rettificati e prepara un movimento di rettifica per ciascuno di tali movimenti per i conti di rettifica del tasso di cambio per IVA a esigibilità immediata o differita.</span><span class="sxs-lookup"><span data-stu-id="e307c-127">This batch job controls whether VAT entries have to be adjusted and prepares an adjusting entry for each of these entries for the Unrealized/Realized Exchange Rate Adjustment accounts.</span></span> <span data-ttu-id="e307c-128">Vengono rettificati anche i movimenti IVA esistenti.</span><span class="sxs-lookup"><span data-stu-id="e307c-128">The existing VAT entries are also corrected.</span></span>  

## <a name="see-also"></a><span data-ttu-id="e307c-129">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="e307c-129">See Also</span></span>  
 <span data-ttu-id="e307c-130">[IVA svizzera](swiss-value-added-tax.md) </span><span class="sxs-lookup"><span data-stu-id="e307c-130">[Swiss Value Added Tax](swiss-value-added-tax.md) </span></span>  
 <span data-ttu-id="e307c-131">[Aliquote IVA per la Svizzera](vat-rates-for-switzerland.md) </span><span class="sxs-lookup"><span data-stu-id="e307c-131">[VAT Rates for Switzerland](vat-rates-for-switzerland.md) </span></span>  
[<span data-ttu-id="e307c-132">Aggiornare i tassi di cambio valuta</span><span class="sxs-lookup"><span data-stu-id="e307c-132">Update Currency Exchange Rates</span></span>](../../finance-how-update-currencies.md)  
[<span data-ttu-id="e307c-133">Impostare una valuta contabile addizionale</span><span class="sxs-lookup"><span data-stu-id="e307c-133">Set Up an Additional Reporting Currency</span></span>](../../finance-how-setup-additional-currencies.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]