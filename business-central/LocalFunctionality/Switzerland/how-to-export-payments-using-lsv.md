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
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: a2799b9552ba1f4c5c88827c0ba7a5f6cf321155
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 03/31/2019
ms.locfileid: "936835"
---
# <a name="export-payments-using-lsv"></a><span data-ttu-id="d57a4-104">Esportare pagamenti tramite LSV</span><span class="sxs-lookup"><span data-stu-id="d57a4-104">Export Payments Using LSV</span></span>
<span data-ttu-id="d57a4-105">È possibile esportare o creare file LSV+ (Lastschrift Verfahren) che contengono informazioni sui pagamenti dopo aver chiuso la riscossione LSV.</span><span class="sxs-lookup"><span data-stu-id="d57a4-105">You can export or write Lastschrift Verfahren (LSV+) files that contain payments information after closing the LSV collection.</span></span> <span data-ttu-id="d57a4-106">È possibile inviare i file generati alla banca su un disco oppure usare un trasferimento file elettronico, ad esempio tramite il servizio di online banking o tramite un portale Internet.</span><span class="sxs-lookup"><span data-stu-id="d57a4-106">You can send the generated files to the bank on a disk, or use an electronic file transfer such as your online banking software or an Internet portal.</span></span>  

## <a name="to-export-payments-using-lsv"></a><span data-ttu-id="d57a4-107">Per esportare pagamenti tramite LSV</span><span class="sxs-lookup"><span data-stu-id="d57a4-107">To export payments using LSV</span></span>  

1.  <span data-ttu-id="d57a4-108">Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "Cerca pagina o report"), immettere **Lista registrazioni LSV**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="d57a4-108">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **LSV Journal List**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="d57a4-109">Nella pagina **Lista registrazioni LSV** selezionare le registrazioni LSV desiderate.</span><span class="sxs-lookup"><span data-stu-id="d57a4-109">On the **LSV Journal List** page, select the required LSV journal.</span></span>  
3.  <span data-ttu-id="d57a4-110">Scegliere l'azione **Scrivi file LSV**.</span><span class="sxs-lookup"><span data-stu-id="d57a4-110">Choose the **Write LSV File** action.</span></span>  
4.  <span data-ttu-id="d57a4-111">Nella pagina **Scrivi file LSV**, nella Scheda dettaglio **Opzioni** compilare i campi come descritto nella tabella seguente.</span><span class="sxs-lookup"><span data-stu-id="d57a4-111">On the **Write LSV File** page, on the **Options** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="d57a4-112">Campo</span><span class="sxs-lookup"><span data-stu-id="d57a4-112">Field</span></span>|<span data-ttu-id="d57a4-113">Descrizione</span><span class="sxs-lookup"><span data-stu-id="d57a4-113">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="d57a4-114">**Nr.**</span><span class="sxs-lookup"><span data-stu-id="d57a4-114">**No.**</span></span>|<span data-ttu-id="d57a4-115">Specifica il numero di registrazioni LSV da esportare.</span><span class="sxs-lookup"><span data-stu-id="d57a4-115">Specify the LSV journal number that you want to export.</span></span>|  
    |<span data-ttu-id="d57a4-116">**Test**</span><span class="sxs-lookup"><span data-stu-id="d57a4-116">**Test**</span></span>|<span data-ttu-id="d57a4-117">Specifica se si inviano consegne di prova alla banca.</span><span class="sxs-lookup"><span data-stu-id="d57a4-117">Specify if you are sending test deliveries to your bank.</span></span> <span data-ttu-id="d57a4-118">La banca non elabora file di test.</span><span class="sxs-lookup"><span data-stu-id="d57a4-118">The bank does not process test files.</span></span>|  

5.  <span data-ttu-id="d57a4-119">Tutte le righe correlate vengono trasferite alle registrazioni LSV.</span><span class="sxs-lookup"><span data-stu-id="d57a4-119">All related lines are transferred to the LSV journal.</span></span> <span data-ttu-id="d57a4-120">Il file LSV viene generato nella cartella determinata in precedenza.</span><span class="sxs-lookup"><span data-stu-id="d57a4-120">The LSV file is generated in the predetermined folder.</span></span>  

## <a name="see-also"></a><span data-ttu-id="d57a4-121">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="d57a4-121">See Also</span></span>  
 <span data-ttu-id="d57a4-122">[Pagamenti elettronici svizzeri tramite LSV+](swiss-electronic-payments-using-lsv-.md) </span><span class="sxs-lookup"><span data-stu-id="d57a4-122">[Swiss Electronic Payments Using LSV+](swiss-electronic-payments-using-lsv-.md) </span></span>  
 <span data-ttu-id="d57a4-123">[Elaborare una riscossione LSV](how-to-process-an-lsv-collection.md) </span><span class="sxs-lookup"><span data-stu-id="d57a4-123">[Process an LSV Collection](how-to-process-an-lsv-collection.md) </span></span>  
 <span data-ttu-id="d57a4-124">[Chiudere una riscossione LSV](how-to-close-an-lsv-collection.md) </span><span class="sxs-lookup"><span data-stu-id="d57a4-124">[Close an LSV Collection](how-to-close-an-lsv-collection.md) </span></span>  
 [<span data-ttu-id="d57a4-125">Registrare pagamenti LSV+</span><span class="sxs-lookup"><span data-stu-id="d57a4-125">Post LSV+ Payments</span></span>](how-to-post-lsv-payments.md)
