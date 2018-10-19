---
title: IVA svizzera
description: I miglioramenti svizzeri includono funzioni speciali di dichiarazione IVA.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 66ac3a70ee4f40ab1b4c86afcc8ad28357c7a543
ms.contentlocale: it-ch
ms.lasthandoff: 09/28/2018

---
# <a name="swiss-value-added-tax"></a><span data-ttu-id="b0a18-103">IVA svizzera</span><span class="sxs-lookup"><span data-stu-id="b0a18-103">Swiss Value Added Tax</span></span>
[!INCLUDE[d365fin](../../includes/d365fin_md.md)] <span data-ttu-id="b0a18-104">includono i seguenti miglioramenti alla dichiarazione IVA svizzera:</span><span class="sxs-lookup"><span data-stu-id="b0a18-104">includes the following enhancements to Swiss VAT reporting:</span></span>  

- <span data-ttu-id="b0a18-105">Rettifica automatica degli importi IVA per fatture, in base agli sconti di pagamento.</span><span class="sxs-lookup"><span data-stu-id="b0a18-105">Automatic adjustment of VAT amounts for invoices, according to payment discounts.</span></span>  
- <span data-ttu-id="b0a18-106">Tassi di cambio IVA aggiuntivi per le fatture in valute estere.</span><span class="sxs-lookup"><span data-stu-id="b0a18-106">Additional VAT exchange rates for invoices in foreign currencies.</span></span>  

<span data-ttu-id="b0a18-107">Per ulteriori informazioni sui requisiti di codifica a reporting dell'IVA svizzera, vedi [Informazioni sull'IVA svizzera](https://www.estv.admin.ch/estv/en/home.html).</span><span class="sxs-lookup"><span data-stu-id="b0a18-107">For more information about Swiss VAT reporting and coding requirements, see [Swiss VAT Information](https://www.estv.admin.ch/estv/en/home.html).</span></span> <span data-ttu-id="b0a18-108">Le informazioni sono disponibili in francese, tedesco e italiano.</span><span class="sxs-lookup"><span data-stu-id="b0a18-108">The information is available in French, German, and Italian.</span></span>  

## <a name="vat-amounts-and-vat-exchange-rates"></a><span data-ttu-id="b0a18-109">Importi IVA e tassi di cambio IVA</span><span class="sxs-lookup"><span data-stu-id="b0a18-109">VAT Amounts and VAT Exchange Rates</span></span>  
<span data-ttu-id="b0a18-110">Secondo le leggi locali dell'IVA, l'importo base dell'IVA per una fattura può essere ridotto dello sconto di pagamento se viene concesso uno sconto.</span><span class="sxs-lookup"><span data-stu-id="b0a18-110">According to local VAT laws, the VAT base amount for an invoice can be reduced by the payment discount if a discount is granted.</span></span> <span data-ttu-id="b0a18-111">Per consentire la rettifica automatica dell'IVA per uno sconto di pagamento su una fattura, il campo **Rettifica per sconto pagamento** viene attivato per impostazione predefinita nella finestra **Setup contabilità generale**.</span><span class="sxs-lookup"><span data-stu-id="b0a18-111">To allow automatic VAT adjustment for a payment discount on an invoice, the **Adjust for Payment Discount** field is activated by default in the **General Ledger Setup** window.</span></span> <span data-ttu-id="b0a18-112">È anche possibile attivare questa funzione nel setup registrazioni IVA.</span><span class="sxs-lookup"><span data-stu-id="b0a18-112">You can also activate this function in the VAT posting setup.</span></span> <span data-ttu-id="b0a18-113">Per ulteriori informazioni, vedere la tabella Setup contabilità generale e Setup registrazioni IVA.</span><span class="sxs-lookup"><span data-stu-id="b0a18-113">For more information, see the General Ledger Setup table and the VAT Posting Setup table.</span></span>  

### <a name="currency-exchange-rates-for-vat-reporting"></a><span data-ttu-id="b0a18-114">Tassi di cambio valuta per dichiarazione IVA </span><span class="sxs-lookup"><span data-stu-id="b0a18-114">Currency Exchange Rates for VAT Reporting</span></span>  
<span data-ttu-id="b0a18-115">Per le fatture in valuta estera è necessario utilizzare il tasso di cambio ufficiale fornito dal governo per il calcolo dell'IVA.</span><span class="sxs-lookup"><span data-stu-id="b0a18-115">For invoices in foreign currency, you must use the official exchange rate provided by the government for the VAT calculation itself.</span></span> <span data-ttu-id="b0a18-116">È inoltre possibile impostare ulteriori tassi di cambio per l'IVA, che è possibile utilizzare per aspetti della fattura diversi dal calcolo dell'IVA.</span><span class="sxs-lookup"><span data-stu-id="b0a18-116">You can also set up additional exchange rates for VAT, which you can use for aspects of the invoice other than the VAT calculation.</span></span> <span data-ttu-id="b0a18-117">È possibile fornire il corretto tasso di cambio dell'IVA di governo per ogni valuta estera rilevante nel setup dei tassi di cambio per le fatture.</span><span class="sxs-lookup"><span data-stu-id="b0a18-117">You can provide the correct government VAT exchange rate for each relevant foreign currency in the exchange rate setup for invoices.</span></span> <span data-ttu-id="b0a18-118">Per ulteriori informazioni, vedere la tabella Tassi di cambio valute.</span><span class="sxs-lookup"><span data-stu-id="b0a18-118">For more information, see the Currency Exchange Rate table.</span></span>  

<span data-ttu-id="b0a18-119">È inoltre possibile rettificare tutti gli importi IVA nei movimenti IVA risultanti da transazioni in valuta estera.</span><span class="sxs-lookup"><span data-stu-id="b0a18-119">You can also adjust all VAT amounts in VAT entries that result from foreign currency transactions.</span></span> <span data-ttu-id="b0a18-120">Quando si attiva la funzione di rettifica del tasso di cambio IVA, i tassi di cambio IVA vengono rettificati automaticamente.</span><span class="sxs-lookup"><span data-stu-id="b0a18-120">When you activate the adjust VAT exchange rate function, VAT exchange rates are adjusted automatically.</span></span> <span data-ttu-id="b0a18-121">Le differenze positive derivanti dai tassi di cambio sono registrate in conti di utili di conversione.</span><span class="sxs-lookup"><span data-stu-id="b0a18-121">The positive differences that result from exchange rates are posted to exchange rate gain accounts.</span></span> <span data-ttu-id="b0a18-122">Le differenze negative derivanti dai tassi di cambio sono registrate in conti di perdite di conversione.</span><span class="sxs-lookup"><span data-stu-id="b0a18-122">The negative differences that result from exchange rates are posted to exchange rate loss accounts.</span></span> <span data-ttu-id="b0a18-123">Per ulteriori informazioni, vedere il processo batch Rettifica tassi di cambio.</span><span class="sxs-lookup"><span data-stu-id="b0a18-123">For more information, see the Adjust Exchange Rates batch job.</span></span>  

<span data-ttu-id="b0a18-124">Ulteriori informazioni, come l'aliquota IVA e l'importo in valuta originale, vengono trasferiti ai movimenti IVA.</span><span class="sxs-lookup"><span data-stu-id="b0a18-124">Additional information, such as VAT rate and original currency amount, is transferred to the VAT entries.</span></span> <span data-ttu-id="b0a18-125">Per ulteriori informazioni, vedere la tabella Movimenti IVA.</span><span class="sxs-lookup"><span data-stu-id="b0a18-125">For more information, see the VAT Entry table.</span></span>  

## <a name="see-also"></a><span data-ttu-id="b0a18-126">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="b0a18-126">See Also</span></span>  
 <span data-ttu-id="b0a18-127">[Aliquote IVA per la Svizzera](vat-rates-for-switzerland.md) </span><span class="sxs-lookup"><span data-stu-id="b0a18-127">[VAT Rates for Switzerland](vat-rates-for-switzerland.md) </span></span>  
 <span data-ttu-id="b0a18-128">[Creare e stampare una dichiarazione IVA svizzera](how-to-create-and-print-a-swiss-vat-statement.md) </span><span class="sxs-lookup"><span data-stu-id="b0a18-128">[Create and Print a Swiss VAT Statement](how-to-create-and-print-a-swiss-vat-statement.md) </span></span>  
 [<span data-ttu-id="b0a18-129">Funzionalità locale per la Svizzera</span><span class="sxs-lookup"><span data-stu-id="b0a18-129">Switzerland Local Functionality</span></span>](switzerland-local-functionality.md)   

