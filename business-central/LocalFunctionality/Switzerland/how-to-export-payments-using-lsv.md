---
title: Come esportare pagamenti tramite LSV
description: È possibile esportare o creare file LSV+ (Lastschrift Verfahren) che contengono informazioni sui pagamenti dopo aver chiuso la riscossione LSV. È possibile inviare i file generati alla banca su un disco oppure usare un trasferimento file elettronico, ad esempio tramite il servizio di online banking o tramite un portale Internet.
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
ms.openlocfilehash: 7b391d655c4fc61f15cd240809183550a678f143
ms.sourcegitcommit: 007b331b6974983ee614db0406f00777da359ecb
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 08/10/2020
ms.locfileid: "3676953"
---
# <a name="export-payments-using-lsv"></a><span data-ttu-id="9bb58-104">Esportare pagamenti tramite LSV</span><span class="sxs-lookup"><span data-stu-id="9bb58-104">Export Payments Using LSV</span></span>
<span data-ttu-id="9bb58-105">È possibile esportare o creare file LSV+ (Lastschrift Verfahren) che contengono informazioni sui pagamenti dopo aver chiuso la riscossione LSV.</span><span class="sxs-lookup"><span data-stu-id="9bb58-105">You can export or write Lastschrift Verfahren (LSV+) files that contain payments information after closing the LSV collection.</span></span> <span data-ttu-id="9bb58-106">È possibile inviare i file generati alla banca su un disco oppure usare un trasferimento file elettronico, ad esempio tramite il servizio di online banking o tramite un portale Internet.</span><span class="sxs-lookup"><span data-stu-id="9bb58-106">You can send the generated files to the bank on a disk, or use an electronic file transfer such as your online banking software or an Internet portal.</span></span>  

## <a name="to-export-payments-using-lsv"></a><span data-ttu-id="9bb58-107">Per esportare pagamenti tramite LSV</span><span class="sxs-lookup"><span data-stu-id="9bb58-107">To export payments using LSV</span></span>  

1.  <span data-ttu-id="9bb58-108">Scegliere l'![icona a forma di lampadina che consente di aprire la funzionalità delle informazioni](../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Lista registrazioni LSV** e quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="9bb58-108">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **LSV Journal List**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="9bb58-109">Nella pagina **Lista registrazioni LSV** selezionare le registrazioni LSV desiderate.</span><span class="sxs-lookup"><span data-stu-id="9bb58-109">On the **LSV Journal List** page, select the required LSV journal.</span></span>  
3.  <span data-ttu-id="9bb58-110">Scegliere l'azione **Scrivi file LSV**.</span><span class="sxs-lookup"><span data-stu-id="9bb58-110">Choose the **Write LSV File** action.</span></span>  
4.  <span data-ttu-id="9bb58-111">Nella pagina **Scrivi file LSV**, nella Scheda dettaglio **Opzioni** compilare i campi come descritto nella tabella seguente.</span><span class="sxs-lookup"><span data-stu-id="9bb58-111">On the **Write LSV File** page, on the **Options** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="9bb58-112">Campo</span><span class="sxs-lookup"><span data-stu-id="9bb58-112">Field</span></span>|<span data-ttu-id="9bb58-113">Descrizione</span><span class="sxs-lookup"><span data-stu-id="9bb58-113">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="9bb58-114">**Nr.**</span><span class="sxs-lookup"><span data-stu-id="9bb58-114">**No.**</span></span>|<span data-ttu-id="9bb58-115">Specifica il numero di registrazioni LSV da esportare.</span><span class="sxs-lookup"><span data-stu-id="9bb58-115">Specify the LSV journal number that you want to export.</span></span>|  
    |<span data-ttu-id="9bb58-116">**Test**</span><span class="sxs-lookup"><span data-stu-id="9bb58-116">**Test**</span></span>|<span data-ttu-id="9bb58-117">Specifica se si inviano consegne di prova alla banca.</span><span class="sxs-lookup"><span data-stu-id="9bb58-117">Specify if you are sending test deliveries to your bank.</span></span> <span data-ttu-id="9bb58-118">La banca non elabora file di test.</span><span class="sxs-lookup"><span data-stu-id="9bb58-118">The bank does not process test files.</span></span>|  

5.  <span data-ttu-id="9bb58-119">Tutte le righe correlate vengono trasferite alle registrazioni LSV.</span><span class="sxs-lookup"><span data-stu-id="9bb58-119">All related lines are transferred to the LSV journal.</span></span> <span data-ttu-id="9bb58-120">Il file LSV viene generato nella cartella determinata in precedenza.</span><span class="sxs-lookup"><span data-stu-id="9bb58-120">The LSV file is generated in the predetermined folder.</span></span>  

## <a name="see-also"></a><span data-ttu-id="9bb58-121">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="9bb58-121">See Also</span></span>  
 <span data-ttu-id="9bb58-122">[Pagamenti elettronici svizzeri tramite LSV+](swiss-electronic-payments-using-lsv-.md) </span><span class="sxs-lookup"><span data-stu-id="9bb58-122">[Swiss Electronic Payments Using LSV+](swiss-electronic-payments-using-lsv-.md) </span></span>  
 <span data-ttu-id="9bb58-123">[Elaborare una riscossione LSV](how-to-process-an-lsv-collection.md) </span><span class="sxs-lookup"><span data-stu-id="9bb58-123">[Process an LSV Collection](how-to-process-an-lsv-collection.md) </span></span>  
 <span data-ttu-id="9bb58-124">[Chiudere una riscossione LSV](how-to-close-an-lsv-collection.md) </span><span class="sxs-lookup"><span data-stu-id="9bb58-124">[Close an LSV Collection](how-to-close-an-lsv-collection.md) </span></span>  
 [<span data-ttu-id="9bb58-125">Registrare pagamenti LSV+</span><span class="sxs-lookup"><span data-stu-id="9bb58-125">Post LSV+ Payments</span></span>](how-to-post-lsv-payments.md)
