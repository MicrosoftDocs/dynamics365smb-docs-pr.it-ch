---
title: Come importare pagamenti ESR
description: Dopo aver ricevuto un pagamento da un cliente, si riceve un file che contiene informazioni sulle fatture pagate. È possibile ricevere questo file dalla banca in formato elettronico oppure tramite e-mail.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: 832dbad14962b0e7a1f324d81d798fb4d6759e13
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 04/01/2020
ms.locfileid: "3189125"
---
# <a name="import-esr-payments"></a><span data-ttu-id="db0e5-104">Importare i pagamenti ESR</span><span class="sxs-lookup"><span data-stu-id="db0e5-104">Import ESR Payments</span></span>
<span data-ttu-id="db0e5-105">Dopo aver ricevuto un pagamento da un cliente, si riceve un file che contiene informazioni sulle fatture pagate.</span><span class="sxs-lookup"><span data-stu-id="db0e5-105">After you receive payment from a customer, you receive a file that contains information about paid invoices.</span></span> <span data-ttu-id="db0e5-106">È possibile ricevere questo file dalla banca in formato elettronico oppure tramite e-mail.</span><span class="sxs-lookup"><span data-stu-id="db0e5-106">You can receive this file from your bank electronically, or by mail.</span></span>  

<span data-ttu-id="db0e5-107">È possibile importare dati di fattura ESR (polizza di versamento con numero di riferimento, in tedesco ESR, Einzahlungsschein mit Referenznummer) dal file, stampare i dati tramite il report ESR della fattura di vendita o tramite il report di tagliandi ESR di vendita ed eseguire la verifica prima della registrazione.</span><span class="sxs-lookup"><span data-stu-id="db0e5-107">You can import the Einzahlungsschein mit Referenznummer (ESR) invoice data from the file, print the data by using the sales invoice ESR report or the sales ESR coupon report, and verify before posting.</span></span> <span data-ttu-id="db0e5-108">Per ulteriori informazioni, vedere [Stampare fatture ESR](how-to-print-esr-invoices.md).</span><span class="sxs-lookup"><span data-stu-id="db0e5-108">For more information, see [Print ESR Invoices](how-to-print-esr-invoices.md).</span></span>  

## <a name="to-import-esr-payments"></a><span data-ttu-id="db0e5-109">Per importare pagamenti ESR</span><span class="sxs-lookup"><span data-stu-id="db0e5-109">To import ESR payments</span></span>  

1.  <span data-ttu-id="db0e5-110">Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "Icona della funzionalità Cerca pagina o report"), immettere **Registrazioni incassi**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="db0e5-110">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Cash Receipt Journals**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="db0e5-111">Nel campo **Nome batch** selezionare il batch contabile necessario.</span><span class="sxs-lookup"><span data-stu-id="db0e5-111">In the **Batch Name** field, select the required journal batch.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="db0e5-112">Prima di importare il file ESR, è necessario che le registrazioni siano vuote.</span><span class="sxs-lookup"><span data-stu-id="db0e5-112">The journal must be empty before you import the ESR file.</span></span> <span data-ttu-id="db0e5-113">Non è possibile importare più di un file ESR nelle stesse registrazioni incassi.</span><span class="sxs-lookup"><span data-stu-id="db0e5-113">You cannot import more than one ESR file into the same cash receipt journal.</span></span>  

3.  <span data-ttu-id="db0e5-114">Scegliere l'azione **Leggi file ESR**.</span><span class="sxs-lookup"><span data-stu-id="db0e5-114">Choose the **Read ESR File** action.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="db0e5-115">Se è stata definita più di una banca ESR, viene visualizzato un messaggio di avviso che indica di scegliere la banca pertinente.</span><span class="sxs-lookup"><span data-stu-id="db0e5-115">If you have defined more than one ESR bank, a warning message displays instructing you to choose the relevant bank.</span></span> <span data-ttu-id="db0e5-116">Per ulteriori informazioni, vedere la tabella Setup ESR.</span><span class="sxs-lookup"><span data-stu-id="db0e5-116">For more information, see the ESR Setup table.</span></span>  

4.  <span data-ttu-id="db0e5-117">Scegliere il pulsante **Sì**, quindi scegliere il pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="db0e5-117">Choose the **Yes** button, and then choose the **OK** button.</span></span>  

<span data-ttu-id="db0e5-118">Le informazioni sui pagamenti vengono importate nelle righe di registrazioni.</span><span class="sxs-lookup"><span data-stu-id="db0e5-118">The payments information is imported to the journal lines.</span></span> <span data-ttu-id="db0e5-119">I pagamenti vengono applicati automaticamente alle rispettive fatture in base a numeri di riferimento ESR univoci.</span><span class="sxs-lookup"><span data-stu-id="db0e5-119">The payments are automatically applied to the respective invoices according to unique ESR reference numbers.</span></span>  

## <a name="see-also"></a><span data-ttu-id="db0e5-120">Vedere anche</span><span class="sxs-lookup"><span data-stu-id="db0e5-120">See Also</span></span>  
 <span data-ttu-id="db0e5-121">[Pagamenti elettronici svizzeri utilizzando ESR](swiss-electronic-payments-using-esr.md) </span><span class="sxs-lookup"><span data-stu-id="db0e5-121">[Swiss Electronic Payments Using ESR](swiss-electronic-payments-using-esr.md) </span></span>  
 [<span data-ttu-id="db0e5-122">Stampare fatture ESR</span><span class="sxs-lookup"><span data-stu-id="db0e5-122">Print ESR Invoices</span></span>](how-to-print-esr-invoices.md)
