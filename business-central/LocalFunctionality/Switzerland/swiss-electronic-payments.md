---
title: Pagamenti elettronici svizzeri
description: I miglioramenti svizzeri consentono di inviare le fatture ai clienti elettronicamente. Le fatture vengono presentate e pagate direttamente utilizzando il software bancario online del cliente.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: 9cc447cd05718eb7cadb6ddb13bbe0e0584b17cd
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 03/31/2019
ms.locfileid: "917811"
---
# <a name="swiss-electronic-payments"></a><span data-ttu-id="39650-104">Pagamenti elettronici svizzeri</span><span class="sxs-lookup"><span data-stu-id="39650-104">Swiss Electronic Payments</span></span>
[!INCLUDE[d365fin](../../includes/d365fin_md.md)] <span data-ttu-id="39650-105">consente di inviare le fatture ai clienti elettronicamente.</span><span class="sxs-lookup"><span data-stu-id="39650-105">allows you to send invoices to customers electronically.</span></span> <span data-ttu-id="39650-106">Le fatture vengono presentate e pagate direttamente utilizzando il software bancario online del cliente.</span><span class="sxs-lookup"><span data-stu-id="39650-106">The invoices are presented and paid directly using the customer's online banking software.</span></span>  

## <a name="electronic-payment-methods"></a><span data-ttu-id="39650-107">Metodi di pagamento elettronico</span><span class="sxs-lookup"><span data-stu-id="39650-107">Electronic Payment Methods</span></span>  
<span data-ttu-id="39650-108">È possibile effettuare pagamenti elettronici utilizzando i seguenti metodi:</span><span class="sxs-lookup"><span data-stu-id="39650-108">You can make electronic payments using the following methods:</span></span>  

- <span data-ttu-id="39650-109">Einzahlungsschein mit Referenznummer (ESR)</span><span class="sxs-lookup"><span data-stu-id="39650-109">Einzahlungsschein mit Referenznummer (ESR)</span></span>  
- <span data-ttu-id="39650-110">Lastschrift Verfahren (LSV+)</span><span class="sxs-lookup"><span data-stu-id="39650-110">Lastschrift Verfahren (LSV+)</span></span>  
- <span data-ttu-id="39650-111">Bonifici SEPA</span><span class="sxs-lookup"><span data-stu-id="39650-111">SEPA credit transfers</span></span>  

## <a name="esr"></a><span data-ttu-id="39650-112">ESR</span><span class="sxs-lookup"><span data-stu-id="39650-112">ESR</span></span>  
<span data-ttu-id="39650-113">ESR è un servizio debitore elettronico che utilizza distinte di pagamento per riscuotere fondi.</span><span class="sxs-lookup"><span data-stu-id="39650-113">ESR is an electronic debtor service that uses payment slips to collect money.</span></span> <span data-ttu-id="39650-114">È il sistema di pagamento elettronico standard creato da Swiss Post.</span><span class="sxs-lookup"><span data-stu-id="39650-114">It is the standard electronic payment system created by Swiss Post.</span></span> <span data-ttu-id="39650-115">È possibile stampare le distinte di pagamento ESR come allegati a fattura, calcolare i numeri di riferimento ESR e importare file ESR che hanno informazioni di pagamento delle banche.</span><span class="sxs-lookup"><span data-stu-id="39650-115">You can print ESR payment slips as invoice attachments, calculate ESR reference numbers, and import ESR files that have payment information from banks.</span></span> <span data-ttu-id="39650-116">Per ulteriori informazioni, vedere [Pagamenti elettronici svizzeri tramite ESR](how-to-print-esr-invoices.md).</span><span class="sxs-lookup"><span data-stu-id="39650-116">For more information, see [Swiss Electronic Payments Using ESR](how-to-print-esr-invoices.md).</span></span> <span data-ttu-id="39650-117">Inoltre, è possibile effettuare pagamenti ESR e ESR+ utilizzando la versione della banca di questo metodo di pagamento denominato Bank-ESR (BESR).</span><span class="sxs-lookup"><span data-stu-id="39650-117">You can also make ESR and ESR+ payments using the bank’s version of this payment method, which is named Bank-ESR (BESR).</span></span>  

## <a name="lsv"></a><span data-ttu-id="39650-118">LSV+</span><span class="sxs-lookup"><span data-stu-id="39650-118">LSV+</span></span>  
<span data-ttu-id="39650-119">LSV+ è un servizio di addebito diretto che viene utilizzato per l'elaborazione dei pagamenti.</span><span class="sxs-lookup"><span data-stu-id="39650-119">LSV+ is a direct debit service that is used for processing payments.</span></span> <span data-ttu-id="39650-120">Le aziende possono rilasciare i pagamenti dei clienti direttamente dalla banca del cliente utilizzando l'addebito diretto.</span><span class="sxs-lookup"><span data-stu-id="39650-120">Companies can release customer payments directly from the customer's bank using direct debit.</span></span> <span data-ttu-id="39650-121">È possibile richiedere e riscuotere i pagamenti dei clienti utilizzando l'addebito diretto nel formato bancario LSV+ o nel formato DebitDirect PostFinance.</span><span class="sxs-lookup"><span data-stu-id="39650-121">You can request and collect customer payments using direct debit in the LSV+ bank format, or in the DebitDirect PostFinance format.</span></span> <span data-ttu-id="39650-122">Per ulteriori informazioni, vedere [Pagamenti elettronici svizzeri tramite LSV+](swiss-electronic-payments-using-lsv-.md).</span><span class="sxs-lookup"><span data-stu-id="39650-122">For more information, see [Swiss Electronic Payments Using LSV+](swiss-electronic-payments-using-lsv-.md).</span></span>  

## <a name="sepa-credit-transfers"></a><span data-ttu-id="39650-123">Bonifici SEPA</span><span class="sxs-lookup"><span data-stu-id="39650-123">SEPA Credit Transfers</span></span>  
<span data-ttu-id="39650-124">Per esportare i pagamenti secondo lo standard SEPA, è necessario utilizzare un conto bancario.</span><span class="sxs-lookup"><span data-stu-id="39650-124">To export payments according to the SEPA standard, you must use a bank account.</span></span> <span data-ttu-id="39650-125">Per assicurarsi che i movimenti contabili corrispondenti siano coerenti con quelli generati per i metodi di pagamento svizzeri locali (vedere sopra), il valore nel campo **Cat. reg. C/C bancario** della pagina **Scheda conto corrente bancario** deve indicare il relativo conto C/G.</span><span class="sxs-lookup"><span data-stu-id="39650-125">To make sure that the related general ledger entries are consistent with those generated for local Swiss payment methods (see above), the value in the **Bank Acc. Posting Group** field on the **Bank Account Card** page must point to the relevant general ledger account.</span></span> <span data-ttu-id="39650-126">Per ulteriori informazioni su come esportare i pagamenti SEPA, vedere [Creare movimenti riscossione addebiti diretti SEPA ed esportarli in un file della banca](../../finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md).</span><span class="sxs-lookup"><span data-stu-id="39650-126">For more information about how to export SEPA payments, see [Create SEPA Direct Debit Collection Entries and Export to a Bank File](../../finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="39650-127">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="39650-127">See Also</span></span>  
 <span data-ttu-id="39650-128">[Importare numeri di clearing svizzeri](how-to-import-swiss-bank-clearing-numbers.md) </span><span class="sxs-lookup"><span data-stu-id="39650-128">[Import Swiss Bank Clearing Numbers](how-to-import-swiss-bank-clearing-numbers.md) </span></span>  
 <span data-ttu-id="39650-129">[Pagamenti elettronici svizzeri tramite ESR](swiss-electronic-payments-using-esr.md) </span><span class="sxs-lookup"><span data-stu-id="39650-129">[Swiss Electronic Payments Using ESR](swiss-electronic-payments-using-esr.md) </span></span>  
 <span data-ttu-id="39650-130">[Stampare fatture ESR](how-to-print-esr-invoices.md) </span><span class="sxs-lookup"><span data-stu-id="39650-130">[Print ESR Invoices](how-to-print-esr-invoices.md) </span></span>  
 <span data-ttu-id="39650-131">[Pagamenti elettronici svizzeri tramite LSV+](swiss-electronic-payments-using-lsv-.md) </span><span class="sxs-lookup"><span data-stu-id="39650-131">[Swiss Electronic Payments Using LSV+](swiss-electronic-payments-using-lsv-.md) </span></span>  
 <span data-ttu-id="39650-132">[Funzionalità locale per la Svizzera](switzerland-local-functionality.md)  ' [Creare movimenti riscossione addebiti diretti SEPA ed esportarli in un file della banca](../../finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md)</span><span class="sxs-lookup"><span data-stu-id="39650-132">[Switzerland Local Functionality](switzerland-local-functionality.md)  ' [Create SEPA Direct Debit Collection Entries and Export to a Bank File](../../finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md)</span></span>  
 [<span data-ttu-id="39650-133">Effettuare i pagamenti</span><span class="sxs-lookup"><span data-stu-id="39650-133">Making Payments</span></span>](../../payables-make-payments.md)
