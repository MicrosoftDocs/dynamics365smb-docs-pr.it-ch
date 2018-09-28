---
title: Pagamenti elettronici svizzeri
description: I miglioramenti svizzeri consentono di inviare le fatture ai clienti elettronicamente. Le fatture vengono presentate e pagate direttamente utilizzando il software bancario online del cliente.
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
ms.openlocfilehash: 282f9c9b2245b8d989eed7a564b8bddff2234c1d
ms.contentlocale: it-ch
ms.lasthandoff: 09/28/2018

---
# <a name="swiss-electronic-payments"></a><span data-ttu-id="722dc-104">Pagamenti elettronici svizzeri</span><span class="sxs-lookup"><span data-stu-id="722dc-104">Swiss Electronic Payments</span></span>
[!INCLUDE[d365fin](../../includes/d365fin_md.md)] <span data-ttu-id="722dc-105">consente di inviare le fatture ai clienti elettronicamente.</span><span class="sxs-lookup"><span data-stu-id="722dc-105"> allows you to send invoices to customers electronically.</span></span> <span data-ttu-id="722dc-106">Le fatture vengono presentate e pagate direttamente utilizzando il software bancario online del cliente.</span><span class="sxs-lookup"><span data-stu-id="722dc-106">The invoices are presented and paid directly using the customer's online banking software.</span></span>  

## <a name="electronic-payment-methods"></a><span data-ttu-id="722dc-107">Metodi di pagamento elettronico</span><span class="sxs-lookup"><span data-stu-id="722dc-107">Electronic Payment Methods</span></span>  
<span data-ttu-id="722dc-108">È possibile effettuare pagamenti elettronici utilizzando i seguenti metodi:</span><span class="sxs-lookup"><span data-stu-id="722dc-108">You can make electronic payments using the following methods:</span></span>  

- <span data-ttu-id="722dc-109">Einzahlungsschein mit Referenznummer (ESR)</span><span class="sxs-lookup"><span data-stu-id="722dc-109">Einzahlungsschein mit Referenznummer (ESR)</span></span>  
- <span data-ttu-id="722dc-110">Lastschrift Verfahren (LSV+)</span><span class="sxs-lookup"><span data-stu-id="722dc-110">Lastschrift Verfahren (LSV+)</span></span>  
- <span data-ttu-id="722dc-111">Bonifici SEPA</span><span class="sxs-lookup"><span data-stu-id="722dc-111">SEPA credit transfers</span></span>  

## <a name="esr"></a><span data-ttu-id="722dc-112">ESR</span><span class="sxs-lookup"><span data-stu-id="722dc-112">ESR</span></span>  
<span data-ttu-id="722dc-113">ESR è un servizio debitore elettronico che utilizza distinte di pagamento per riscuotere fondi.</span><span class="sxs-lookup"><span data-stu-id="722dc-113">ESR is an electronic debtor service that uses payment slips to collect money.</span></span> <span data-ttu-id="722dc-114">È il sistema di pagamento elettronico standard creato da Swiss Post.</span><span class="sxs-lookup"><span data-stu-id="722dc-114">It is the standard electronic payment system created by Swiss Post.</span></span> <span data-ttu-id="722dc-115">È possibile stampare le distinte di pagamento ESR come allegati a fattura, calcolare i numeri di riferimento ESR e importare file ESR che hanno informazioni di pagamento delle banche.</span><span class="sxs-lookup"><span data-stu-id="722dc-115">You can print ESR payment slips as invoice attachments, calculate ESR reference numbers, and import ESR files that have payment information from banks.</span></span> <span data-ttu-id="722dc-116">Per ulteriori informazioni, vedere [Pagamenti elettronici svizzeri tramite ESR](how-to-print-esr-invoices.md).</span><span class="sxs-lookup"><span data-stu-id="722dc-116">For more information, see [Swiss Electronic Payments Using ESR](how-to-print-esr-invoices.md).</span></span> <span data-ttu-id="722dc-117">Inoltre, è possibile effettuare pagamenti ESR e ESR+ utilizzando la versione della banca di questo metodo di pagamento denominato Bank-ESR (BESR).</span><span class="sxs-lookup"><span data-stu-id="722dc-117">You can also make ESR and ESR+ payments using the bank’s version of this payment method, which is named Bank-ESR (BESR).</span></span>  

## <a name="lsv"></a><span data-ttu-id="722dc-118">LSV+</span><span class="sxs-lookup"><span data-stu-id="722dc-118">LSV+</span></span>  
<span data-ttu-id="722dc-119">LSV+ è un servizio di addebito diretto che viene utilizzato per l'elaborazione dei pagamenti.</span><span class="sxs-lookup"><span data-stu-id="722dc-119">LSV+ is a direct debit service that is used for processing payments.</span></span> <span data-ttu-id="722dc-120">Le aziende possono rilasciare i pagamenti dei clienti direttamente dalla banca del cliente utilizzando l'addebito diretto.</span><span class="sxs-lookup"><span data-stu-id="722dc-120">Companies can release customer payments directly from the customer's bank using direct debit.</span></span> <span data-ttu-id="722dc-121">È possibile richiedere e riscuotere i pagamenti dei clienti utilizzando l'addebito diretto nel formato bancario LSV+ o nel formato DebitDirect PostFinance.</span><span class="sxs-lookup"><span data-stu-id="722dc-121">You can request and collect customer payments using direct debit in the LSV+ bank format, or in the DebitDirect PostFinance format.</span></span> <span data-ttu-id="722dc-122">Per ulteriori informazioni, vedere [Pagamenti elettronici svizzeri tramite LSV+](swiss-electronic-payments-using-lsv-.md).</span><span class="sxs-lookup"><span data-stu-id="722dc-122">For more information, see [Swiss Electronic Payments Using LSV+](swiss-electronic-payments-using-lsv-.md).</span></span>  

## <a name="sepa-credit-transfers"></a><span data-ttu-id="722dc-123">Bonifici SEPA</span><span class="sxs-lookup"><span data-stu-id="722dc-123">SEPA Credit Transfers</span></span>  
<span data-ttu-id="722dc-124">Per esportare i pagamenti secondo lo standard SEPA, è necessario utilizzare un conto bancario.</span><span class="sxs-lookup"><span data-stu-id="722dc-124">To export payments according to the SEPA standard, you must use a bank account.</span></span> <span data-ttu-id="722dc-125">Per assicurarsi che i movimenti contabili corrispondenti siano coerenti con quelli generati per i metodi di pagamento svizzeri locali (vedere sopra), il valore nel campo **Cat. reg. C/C bancario** della finestra **Scheda conto corrente bancario** deve indicare il relativo conto C/G.</span><span class="sxs-lookup"><span data-stu-id="722dc-125">To make sure that the related general ledger entries are consistent with those generated for local Swiss payment methods (see above), the value in the **Bank Acc. Posting Group** field in the **Bank Account Card** window must point to the relevant general ledger account.</span></span> <span data-ttu-id="722dc-126">Per ulteriori informazioni su come esportare i pagamenti SEPA, vedere [Creare movimenti riscossione addebiti diretti SEPA ed esportarli in un file della banca](../../finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md).</span><span class="sxs-lookup"><span data-stu-id="722dc-126">For more information about how to export SEPA payments, see [Create SEPA Direct Debit Collection Entries and Export to a Bank File](../../finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="722dc-127">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="722dc-127">See Also</span></span>  
 <span data-ttu-id="722dc-128">[Importare numeri di clearing svizzeri](how-to-import-swiss-bank-clearing-numbers.md) </span><span class="sxs-lookup"><span data-stu-id="722dc-128">[Import Swiss Bank Clearing Numbers](how-to-import-swiss-bank-clearing-numbers.md) </span></span>  
 <span data-ttu-id="722dc-129">[Pagamenti elettronici svizzeri tramite ESR](swiss-electronic-payments-using-esr.md) </span><span class="sxs-lookup"><span data-stu-id="722dc-129">[Swiss Electronic Payments Using ESR](swiss-electronic-payments-using-esr.md) </span></span>  
 <span data-ttu-id="722dc-130">[Stampare fatture ESR](how-to-print-esr-invoices.md) </span><span class="sxs-lookup"><span data-stu-id="722dc-130">[Print ESR Invoices](how-to-print-esr-invoices.md) </span></span>  
 <span data-ttu-id="722dc-131">[Pagamenti elettronici svizzeri tramite LSV+](swiss-electronic-payments-using-lsv-.md) </span><span class="sxs-lookup"><span data-stu-id="722dc-131">[Swiss Electronic Payments Using LSV+](swiss-electronic-payments-using-lsv-.md) </span></span>  
 <span data-ttu-id="722dc-132">[Funzionalità locale per la Svizzera](switzerland-local-functionality.md)  ' [Creare movimenti riscossione addebiti diretti SEPA ed esportarli in un file della banca](../../finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md)</span><span class="sxs-lookup"><span data-stu-id="722dc-132">[Switzerland Local Functionality](switzerland-local-functionality.md)  ' [Create SEPA Direct Debit Collection Entries and Export to a Bank File](../../finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md)</span></span>  
 [<span data-ttu-id="722dc-133">Effettuare i pagamenti</span><span class="sxs-lookup"><span data-stu-id="722dc-133">Making Payments</span></span>](../../payables-make-payments.md)

