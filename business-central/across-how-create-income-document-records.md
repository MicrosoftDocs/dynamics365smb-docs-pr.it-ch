---
title: Creare i record di documenti in entrata| Documenti Microsoft
description: È possibile creare i record dei documenti in entrata, ad esempio le fatture elettroniche, e gestire le attività OCR, il commercio elettronico e il servizio di scambio documenti.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 7e045948aae1140f999a2a1d0db98de162e8e1e8
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 03/31/2021
ms.locfileid: "5776065"
---
# <a name="create-incoming-document-records"></a><span data-ttu-id="581b5-103">Creare i record di documenti in entrata</span><span class="sxs-lookup"><span data-stu-id="581b5-103">Create Incoming Document Records</span></span>
<span data-ttu-id="581b5-104">Nella pagina **Documenti in entrata** è possibile utilizzare diverse funzioni per esaminare le ricevute relative alle spese, gestire le attività OCR e convertire i file dei documenti in entrata, manualmente o automaticamente, nei relativi documenti o in righe di registrazione.</span><span class="sxs-lookup"><span data-stu-id="581b5-104">On the **Incoming Documents** page, you can use different functions to review expense receipts, manage OCR tasks, and convert incoming document files, manually or automatically, to the relevant documents or journal lines.</span></span> <span data-ttu-id="581b5-105">I file esterni possono essere allegati in qualsiasi fase dell'elaborazione, ad esempio ai documenti registrati, nonché ai fornitori, clienti e movimenti di contabilità generale risultanti.</span><span class="sxs-lookup"><span data-stu-id="581b5-105">The external files can be attached at any process stage, including to posted documents and to the resulting vendor, customer, and general ledger entries.</span></span>

<span data-ttu-id="581b5-106">Per registrare un documento esterno in [!INCLUDE[prod_short](includes/prod_short.md)], è necessario prima creare o completare un record di documento in entrata.</span><span class="sxs-lookup"><span data-stu-id="581b5-106">To record an external document in [!INCLUDE[prod_short](includes/prod_short.md)], you must first create or complete an incoming document record.</span></span> <span data-ttu-id="581b5-107">Questa operazione può essere eseguita manualmente oppure scattando una foto del documento e quindi creando un record del documento in entrata con il file immagine allegato.</span><span class="sxs-lookup"><span data-stu-id="581b5-107">You can do this manually, or you can take a photo of the external document and then create the incoming document record with the image file attached.</span></span>

<span data-ttu-id="581b5-108">Per poter utilizzare la funzionalità Documenti in entrata, è necessario eseguire l'impostazione necessaria.</span><span class="sxs-lookup"><span data-stu-id="581b5-108">Before you can use the Incoming Documents feature, you must perform the required setup.</span></span> <span data-ttu-id="581b5-109">Per ulteriori informazioni, vedere [Impostare documenti in entrata](across-how-setup-income-documents.md).</span><span class="sxs-lookup"><span data-stu-id="581b5-109">For more information, see [Set Up Incoming Documents](across-how-setup-income-documents.md).</span></span>

## <a name="to-approve-or-reject-an-incoming-document"></a><span data-ttu-id="581b5-110">Per approvare o rifiutare un documento in entrata</span><span class="sxs-lookup"><span data-stu-id="581b5-110">To approve or reject an incoming document</span></span>
<span data-ttu-id="581b5-111">Se non si desidera consentire agli utenti di creare fatture o righe registrazioni COGE da record di documenti in entrata prima che vengano approvati, è possibile impostare dei responsabili che devono approvare i record prima che possano essere elaborati.</span><span class="sxs-lookup"><span data-stu-id="581b5-111">If you do want to allow users to create invoices or general journal lines from incoming document records unless they are approved, you can set up approvers who must approve the records before they can be processed.</span></span>

1. <span data-ttu-id="581b5-112">Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Documenti in entrata** e quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="581b5-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Incoming Documents**, and then choose the related link.</span></span>
2. <span data-ttu-id="581b5-113">Selezionare la riga con il documento che si desidera approvare o rifiutare quindi selezionare l'azione **Approva** o **Rifiuta**.</span><span class="sxs-lookup"><span data-stu-id="581b5-113">Select the line with the document that you want to approve or reject, and then choose the **Approve** or **Reject** actions.</span></span>

<span data-ttu-id="581b5-114">Se si approva il record del documento in entrata, la casella di controllo **Rilasciato** nella riga del documento in entrata è selezionata.</span><span class="sxs-lookup"><span data-stu-id="581b5-114">If you approve the incoming document record, the **Released** check box on the incoming document line is selected.</span></span> <span data-ttu-id="581b5-115">L'utente incaricato di creare, ad esempio, le fatture di acquisto può procedere all'elaborazione del record.</span><span class="sxs-lookup"><span data-stu-id="581b5-115">The user in charge of creating, for example, purchase invoices can proceed to process the record.</span></span>

## <a name="to-create-an-incoming-document-record-by-taking-a-photo"></a><span data-ttu-id="581b5-116">Per creare un record di documento in entrata facendo una foto</span><span class="sxs-lookup"><span data-stu-id="581b5-116">To create an incoming document record by taking a photo</span></span>
> [!NOTE]  
>   <span data-ttu-id="581b5-117">La seguente procedura si applica solo ai client di [!INCLUDE[prod_short](includes/prod_short.md)] per tablet e telefono.</span><span class="sxs-lookup"><span data-stu-id="581b5-117">The following procedure only applies to the [!INCLUDE[prod_short](includes/prod_short.md)] Tablet and Phone clients.</span></span>

1. <span data-ttu-id="581b5-118">Sulla barra delle applicazioni, scegliere il riquadro **Crea documento in entrata da fotocamera** e andare al passaggio 4.</span><span class="sxs-lookup"><span data-stu-id="581b5-118">On the app bar, choose the **Create Incoming Document from Camera** tile, and then go to step 4.</span></span>
2. <span data-ttu-id="581b5-119">In alternativa, nella barra delle applicazioni, fare clic sul pulsante di opzione, selezionare **Documenti in entrata** e scegliere **Tutto**.</span><span class="sxs-lookup"><span data-stu-id="581b5-119">Alternatively, on the app bar, choose the options button, choose **Incoming Documents**, and then choose **All**.</span></span>
3. <span data-ttu-id="581b5-120">Nella pagina **Documenti in entrata** scegliere il pulsante con i puntini di sospensione e selezionare **Crea da fotocamera**.</span><span class="sxs-lookup"><span data-stu-id="581b5-120">On the **Incoming Documents** page, choose the ellipsis button, and then choose **Create from Camera**.</span></span> <span data-ttu-id="581b5-121">La fotocamera del tablet o del telefono è attivata.</span><span class="sxs-lookup"><span data-stu-id="581b5-121">The camera on the tablet or phone is activated.</span></span>
4. <span data-ttu-id="581b5-122">Scattare la foto di un documento, ad esempio una ricevuta di acquisto, che si desidera elaborare come documento in entrata e fare clic sul pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="581b5-122">Take a photo of a document, such as a purchase receipt, that you want to process as an incoming document, and then choose the **OK** button.</span></span>

    <span data-ttu-id="581b5-123">Viene creato un nuovo record di documento in entrata con l'immagine allegata.</span><span class="sxs-lookup"><span data-stu-id="581b5-123">A new incoming document record is created, with the image attached.</span></span>

## <a name="to-attach-an-image-to-an-incoming-document-record-by-taking-a-photo"></a><span data-ttu-id="581b5-124">Per allegare un'immagine a un record di documento in entrata facendo una foto</span><span class="sxs-lookup"><span data-stu-id="581b5-124">To attach an image to an incoming document record by taking a photo</span></span>
> [!NOTE]  
>   <span data-ttu-id="581b5-125">La seguente procedura si applica solo ai client di [!INCLUDE[prod_short](includes/prod_short.md)] per tablet e telefono.</span><span class="sxs-lookup"><span data-stu-id="581b5-125">The following procedure only applies to the [!INCLUDE[prod_short](includes/prod_short.md)] Tablet and Phone clients.</span></span>

1. <span data-ttu-id="581b5-126">Nella barra delle applicazioni, fare clic sul pulsante di opzione, selezionare **Documenti in entrata** e scegliere **Tutto**.</span><span class="sxs-lookup"><span data-stu-id="581b5-126">On the app bar, choose the options button, choose **Incoming Documents**, and then choose **All**.</span></span>
2. <span data-ttu-id="581b5-127">Aprire la scheda di un record di documento in entrata esistente.</span><span class="sxs-lookup"><span data-stu-id="581b5-127">Open the card for an existing incoming document record.</span></span>
3. <span data-ttu-id="581b5-128">Nella pagina **Documento in entrata** scegliere il pulsante con i puntini di sospensione e selezionare **Allega immagine da fotocamera**.</span><span class="sxs-lookup"><span data-stu-id="581b5-128">On the **Incoming Document** page, choose the ellipsis button, and then choose **Attach Image from Camera**.</span></span> <span data-ttu-id="581b5-129">La fotocamera del tablet o del telefono è attivata.</span><span class="sxs-lookup"><span data-stu-id="581b5-129">The camera on the tablet or phone is activated.</span></span>
4. <span data-ttu-id="581b5-130">Scattare la foto di un documento, ad esempio una ricevuta di acquisto, che si desidera elaborare come documento in entrata e fare clic sul pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="581b5-130">Take a photo of a document, such as a purchase receipt, that you want to process as an incoming document, and then choose the **OK** button.</span></span>

    <span data-ttu-id="581b5-131">L'immagine viene allegata al record di documento in entrata.</span><span class="sxs-lookup"><span data-stu-id="581b5-131">The image is attached to the incoming document record.</span></span>

## <a name="to-create-an-incoming-document-record-manually"></a><span data-ttu-id="581b5-132">Per creare manualmente il record di un documento in entrata</span><span class="sxs-lookup"><span data-stu-id="581b5-132">To create an incoming document record manually</span></span>
1. <span data-ttu-id="581b5-133">Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Documenti in entrata** e quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="581b5-133">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Incoming Documents**, and then choose the related link.</span></span>
2. <span data-ttu-id="581b5-134">Selezionare l'azione **Crea da file**.</span><span class="sxs-lookup"><span data-stu-id="581b5-134">Choose the **Create from File** action.</span></span>  
3. <span data-ttu-id="581b5-135">Nella pagina **Inserisci file** selezionare un file e scegliere **Apri**.</span><span class="sxs-lookup"><span data-stu-id="581b5-135">On the **Insert File** page, select a file, and then choose **Open**.</span></span> <span data-ttu-id="581b5-136">Il file viene automaticamente allegato.</span><span class="sxs-lookup"><span data-stu-id="581b5-136">The file is automatically attached.</span></span>
4. <span data-ttu-id="581b5-137">In alternativa, selezionare l'azione **Nuovo**.</span><span class="sxs-lookup"><span data-stu-id="581b5-137">Alternatively, choose the **New** action.</span></span>
5. <span data-ttu-id="581b5-138">Per allegare un file, selezionare l'azione **Allega file**.</span><span class="sxs-lookup"><span data-stu-id="581b5-138">To attach a file, choose the **Attach File** action.</span></span>
6. <span data-ttu-id="581b5-139">Nella pagina **Inserisci file** selezionare il file che rappresenta il documento in entrata in questione, quindi scegliere il pulsante **Apri**.</span><span class="sxs-lookup"><span data-stu-id="581b5-139">On the **Insert File** page, select the file that represents the incoming document in question, and then choose the **Open** button.</span></span>
7. <span data-ttu-id="581b5-140">Nella pagina **Documento in entrata** compilare i campi secondo le proprie necessità.</span><span class="sxs-lookup"><span data-stu-id="581b5-140">On the **Incoming Document** page, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="see-also"></a><span data-ttu-id="581b5-141">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="581b5-141">See Also</span></span>
[<span data-ttu-id="581b5-142">Elaborare i documenti in entrata</span><span class="sxs-lookup"><span data-stu-id="581b5-142">Process Incoming Documents</span></span>](across-process-income-documents.md)  
[<span data-ttu-id="581b5-143">Documenti in entrata</span><span class="sxs-lookup"><span data-stu-id="581b5-143">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="581b5-144">Acquisti</span><span class="sxs-lookup"><span data-stu-id="581b5-144">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="581b5-145">[Utilizzo di [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="581b5-145">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]