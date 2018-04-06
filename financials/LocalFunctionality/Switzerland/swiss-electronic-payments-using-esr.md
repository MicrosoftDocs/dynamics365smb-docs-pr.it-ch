---
title: Pagamenti elettronici svizzeri tramite ESR
description: "Il metodo di pagamento elettronico ESR (polizza di versamento con numero di riferimento, in tedesco ESR, Einzahlungsschein mit Referenznummer) è un servizio debitori elettronico che consente al cliente di fatturare fatture aperte in franchi svizzeri (CHF) ed euro (EUR) e di registrare pagamenti in entrata in modo efficiente."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 9f76b2e2c4e099592a8cb9476225a51a378aec57
ms.contentlocale: it-ch
ms.lasthandoff: 03/22/2018

---
# <a name="swiss-electronic-payments-using-esr"></a><span data-ttu-id="03e7d-103">Pagamenti elettronici svizzeri tramite ESR</span><span class="sxs-lookup"><span data-stu-id="03e7d-103">Swiss Electronic Payments Using ESR</span></span>
<span data-ttu-id="03e7d-104">Il metodo di pagamento elettronico ESR (polizza di versamento con numero di riferimento, in tedesco ESR, Einzahlungsschein mit Referenznummer) è un servizio debitori elettronico che consente al cliente di fatturare fatture aperte in franchi svizzeri (CHF) ed euro (EUR) e di registrare pagamenti in entrata in modo efficiente.</span><span class="sxs-lookup"><span data-stu-id="03e7d-104">The Einzahlungsschein mit Referenznummer (ESR) electronic payment method is an electronic debtor service that allows the customer to bill open invoices in Swiss Francs (CHF) and Euros (EUR), and to post incoming payments efficiently.</span></span> <span data-ttu-id="03e7d-105">Il numero di riferimento, o riga di codice, contiene tutti i dati contabili rilevanti.</span><span class="sxs-lookup"><span data-stu-id="03e7d-105">The reference number, or code line, contains all relevant bookkeeping data.</span></span>  

<span data-ttu-id="03e7d-106">Con i pagamenti elettronici ESR è possibile effettuare le seguenti operazioni:</span><span class="sxs-lookup"><span data-stu-id="03e7d-106">With ESR electronic payments, you can do the following:</span></span>  

- <span data-ttu-id="03e7d-107">Inviare distinte di pagamento ESR con numeri di riferimento univoci sulle fatture.</span><span class="sxs-lookup"><span data-stu-id="03e7d-107">Send ESR payment slips with unique reference numbers on the invoices.</span></span> <span data-ttu-id="03e7d-108">Poiché i numeri di riferimento ESR sono univoci, i pagamenti per la liquidazione vengono applicati automaticamente alle fatture correlate.</span><span class="sxs-lookup"><span data-stu-id="03e7d-108">Because of the unique ESR reference numbers, the payments for settlement are automatically applied to the related invoices.</span></span> <span data-ttu-id="03e7d-109">Per ulteriori informazioni, vedere [Stampare fatture ESR](how-to-print-esr-invoices.md).</span><span class="sxs-lookup"><span data-stu-id="03e7d-109">For more information, see [Print ESR Invoices](how-to-print-esr-invoices.md).</span></span>  

- <span data-ttu-id="03e7d-110">Scaricare giornalmente i file ESR dalla banca.</span><span class="sxs-lookup"><span data-stu-id="03e7d-110">Download the ESR files from the bank daily.</span></span> <span data-ttu-id="03e7d-111">I file contengono informazioni su tutte le fatture pagate.</span><span class="sxs-lookup"><span data-stu-id="03e7d-111">The files contain information about all paid invoices.</span></span>  

- <span data-ttu-id="03e7d-112">Importare i file ESR e creare righe di pagamento in modo automatico per ogni pagamento.</span><span class="sxs-lookup"><span data-stu-id="03e7d-112">Import the ESR files and create payment lines automatically for each payment.</span></span> <span data-ttu-id="03e7d-113">Per ulteriori informazioni, vedere [Importare pagamenti ESR](how-to-import-esr-payments.md).</span><span class="sxs-lookup"><span data-stu-id="03e7d-113">For more information, see [Import ESR Payments](how-to-import-esr-payments.md).</span></span>  

> [!NOTE]  
>  <span data-ttu-id="03e7d-114">Prima di usare il modulo ESR, è necessario impostare la banca, il conto corrente bancario e il nome del file.</span><span class="sxs-lookup"><span data-stu-id="03e7d-114">Before you can use the ESR module, you must set up the bank, bank account, and file name.</span></span> <span data-ttu-id="03e7d-115">È inoltre necessario specificare se deve essere usato il metodo ESR o ESR+.</span><span class="sxs-lookup"><span data-stu-id="03e7d-115">You must also specify whether ESR or ESR+ should be used.</span></span>

<span data-ttu-id="03e7d-116">Dopo aver valutato le informazioni di setup, è possibile modificare il modulo di fatturazione e creare una serie di test che la banca o il servizio postale può convalidare.</span><span class="sxs-lookup"><span data-stu-id="03e7d-116">When you have evaluated the setup information, you can adjust the invoice form, and you can create a test series that you can ask your bank or postal service to validate.</span></span>  

<span data-ttu-id="03e7d-117">Quando si impostano le numerazioni per le fatture, è necessario seguire queste linee guida:</span><span class="sxs-lookup"><span data-stu-id="03e7d-117">When you set up number series for invoices, you must follow these guidelines:</span></span>  

- <span data-ttu-id="03e7d-118">Usa un massimo di otto cifre.</span><span class="sxs-lookup"><span data-stu-id="03e7d-118">Use a maximum of eight digits.</span></span>  
- <span data-ttu-id="03e7d-119">Usare solo caratteri numerici.</span><span class="sxs-lookup"><span data-stu-id="03e7d-119">Use only numeric characters.</span></span>  
- <span data-ttu-id="03e7d-120">Non anteporre zero ai numeri.</span><span class="sxs-lookup"><span data-stu-id="03e7d-120">Do not precede numbers with zeros.</span></span>  

## <a name="see-also"></a><span data-ttu-id="03e7d-121">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="03e7d-121">See Also</span></span>  
 <span data-ttu-id="03e7d-122">[Pagamenti elettronici svizzeri](swiss-electronic-payments.md) </span><span class="sxs-lookup"><span data-stu-id="03e7d-122">[Swiss Electronic Payments](swiss-electronic-payments.md) </span></span>  
 <span data-ttu-id="03e7d-123">[Stampare fatture ESR](how-to-print-esr-invoices.md) </span><span class="sxs-lookup"><span data-stu-id="03e7d-123">[Print ESR Invoices](how-to-print-esr-invoices.md) </span></span>  
 <span data-ttu-id="03e7d-124">[Importare i pagamenti ESR](how-to-import-esr-payments.md) </span><span class="sxs-lookup"><span data-stu-id="03e7d-124">[Import ESR Payments](how-to-import-esr-payments.md) </span></span>  
 <span data-ttu-id="03e7d-125">[Pagamenti elettronici svizzeri tramite LSV+](swiss-electronic-payments-using-lsv-.md) </span><span class="sxs-lookup"><span data-stu-id="03e7d-125">[Swiss Electronic Payments Using LSV+](swiss-electronic-payments-using-lsv-.md) </span></span>  
 [<span data-ttu-id="03e7d-126">Effettuare i pagamenti</span><span class="sxs-lookup"><span data-stu-id="03e7d-126">Making Payments</span></span>](../../payables-make-payments.md)

