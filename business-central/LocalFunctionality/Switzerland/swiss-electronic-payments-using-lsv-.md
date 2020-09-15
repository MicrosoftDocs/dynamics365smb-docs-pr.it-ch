---
title: Pagamenti elettronici svizzeri tramite LSV+
description: Il metodo di pagamento elettronico svizzero, ovvero Lastschrift Verfahren (LSV+) o addebito diretto, versione migliorata del metodo LSV, consente alle aziende di recuperare i pagamenti direttamente dai conti correnti dei clienti. Per recuperare i pagamenti dei clienti, è necessario inviare un file LSV alla banca, che raccoglierà i pagamenti richiesti nel file.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: edupont
ms.openlocfilehash: bdb91e0528985cd0a8cfc043fb32636f0d68c285
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 09/09/2020
ms.locfileid: "3778180"
---
# <a name="swiss-electronic-payments-using-lsv"></a><span data-ttu-id="6d461-104">Pagamenti elettronici svizzeri tramite LSV+</span><span class="sxs-lookup"><span data-stu-id="6d461-104">Swiss Electronic Payments Using LSV+</span></span>
<span data-ttu-id="6d461-105">Il metodo di pagamento elettronico svizzero, ovvero Lastschrift Verfahren (LSV+) o addebito diretto, versione migliorata del metodo LSV, consente alle aziende di recuperare i pagamenti direttamente dai conti correnti dei clienti.</span><span class="sxs-lookup"><span data-stu-id="6d461-105">The Lastschrift Verfahren (LSV+)—or direct debit—electronic payment method, an improved version of LSV, allows companies to retrieve payments directly from its customers’ bank accounts.</span></span> <span data-ttu-id="6d461-106">Per recuperare i pagamenti dei clienti, è necessario inviare un file LSV alla banca, che raccoglierà i pagamenti richiesti nel file.</span><span class="sxs-lookup"><span data-stu-id="6d461-106">To retrieve customer payments, you must send an LSV file to the bank, and the bank will collect the payments requested in the file.</span></span>  

<span data-ttu-id="6d461-107">Il metodo LSV+ è un principio di addebito diretto con facoltà di opporsi.</span><span class="sxs-lookup"><span data-stu-id="6d461-107">The LSV+ method is a direct debit principle with right of objection.</span></span> <span data-ttu-id="6d461-108">Il metodo BDD (Business Direct Debit) è invece un sistema di addebito diretto senza facoltà di opporsi.</span><span class="sxs-lookup"><span data-stu-id="6d461-108">Business Direct Debit (BDD) is a direct debit system without right of objection.</span></span> <span data-ttu-id="6d461-109">Il formato di file da inviare alla banca è lo stesso per i sistemi LSV+ e BDD.</span><span class="sxs-lookup"><span data-stu-id="6d461-109">The file format to be sent to the bank is the same for LSV+ and BDD.</span></span>  

<span data-ttu-id="6d461-110">Prima di usare il modulo LSV, è necessario definire le impostazioni nella pagina **Setup LSV**.</span><span class="sxs-lookup"><span data-stu-id="6d461-110">Before using the LSV module, you must define the settings on the **LSV Setup** page.</span></span>

## <a name="automatic-esr-processing"></a><span data-ttu-id="6d461-111">Elaborazione ESR automatica</span><span class="sxs-lookup"><span data-stu-id="6d461-111">Automatic ESR Processing</span></span>  
<span data-ttu-id="6d461-112">È possibile scaricare transazioni creditizie di pagamento nel formato di file ESR (polizza di versamento con numero di riferimento, in tedesco ESR, Einzahlungsschein mit Referenznummer) dalla banca.</span><span class="sxs-lookup"><span data-stu-id="6d461-112">You can download payment credit transactions in Einzahlungsschein mit Referenznummer (ESR) file format from the bank.</span></span> <span data-ttu-id="6d461-113">È possibile ricevere pagamenti LSV nel file ESR se il numero di riferimento ESR è integrato nel sistema LSV+.</span><span class="sxs-lookup"><span data-stu-id="6d461-113">You can receive processed LSV payments in the ESR file if the ESR reference number is integrated with the LSV+ system.</span></span> <span data-ttu-id="6d461-114">Se nei file LSV importati sono inclusi pagamenti LSV+, le righe di registrazione LSV correlate vengono chiuse automaticamente.</span><span class="sxs-lookup"><span data-stu-id="6d461-114">If LSV+ payments are included in your imported LSV files, the related LSV journal lines are closed automatically.</span></span> <span data-ttu-id="6d461-115">L'elaborazione ESR automatica viene eseguita solo per i pagamenti che utilizzano franchi svizzeri (CHF) e richiede che vengano effettuate queste operazioni:</span><span class="sxs-lookup"><span data-stu-id="6d461-115">Automatic ESR processing is performed only for payments that use Swiss Francs (CHF), and requires that you do the following:</span></span>  

- <span data-ttu-id="6d461-116">Dopo aver inviato il file LSV+ alla banca, inviare un report di pagamenti entro tre giorni lavorativi dalla data di elaborazione LSV richiesta.</span><span class="sxs-lookup"><span data-stu-id="6d461-116">After you have sent the LSV+ file to the bank, submit a payments report within three business days following the requested LSV processing date.</span></span>  

- <span data-ttu-id="6d461-117">Importare i file ESR, quindi inserire le registrazioni ESR.</span><span class="sxs-lookup"><span data-stu-id="6d461-117">Import the ESR files, and post the ESR journals.</span></span> <span data-ttu-id="6d461-118">Se una transazione ESR importata è correlata alla riga di pagamento LSV+, la riga di registrazione LSV appropriata viene chiusa automaticamente da ESR.</span><span class="sxs-lookup"><span data-stu-id="6d461-118">If an imported ESR transaction is related to an open LSV+ payment line, then the appropriate LSV journal line is automatically closed by ESR.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="6d461-119">Quando si importa un file ESR, la riga di registrazione LSV viene chiusa da ESR se viene trovata la registrazione LSV appropriata, indipendentemente dal tipo di transazione ESR.</span><span class="sxs-lookup"><span data-stu-id="6d461-119">When importing an ESR file, the LSV journal line is closed by ESR if the appropriate LSV journal is found, regardless of the ESR transaction type.</span></span>  

- <span data-ttu-id="6d461-120">Dopo la data di elaborazione LSV, è possibile controllare le righe di registrazione LSV.</span><span class="sxs-lookup"><span data-stu-id="6d461-120">After the LSV processing date, you can check the LSV journal lines.</span></span> <span data-ttu-id="6d461-121">Se tutte le righe di registrazione LSV sono chiuse, lo stato del campo **Stato LSV** viene aggiornato sul valore **Completato**.</span><span class="sxs-lookup"><span data-stu-id="6d461-121">If all of the LSV journal lines are closed, then the status of the **LSV Status** field is updated to  **Finished**.</span></span>  

## <a name="see-also"></a><span data-ttu-id="6d461-122">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="6d461-122">See Also</span></span>  
 <span data-ttu-id="6d461-123">[Elaborare una riscossione LSV](how-to-process-an-lsv-collection.md) </span><span class="sxs-lookup"><span data-stu-id="6d461-123">[Process an LSV Collection](how-to-process-an-lsv-collection.md) </span></span>  
 <span data-ttu-id="6d461-124">[Chiudere una riscossione LSV](how-to-close-an-lsv-collection.md) </span><span class="sxs-lookup"><span data-stu-id="6d461-124">[Close an LSV Collection](how-to-close-an-lsv-collection.md) </span></span>  
 <span data-ttu-id="6d461-125">[Registrare pagamenti LSV+](how-to-post-lsv-payments.md) </span><span class="sxs-lookup"><span data-stu-id="6d461-125">[Post LSV+ Payments](how-to-post-lsv-payments.md) </span></span>  
 <span data-ttu-id="6d461-126">[Esportare pagamenti tramite LSV](how-to-export-payments-using-lsv.md) </span><span class="sxs-lookup"><span data-stu-id="6d461-126">[Export Payments Using LSV](how-to-export-payments-using-lsv.md) </span></span>  
 <span data-ttu-id="6d461-127">[Pagamenti elettronici svizzeri](swiss-electronic-payments.md) </span><span class="sxs-lookup"><span data-stu-id="6d461-127">[Swiss Electronic Payments](swiss-electronic-payments.md) </span></span>  
 <span data-ttu-id="6d461-128">[Pagamenti elettronici svizzeri tramite ESR](swiss-electronic-payments-using-esr.md) </span><span class="sxs-lookup"><span data-stu-id="6d461-128">[Swiss Electronic Payments Using ESR](swiss-electronic-payments-using-esr.md) </span></span>  
 [<span data-ttu-id="6d461-129">Effettuare i pagamenti</span><span class="sxs-lookup"><span data-stu-id="6d461-129">Making Payments</span></span>](../../payables-make-payments.md)
