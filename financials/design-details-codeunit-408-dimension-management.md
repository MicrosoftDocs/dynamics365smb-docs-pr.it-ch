---
title: 'Dettagli di progettazione: Gestione dimensioni della codeunit 408 | Microsoft Docs'
description: "La gestione delle dimensioni della Codeunit 408 è una libreria di funzione che gestisce le attività comuni correlate alle dimensioni, ad esempio copia da una tabella a un'altra oppure da un documento a un altro."
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
ms.sourcegitcommit: ba26b354d235981bd7291f9ac6402779f554ac7a
ms.openlocfilehash: 32f67c058570f03d4aa1c84d9bb32289b1f07bec
ms.contentlocale: it-ch
ms.lasthandoff: 12/14/2017

---
# <a name="design-details-codeunit-408-dimension-management"></a><span data-ttu-id="c66c7-103">Dettagli di progettazione: Gestione dimensioni della codeunit 408</span><span class="sxs-lookup"><span data-stu-id="c66c7-103">Design Details: Codeunit 408 Dimension Management</span></span>
<span data-ttu-id="c66c7-104">La gestione delle dimensioni della Codeunit 408 è una libreria di funzione che gestisce le attività comuni correlate alle dimensioni, ad esempio copia da una tabella a un'altra oppure da un documento a un altro.</span><span class="sxs-lookup"><span data-stu-id="c66c7-104">Codeunit 408 Dimension Management is a function library that handles common tasks that are related to dimensions, such as copying from one table to another or from one document to another.</span></span> <span data-ttu-id="c66c7-105">In questo argomento sono elencate le funzioni che vengono modificate in Microsoft Dynamics NAV 2013 R2 e vengono specificate le azioni da intraprendere per le funzioni.</span><span class="sxs-lookup"><span data-stu-id="c66c7-105">This topic lists the functions that are modified in Microsoft Dynamics NAV 2013 R2 and specifies what has to be done to the functions.</span></span> <span data-ttu-id="c66c7-106">Numerose funzioni sono state eliminate in quanto non è necessario eseguire copie tra le tabelle delle dimensioni.</span><span class="sxs-lookup"><span data-stu-id="c66c7-106">Many functions are deleted because there is no need for copying between dimension tables.</span></span>  

## <a name="modified-functions"></a><span data-ttu-id="c66c7-107">Funzioni modificate</span><span class="sxs-lookup"><span data-stu-id="c66c7-107">Modified Functions</span></span>  

|<span data-ttu-id="c66c7-108">Nome funzione</span><span class="sxs-lookup"><span data-stu-id="c66c7-108">Function Name</span></span>|<span data-ttu-id="c66c7-109">Descrizione modifica</span><span class="sxs-lookup"><span data-stu-id="c66c7-109">Modification Description</span></span>|  
|-------------------|------------------------------|  
|<span data-ttu-id="c66c7-110">CheckDimSetIDComb</span><span class="sxs-lookup"><span data-stu-id="c66c7-110">CheckDimSetIDComb</span></span>|<span data-ttu-id="c66c7-111">Nuova funzione che sostituisce le altre funzioni di controllo e accetta un ID di set di dimensioni come argomento anziché una tabella delle dimensioni.</span><span class="sxs-lookup"><span data-stu-id="c66c7-111">New function that substitutes the other check functions and takes a Dimension Set ID as an argument instead of a dimension table.</span></span>|  
|<span data-ttu-id="c66c7-112">CheckDimSetIDComb</span><span class="sxs-lookup"><span data-stu-id="c66c7-112">CheckDimSetIDComb</span></span><br /><br /> <span data-ttu-id="c66c7-113">CheckDocDimComb</span><span class="sxs-lookup"><span data-stu-id="c66c7-113">CheckDocDimComb</span></span><br /><br /> <span data-ttu-id="c66c7-114">CheckServContractDimComb</span><span class="sxs-lookup"><span data-stu-id="c66c7-114">CheckServContractDimComb</span></span><br /><br /> <span data-ttu-id="c66c7-115">CheckDimBuffer</span><span class="sxs-lookup"><span data-stu-id="c66c7-115">CheckDimBuffer</span></span><br /><br /> <span data-ttu-id="c66c7-116">CheckDimComb</span><span class="sxs-lookup"><span data-stu-id="c66c7-116">CheckDimComb</span></span><br /><br /> <span data-ttu-id="c66c7-117">CheckDimValueComb</span><span class="sxs-lookup"><span data-stu-id="c66c7-117">CheckDimValueComb</span></span>|<span data-ttu-id="c66c7-118">Elimina.</span><span class="sxs-lookup"><span data-stu-id="c66c7-118">Delete.</span></span> <span data-ttu-id="c66c7-119">Tutti gli utilizzi devono essere modificati in CheckDimSetIDComb.</span><span class="sxs-lookup"><span data-stu-id="c66c7-119">All usage should be changed to CheckDimSetIDComb.</span></span>|  
|<span data-ttu-id="c66c7-120">GetDefaultDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-120">GetDefaultDim</span></span>|<span data-ttu-id="c66c7-121">Modificare per restituire un ID di set di dimensioni sotto forma di valore intero anziché un set di record.</span><span class="sxs-lookup"><span data-stu-id="c66c7-121">Modify to return an integer Dimension Set ID instead of a set of records.</span></span>|  
|<span data-ttu-id="c66c7-122">CopyJnlLineDimToICJnlDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-122">CopyJnlLineDimToICJnlDim</span></span><br /><br /> <span data-ttu-id="c66c7-123">CopyICJnlDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-123">CopyICJnlDimToJnlLineDim</span></span><br /><br /> <span data-ttu-id="c66c7-124">CopyDocDimtoICDocDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-124">CopyDocDimtoICDocDim</span></span><br /><br /> <span data-ttu-id="c66c7-125">CopyICDocDimtoICDocDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-125">CopyICDocDimtoICDocDim</span></span>|<span data-ttu-id="c66c7-126">Modificare per utilizzare DimSetID -> ICJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-126">Modify to work with DimSetID -> ICJnlLineDim</span></span>|  

## <a name="deleted-functions"></a><span data-ttu-id="c66c7-127">Funzioni eliminate</span><span class="sxs-lookup"><span data-stu-id="c66c7-127">Deleted Functions</span></span>  
 <span data-ttu-id="c66c7-128">Le funzioni che vengono eliminate dalla codeunit 408 in relazione alla funzionalità Movimenti set di dimensioni sono elencate di seguito.</span><span class="sxs-lookup"><span data-stu-id="c66c7-128">Functions that are deleted from codeunit 408 in connection with the Dimension Set Entries feature are listed below.</span></span>  

> [!CAUTION]  
>  <span data-ttu-id="c66c7-129">Durante l'aggiornamento del codice dell'applicazione da Microsoft Dynamics NAV 2009 o versioni precedenti a Microsoft Dynamics NAV 2016, le seguenti funzioni non sono disponibili in Microsoft Dynamics NAV 2016.</span><span class="sxs-lookup"><span data-stu-id="c66c7-129">During the upgrade of application code from Microsoft Dynamics NAV 2009 or earlier versions to Microsoft Dynamics NAV 2016, the following functions are not available in Microsoft Dynamics NAV 2016.</span></span> <span data-ttu-id="c66c7-130">Se si dispone di personalizzazioni in cui vengono utilizzate una o più funzioni, è necessario aggiornare il codice di conseguenza.</span><span class="sxs-lookup"><span data-stu-id="c66c7-130">If you have customizations that use one or more of the functions, you must upgrade that code accordingly.</span></span>

 <span data-ttu-id="c66c7-131">InsertJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-131">InsertJnlLineDim</span></span>  

 <span data-ttu-id="c66c7-132">UpdateJnlLineDefaultDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-132">UpdateJnlLineDefaultDim</span></span>  

 <span data-ttu-id="c66c7-133">GetJnlLineDefaultDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-133">GetJnlLineDefaultDim</span></span>  

 <span data-ttu-id="c66c7-134">GetPreviousDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-134">GetPreviousDocDefaultDim</span></span>  

 <span data-ttu-id="c66c7-135">GetPreviousProdDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-135">GetPreviousProdDocDefaultDim</span></span>  

 <span data-ttu-id="c66c7-136">InsertDocDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-136">InsertDocDim</span></span>  

 <span data-ttu-id="c66c7-137">UpdateDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-137">UpdateDocDefaultDim</span></span>  

 <span data-ttu-id="c66c7-138">ExtractDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-138">ExtractDocDefaultDim</span></span>  

 <span data-ttu-id="c66c7-139">InsertProdDocDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-139">InsertProdDocDim</span></span>  

 <span data-ttu-id="c66c7-140">UpdateProdDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-140">UpdateProdDocDefaultDim</span></span>  

 <span data-ttu-id="c66c7-141">InsertServContractDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-141">InsertServContractDim</span></span>  

 <span data-ttu-id="c66c7-142">UpdateServcontractDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-142">UpdateServcontractDim</span></span>  

 <span data-ttu-id="c66c7-143">UpdateDefaultDimNewDimValue</span><span class="sxs-lookup"><span data-stu-id="c66c7-143">UpdateDefaultDimNewDimValue</span></span>  

 <span data-ttu-id="c66c7-144">GetDocDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-144">GetDocDim</span></span>  

 <span data-ttu-id="c66c7-145">GetProdDocDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-145">GetProdDocDim</span></span>  

 <span data-ttu-id="c66c7-146">TypeToTableID1</span><span class="sxs-lookup"><span data-stu-id="c66c7-146">TypeToTableID1</span></span>  

 <span data-ttu-id="c66c7-147">TypeToTableID2</span><span class="sxs-lookup"><span data-stu-id="c66c7-147">TypeToTableID2</span></span>  

 <span data-ttu-id="c66c7-148">TypeToTableID3</span><span class="sxs-lookup"><span data-stu-id="c66c7-148">TypeToTableID3</span></span>  

 <span data-ttu-id="c66c7-149">TypeToTableID4</span><span class="sxs-lookup"><span data-stu-id="c66c7-149">TypeToTableID4</span></span>  

 <span data-ttu-id="c66c7-150">TypeToTableID5</span><span class="sxs-lookup"><span data-stu-id="c66c7-150">TypeToTableID5</span></span>  

 <span data-ttu-id="c66c7-151">DeleteJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-151">DeleteJnlLineDim</span></span>  

 <span data-ttu-id="c66c7-152">DeleteDocDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-152">DeleteDocDim</span></span>  

 <span data-ttu-id="c66c7-153">DeletePostedDocDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-153">DeletePostedDocDim</span></span>  

 <span data-ttu-id="c66c7-154">DeleteProdDocDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-154">DeleteProdDocDim</span></span>  

 <span data-ttu-id="c66c7-155">DeleteServContractDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-155">DeleteServContractDim</span></span>  

 <span data-ttu-id="c66c7-156">ShowJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-156">ShowJnlLineDim</span></span>  

 <span data-ttu-id="c66c7-157">SaveJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-157">SaveJnlLineDim</span></span>  

 <span data-ttu-id="c66c7-158">ShowJnlLineNewDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-158">ShowJnlLineNewDim</span></span>  

 <span data-ttu-id="c66c7-159">SaveJnlLineNewDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-159">SaveJnlLineNewDim</span></span>  

 <span data-ttu-id="c66c7-160">ShowDocDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-160">ShowDocDim</span></span>  

 <span data-ttu-id="c66c7-161">SaveDocDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-161">SaveDocDim</span></span>  

 <span data-ttu-id="c66c7-162">ShowProdDocDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-162">ShowProdDocDim</span></span>  

 <span data-ttu-id="c66c7-163">SaveProdDocDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-163">SaveProdDocDim</span></span>  

 <span data-ttu-id="c66c7-164">ShowTempDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-164">ShowTempDim</span></span>  

 <span data-ttu-id="c66c7-165">SaveTempDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-165">SaveTempDim</span></span>  

 <span data-ttu-id="c66c7-166">ShowTempNewDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-166">ShowTempNewDim</span></span>  

 <span data-ttu-id="c66c7-167">SaveTempNewDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-167">SaveTempNewDim</span></span>  

 <span data-ttu-id="c66c7-168">SaveServContractDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-168">SaveServContractDim</span></span>  

 <span data-ttu-id="c66c7-169">MoveJnlLineDimToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-169">MoveJnlLineDimToLedgEntryDim</span></span>  

 <span data-ttu-id="c66c7-170">MoveDocDimToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-170">MoveDocDimToPostedDocDim</span></span>  

 <span data-ttu-id="c66c7-171">MoveOneDocDimToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-171">MoveOneDocDimToPostedDocDim</span></span>  

 <span data-ttu-id="c66c7-172">MoveLedgEntryDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-172">MoveLedgEntryDimToJnlLineDim</span></span>  

 <span data-ttu-id="c66c7-173">MoveDimBufToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-173">MoveDimBufToJnlLineDim</span></span>  

 <span data-ttu-id="c66c7-174">MoveDimBufToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-174">MoveDimBufToLedgEntryDim</span></span>  

 <span data-ttu-id="c66c7-175">MoveDimBufToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-175">MoveDimBufToPostedDocDim</span></span>  

 <span data-ttu-id="c66c7-176">MoveDimBufToGLBudgetDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-176">MoveDimBufToGLBudgetDim</span></span>  

 <span data-ttu-id="c66c7-177">CopyJnlLineDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-177">CopyJnlLineDimToJnlLineDim</span></span>  

 <span data-ttu-id="c66c7-178">CopyLedgEntryDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-178">CopyLedgEntryDimToJnlLineDim</span></span>  

 <span data-ttu-id="c66c7-179">CopyDocDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-179">CopyDocDimToDocDim</span></span>  

 <span data-ttu-id="c66c7-180">CopyPostedDocDimToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-180">CopyPostedDocDimToPostedDocDim</span></span>  

 <span data-ttu-id="c66c7-181">CopyDocDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-181">CopyDocDimToJnlLineDim</span></span>  

 <span data-ttu-id="c66c7-182">CopyDimBufToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-182">CopyDimBufToJnlLineDim</span></span>  

 <span data-ttu-id="c66c7-183">CopyDimBufToDocDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-183">CopyDimBufToDocDim</span></span>  

 <span data-ttu-id="c66c7-184">CopySCDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-184">CopySCDimToDocDim</span></span>  

 <span data-ttu-id="c66c7-185">MoveDocDimToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-185">MoveDocDimToLedgEntryDim</span></span>  

 <span data-ttu-id="c66c7-186">MoveDocDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-186">MoveDocDimToDocDim</span></span>  

 <span data-ttu-id="c66c7-187">MoveDocDimArchvToDocDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-187">MoveDocDimArchvToDocDim</span></span>  

 <span data-ttu-id="c66c7-188">MoveLedgEntryDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-188">MoveLedgEntryDimToDocDim</span></span>  

 <span data-ttu-id="c66c7-189">MoveProdDocDimToProdDocDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-189">MoveProdDocDimToProdDocDim</span></span>  

 <span data-ttu-id="c66c7-190">MoveJnlLineDimToProdDocDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-190">MoveJnlLineDimToProdDocDim</span></span>  

 <span data-ttu-id="c66c7-191">MoveJnlLineDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-191">MoveJnlLineDimToDocDim</span></span>  

 <span data-ttu-id="c66c7-192">MoveJnlLineDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-192">MoveJnlLineDimToJnlLineDim</span></span>  

 <span data-ttu-id="c66c7-193">CopyLedgEntryDimToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-193">CopyLedgEntryDimToLedgEntryDim</span></span>  

 <span data-ttu-id="c66c7-194">MoveTempFromDimToTempToDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-194">MoveTempFromDimToTempToDim</span></span>  

 <span data-ttu-id="c66c7-195">TransferTempToDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-195">TransferTempToDimToDocDim</span></span>  

 <span data-ttu-id="c66c7-196">MoveJnlLineDimToBuf</span><span class="sxs-lookup"><span data-stu-id="c66c7-196">MoveJnlLineDimToBuf</span></span>  

 <span data-ttu-id="c66c7-197">CopyICJnlDimToICJnlDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-197">CopyICJnlDimToICJnlDim</span></span>  

 <span data-ttu-id="c66c7-198">TestDimValue</span><span class="sxs-lookup"><span data-stu-id="c66c7-198">TestDimValue</span></span>  

 <span data-ttu-id="c66c7-199">TestNewDimValue</span><span class="sxs-lookup"><span data-stu-id="c66c7-199">TestNewDimValue</span></span>  

 <span data-ttu-id="c66c7-200">MoveDimBufToItemBudgetDim.</span><span class="sxs-lookup"><span data-stu-id="c66c7-200">MoveDimBufToItemBudgetDim.</span></span> <span data-ttu-id="c66c7-201">(Eliminare perché la tabella ItemBudgetDim viene eliminata).</span><span class="sxs-lookup"><span data-stu-id="c66c7-201">(Delete because the ItemBudgetDim Table is deleted.)</span></span>  

 <span data-ttu-id="c66c7-202">GetServContractDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-202">GetServContractDim</span></span>  

 <span data-ttu-id="c66c7-203">MoveTempDimToBuf</span><span class="sxs-lookup"><span data-stu-id="c66c7-203">MoveTempDimToBuf</span></span>  

 <span data-ttu-id="c66c7-204">UpdateSCInvLineDim</span><span class="sxs-lookup"><span data-stu-id="c66c7-204">UpdateSCInvLineDim</span></span>  

 <span data-ttu-id="c66c7-205">CopyJnlLineDimToBuffer</span><span class="sxs-lookup"><span data-stu-id="c66c7-205">CopyJnlLineDimToBuffer</span></span>  

 <span data-ttu-id="c66c7-206">UpdateDocDefaultDim2</span><span class="sxs-lookup"><span data-stu-id="c66c7-206">UpdateDocDefaultDim2</span></span>  

## <a name="see-also"></a><span data-ttu-id="c66c7-207">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="c66c7-207">See Also</span></span>
 <span data-ttu-id="c66c7-208">[Dettagli di progettazione: Movimenti set di dimensioni](design-details-dimension-set-entries.md) </span><span class="sxs-lookup"><span data-stu-id="c66c7-208">[Design Details: Dimension Set Entries](design-details-dimension-set-entries.md) </span></span>  
 <span data-ttu-id="c66c7-209">[Dettagli di progettazione: Sintesi movimenti set di dimensioni](design-details-dimension-set-entries-overview.md) </span><span class="sxs-lookup"><span data-stu-id="c66c7-209">[Design Details: Dimension Set Entries Overview](design-details-dimension-set-entries-overview.md) </span></span>  
 <span data-ttu-id="c66c7-210">[Dettagli di progettazione: Ricerca delle combinazioni di dimensione](design-details-searching-for-dimension-combinations.md) </span><span class="sxs-lookup"><span data-stu-id="c66c7-210">[Design Details: Searching for Dimension Combinations](design-details-searching-for-dimension-combinations.md) </span></span>  
 <span data-ttu-id="c66c7-211">[Dettagli di progettazione: Struttura della tabella](design-details-table-structure.md) </span><span class="sxs-lookup"><span data-stu-id="c66c7-211">[Design Details: Table Structure](design-details-table-structure.md) </span></span>  
 [<span data-ttu-id="c66c7-212">Dettagli di progettazione: Esempi di codice dei modelli modificati nelle modifiche</span><span class="sxs-lookup"><span data-stu-id="c66c7-212">Design Details: Code Examples of Changed Patterns in Modifications</span></span>](design-details-code-examples-of-changed-patterns-in-modifications.md)

