---
title: Come registrare pagamenti LSV+
description: È possibile registrare pagamenti dopo aver ricevuto l'avviso di pagamento LSV+ (Lastschrift Verfahren) dalla banca.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 59490be7066d76ca9d205a61fbe9b5924510f164
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 03/31/2021
ms.locfileid: "5783606"
---
# <a name="post-lsv-payments"></a><span data-ttu-id="955ae-103">Registrare pagamenti LSV+</span><span class="sxs-lookup"><span data-stu-id="955ae-103">Post LSV+ Payments</span></span>
<span data-ttu-id="955ae-104">È possibile registrare pagamenti dopo aver ricevuto l'avviso di pagamento LSV+ (Lastschrift Verfahren) dalla banca.</span><span class="sxs-lookup"><span data-stu-id="955ae-104">You can post payments after you have received Lastschrift Verfahren (LSV+) payment advice from the bank.</span></span>  

## <a name="to-post-lsv-payments"></a><span data-ttu-id="955ae-105">Registrare pagamenti LSV+</span><span class="sxs-lookup"><span data-stu-id="955ae-105">To post LSV+ payments</span></span>  

1.  <span data-ttu-id="955ae-106">Scegliere l'![icona a forma di lampadina che consente di aprire la funzionalità delle informazioni](../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Registrazioni incassi** e quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="955ae-106">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Cash Receipt Journals**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="955ae-107">Selezionare le registrazioni richieste, quindi scegliere l'azione **Modifica registrazioni**.</span><span class="sxs-lookup"><span data-stu-id="955ae-107">Select the required journal, and then choose the **Edit Journal** action.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="955ae-108">È possibile selezionare il batch registrazioni per LSV in cui è definito il conto di contropartita da considerare.</span><span class="sxs-lookup"><span data-stu-id="955ae-108">You can select the journal batch for LSV where the balance account you want to address is defined.</span></span> <span data-ttu-id="955ae-109">Non è possibile importare più di una riga delle registrazioni LSV nelle stesse registrazioni incassi.</span><span class="sxs-lookup"><span data-stu-id="955ae-109">You cannot import more than one LSV journal line into the same cash receipt journal.</span></span> <span data-ttu-id="955ae-110">Per ulteriori informazioni, vedere la pagina Registrazioni incassi.</span><span class="sxs-lookup"><span data-stu-id="955ae-110">For more information, see the Cash Receipt Journal page.</span></span>  

3.  <span data-ttu-id="955ae-111">Scegliere l'azione **Recupera da registrazioni LSV**.</span><span class="sxs-lookup"><span data-stu-id="955ae-111">Choose the **Get From LSV Journal** action.</span></span>  
4.  <span data-ttu-id="955ae-112">Nella pagina **Lista registrazioni LSV** selezionare la riga di registrazioni LSV da importare nelle registrazioni incassi.</span><span class="sxs-lookup"><span data-stu-id="955ae-112">On the **LSV Journal List** page, select the LSV journal line that you want to import to the cash receipt journal.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="955ae-113">È possibile importare solo righe di registrazioni in cui il campo **Stato LSV** è impostato su **File creato**.</span><span class="sxs-lookup"><span data-stu-id="955ae-113">You can only import journal lines where the **LSV Status** field is set to **File Created**.</span></span>  

5.  <span data-ttu-id="955ae-114">Scegliere il pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="955ae-114">Choose the **OK** button.</span></span>  

    <span data-ttu-id="955ae-115">La riga delle registrazioni LSV viene importata nelle registrazioni incassi.</span><span class="sxs-lookup"><span data-stu-id="955ae-115">The LSV journal line is imported into the cash receipt journal.</span></span> <span data-ttu-id="955ae-116">Il valore del campo **Stato LSV** nella pagina **Lista registrazioni LSV** viene modificato da **File creato** a **Completato**.</span><span class="sxs-lookup"><span data-stu-id="955ae-116">The value in the **LSV Status** field on the **LSV Journal List** page changes from **File Created** to **Finished**.</span></span>  

    <span data-ttu-id="955ae-117">È possibile verificare i pagamenti importati e confrontarli con l'avviso di pagamento bancario nella pagina **Registrazioni incassi**.</span><span class="sxs-lookup"><span data-stu-id="955ae-117">You can check the imported payments, and compare them with your bank payment advice on the **Cash Receipt Journal** page.</span></span> <span data-ttu-id="955ae-118">È anche possibile eliminare le righe di pagamento che la banca non ha potuto elaborare e per cui è necessario contattare direttamente il cliente.</span><span class="sxs-lookup"><span data-stu-id="955ae-118">You can also delete the payment lines that could not be processed by the bank, and for which you must follow up with the customer manually.</span></span>  

6.  <span data-ttu-id="955ae-119">Scegliere l'azione **Registra**.</span><span class="sxs-lookup"><span data-stu-id="955ae-119">Choose the **Post** action.</span></span>  

## <a name="see-also"></a><span data-ttu-id="955ae-120">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="955ae-120">See Also</span></span>  
 <span data-ttu-id="955ae-121">[Pagamenti elettronici svizzeri tramite LSV+](swiss-electronic-payments-using-lsv-.md) </span><span class="sxs-lookup"><span data-stu-id="955ae-121">[Swiss Electronic Payments Using LSV+](swiss-electronic-payments-using-lsv-.md) </span></span>  
 <span data-ttu-id="955ae-122">[Elaborare una riscossione LSV](how-to-process-an-lsv-collection.md) </span><span class="sxs-lookup"><span data-stu-id="955ae-122">[Process an LSV Collection](how-to-process-an-lsv-collection.md) </span></span>  
 <span data-ttu-id="955ae-123">[Chiudere una riscossione LSV](how-to-close-an-lsv-collection.md) </span><span class="sxs-lookup"><span data-stu-id="955ae-123">[Close an LSV Collection](how-to-close-an-lsv-collection.md) </span></span>  
 [<span data-ttu-id="955ae-124">Esportare pagamenti tramite LSV</span><span class="sxs-lookup"><span data-stu-id="955ae-124">Export Payments Using LSV</span></span>](how-to-export-payments-using-lsv.md) 


[!INCLUDE[footer-include](../../includes/footer-banner.md)]