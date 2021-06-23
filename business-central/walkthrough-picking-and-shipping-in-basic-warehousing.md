---
title: Prelievo e spedizione nelle configurazioni della warehouse di base
description: In Business Central, i processi in uscita per il prelievo e la spedizione possono essere eseguiti in quattro modalità utilizzando diverse funzionalità a seconda del livello di complessità della warehouse.
author: jill-kotel-andersson
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 05/27/2021
ms.author: edupont
ms.openlocfilehash: e1763e6288c8b8218955049ba7ef4c461ee5164e
ms.sourcegitcommit: 0953171d39e1232a7c126142d68cac858234a20e
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 06/09/2021
ms.locfileid: "6214671"
---
# <a name="walkthrough-picking-and-shipping-in-basic-warehouse-configurations"></a><span data-ttu-id="3e5dd-103">Procedura dettagliata: prelievo e spedizione nelle configurazioni della warehouse di base</span><span class="sxs-lookup"><span data-stu-id="3e5dd-103">Walkthrough: Picking and Shipping in Basic Warehouse Configurations</span></span>

<!-- [!INCLUDE[complete_sample_data](includes/complete_sample_data.md)] -->

<span data-ttu-id="3e5dd-104">In [!INCLUDE[prod_short](includes/prod_short.md)], i processi in uscita per il prelievo e la spedizione possono essere eseguiti in quattro modalità utilizzando diverse funzionalità a seconda del livello di complessità della warehouse.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-104">In [!INCLUDE[prod_short](includes/prod_short.md)], the outbound processes for picking and shipping can be performed in four ways using different functionalities depending on the warehouse complexity level.</span></span>  

|<span data-ttu-id="3e5dd-105">Metodo</span><span class="sxs-lookup"><span data-stu-id="3e5dd-105">Method</span></span>|<span data-ttu-id="3e5dd-106">Processo in entrata</span><span class="sxs-lookup"><span data-stu-id="3e5dd-106">Inbound process</span></span>|<span data-ttu-id="3e5dd-107">Collocazioni</span><span class="sxs-lookup"><span data-stu-id="3e5dd-107">Bins</span></span>|<span data-ttu-id="3e5dd-108">Prelievi</span><span class="sxs-lookup"><span data-stu-id="3e5dd-108">Picks</span></span>|<span data-ttu-id="3e5dd-109">Spedizioni</span><span class="sxs-lookup"><span data-stu-id="3e5dd-109">Shipments</span></span>|<span data-ttu-id="3e5dd-110">Livello di complessità (vedere [Dettagli di progettazione: Setup warehouse](design-details-warehouse-setup.md))</span><span class="sxs-lookup"><span data-stu-id="3e5dd-110">Complexity level (See [Design Details: Warehouse Setup](design-details-warehouse-setup.md))</span></span>|  
|------------|---------------------|----------|-----------|---------------|--------------------------------------------------------------------------------------------------------------------|  
|<span data-ttu-id="3e5dd-111">A</span><span class="sxs-lookup"><span data-stu-id="3e5dd-111">A</span></span>|<span data-ttu-id="3e5dd-112">Registra prelievo e spedizione dalla riga ordine</span><span class="sxs-lookup"><span data-stu-id="3e5dd-112">Post pick and shipment from the order line</span></span>|<span data-ttu-id="3e5dd-113">X</span><span class="sxs-lookup"><span data-stu-id="3e5dd-113">X</span></span>|||<span data-ttu-id="3e5dd-114">2</span><span class="sxs-lookup"><span data-stu-id="3e5dd-114">2</span></span>|  
|<span data-ttu-id="3e5dd-115">B</span><span class="sxs-lookup"><span data-stu-id="3e5dd-115">B</span></span>|<span data-ttu-id="3e5dd-116">Registra prelievo e spedizione da un documento di prelievo magazzino</span><span class="sxs-lookup"><span data-stu-id="3e5dd-116">Post pick and shipment from an inventory pick document</span></span>||<span data-ttu-id="3e5dd-117">X</span><span class="sxs-lookup"><span data-stu-id="3e5dd-117">X</span></span>||<span data-ttu-id="3e5dd-118">3</span><span class="sxs-lookup"><span data-stu-id="3e5dd-118">3</span></span>|  
|<span data-ttu-id="3e5dd-119">C</span><span class="sxs-lookup"><span data-stu-id="3e5dd-119">C</span></span>|<span data-ttu-id="3e5dd-120">Registra prelievo e spedizione da un documento di spedizione warehouse</span><span class="sxs-lookup"><span data-stu-id="3e5dd-120">Post pick and shipment from a warehouse shipment document</span></span>|||<span data-ttu-id="3e5dd-121">X</span><span class="sxs-lookup"><span data-stu-id="3e5dd-121">X</span></span>|<span data-ttu-id="3e5dd-122">5/4/6</span><span class="sxs-lookup"><span data-stu-id="3e5dd-122">4/5/6</span></span>|  
|<span data-ttu-id="3e5dd-123">D</span><span class="sxs-lookup"><span data-stu-id="3e5dd-123">D</span></span>|<span data-ttu-id="3e5dd-124">Registra il prelievo da un documento di prelievo warehouse e la spedizione da un documento di spedizione warehouse</span><span class="sxs-lookup"><span data-stu-id="3e5dd-124">Post pick from a warehouse pick document and post shipment from a warehouse shipment document</span></span>||<span data-ttu-id="3e5dd-125">X</span><span class="sxs-lookup"><span data-stu-id="3e5dd-125">X</span></span>|<span data-ttu-id="3e5dd-126">X</span><span class="sxs-lookup"><span data-stu-id="3e5dd-126">X</span></span>|<span data-ttu-id="3e5dd-127">5/4/6</span><span class="sxs-lookup"><span data-stu-id="3e5dd-127">4/5/6</span></span>|  

<span data-ttu-id="3e5dd-128">Per ulteriori informazioni, vedere [Dettagli di progettazione: Flusso warehouse in uscita](design-details-outbound-warehouse-flow.md).</span><span class="sxs-lookup"><span data-stu-id="3e5dd-128">For more information, see [Design Details: Outbound Warehouse Flow](design-details-outbound-warehouse-flow.md).</span></span>  

<span data-ttu-id="3e5dd-129">Nella seguente procedura dettagliata viene dimostrato il metodo B nella tabella precedente.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-129">The following walkthrough demonstrates method B in the previous table.</span></span>  

## <a name="about-this-walkthrough"></a><span data-ttu-id="3e5dd-130">Informazioni sulla procedura dettagliata</span><span class="sxs-lookup"><span data-stu-id="3e5dd-130">About This Walkthrough</span></span>

<span data-ttu-id="3e5dd-131">Nelle configurazioni della warehouse di base in cui un'ubicazione è impostata in modo da richiedere l'elaborazione dei prelievi ma non l'elaborazione delle spedizioni, utilizzare la pagina **Prelievi magazzino** per registrare le informazioni riguardanti il prelievo e la spedizione per i documenti di origine in uscita.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-131">In basic warehouse configurations where your location is set up to require pick processing but not ship processing, you use the **Inventory Pick** page to record and post pick and ship information for your outbound source documents.</span></span> <span data-ttu-id="3e5dd-132">Il documento di origine in uscita può essere un ordine di vendita, un ordine di reso da acquisto, un ordine di trasferimento in uscita o un ordine di produzione i cui componenti sono necessari.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-132">The outbound source document can be a sales order, purchase return order, outbound transfer order, or a production order with component need.</span></span>  

<span data-ttu-id="3e5dd-133">In questa procedura dettagliata sono illustrati i task seguenti:</span><span class="sxs-lookup"><span data-stu-id="3e5dd-133">This walkthrough demonstrates the following tasks:</span></span>  

- <span data-ttu-id="3e5dd-134">Impostazione ubicazione SUD per i prelievi magazzino.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-134">Setting up SOUTH location for inventory picks.</span></span>  
- <span data-ttu-id="3e5dd-135">Creazione di un ordine di vendita per il cliente 10000 per 30 Lampade Amsterdam.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-135">Creating a sales order for customer 10000 for 30 Amsterdam Lamps.</span></span>  
- <span data-ttu-id="3e5dd-136">Rilascio dell'ordine di vendita per la gestione warehouse.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-136">Releasing the sales order for warehouse handling.</span></span>  
- <span data-ttu-id="3e5dd-137">Creazione di un prelievo di magazzino in base al documento origine rilasciato.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-137">Creating an inventory pick based on a released source document.</span></span>  
- <span data-ttu-id="3e5dd-138">Registrazione della movimentazione warehouse dalla warehouse e registrazione contemporanea della spedizione vendita per l'ordine di vendita di origine.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-138">Registering the warehouse movement from the warehouse and at the same time posting the sales shipment for the source sales order.</span></span>  

## <a name="roles"></a><span data-ttu-id="3e5dd-139">Ruoli</span><span class="sxs-lookup"><span data-stu-id="3e5dd-139">Roles</span></span>

<span data-ttu-id="3e5dd-140">Questa procedura dettagliata comprende task svolti dai ruoli utente seguenti:</span><span class="sxs-lookup"><span data-stu-id="3e5dd-140">This walkthrough demonstrates tasks that are performed by the following user roles:</span></span>  

- <span data-ttu-id="3e5dd-141">Manager warehouse</span><span class="sxs-lookup"><span data-stu-id="3e5dd-141">Warehouse Manager</span></span>  
- <span data-ttu-id="3e5dd-142">Gestore ordini</span><span class="sxs-lookup"><span data-stu-id="3e5dd-142">Order Processor</span></span>  
- <span data-ttu-id="3e5dd-143">Lavoro warehouse</span><span class="sxs-lookup"><span data-stu-id="3e5dd-143">Warehouse Worker</span></span>  

<!-- ## Prerequisites

To complete this walkthrough, you will need:  

- For [!INCLUDE[prod_short](includes/prod_short.md)] online, a company based on the **Advanced Evaluation - Complete Sample Data** option in a sandbox environment. For [!INCLUDE[prod_short](includes/prod_short.md)] on-premises, CRONUS installed.
 -->

## <a name="story"></a><span data-ttu-id="3e5dd-144">Scenario</span><span class="sxs-lookup"><span data-stu-id="3e5dd-144">Story</span></span>

<span data-ttu-id="3e5dd-145">Ellen, responsabile warehouse presso CRONUS, imposta la warehouse SUD per la gestione dei prelievi di base in cui gli addetti alla warehouse elaborano ordini in uscita singoli.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-145">Ellen, the warehouse manager at CRONUS, sets up SOUTH warehouse for basic pick handling where warehouse workers process outbound orders individually.</span></span> <span data-ttu-id="3e5dd-146">Elisabetta, il gestore ordini, crea un ordine di vendita per 30 unità dell'articolo 1928-S da spedire al cliente 10000 dalla warehouse SUD.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-146">Susan, the order processor, creates a sales order for 30 units of item 1928-S to be shipped to customer 10000 from the SOUTH Warehouse.</span></span> <span data-ttu-id="3e5dd-147">Gianni, il lavoratore warehouse deve assicurarsi che la spedizione sia preparata e consegnata al cliente.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-147">John, the warehouse worker must make sure that the shipment is prepared and delivered to the customer.</span></span> <span data-ttu-id="3e5dd-148">Gianni gestisce tutte le attività interessate nella pagina **Prelievo magazzino** che automaticamente punta alle collocazioni in cui viene archiviato 1928-S.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-148">John manages all involved tasks on the **Inventory Pick** page, which automatically points to the bins where 1928-S is stored.</span></span>

[!INCLUDE[set_up_location.md](includes/set_up_location.md)]

### <a name="setting-up-the-bin-codes"></a><span data-ttu-id="3e5dd-149">Impostazione dei codici collocazione</span><span class="sxs-lookup"><span data-stu-id="3e5dd-149">Setting Up the Bin Codes</span></span>
<span data-ttu-id="3e5dd-150">Una volta impostata la posizione, è necessario aggiungere due contenitori.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-150">Once you have the location set up, you must add two bins.</span></span>

#### <a name="to-setup-the-bin-codes"></a><span data-ttu-id="3e5dd-151">Per impostare i codici collocazione</span><span class="sxs-lookup"><span data-stu-id="3e5dd-151">To setup the bin codes</span></span>

1. <span data-ttu-id="3e5dd-152">Scegliere l'azione **Collocazioni**.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-152">Select the **Bins** action.</span></span>
2. <span data-ttu-id="3e5dd-153">Crea due contenitori, con i codici *S-01-0001* e *S-01-0002*.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-153">Create two bins, with the codes *S-01-0001* and *S-01-0002*.</span></span>

### <a name="making-yourself-a-warehouse-employee-at-location-south"></a><span data-ttu-id="3e5dd-154">Diventare un impiegato warehouse presso l'ubicazione SUD</span><span class="sxs-lookup"><span data-stu-id="3e5dd-154">Making Yourself a Warehouse Employee at Location SOUTH</span></span>

<span data-ttu-id="3e5dd-155">Per utilizzare questa funzionalità, devi aggiungerti all'ubicazione come lavoratore warehouse.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-155">In order to use this functionality, you must add yourself to the location as a warehouse worker.</span></span> 

#### <a name="to-make-yourself-a-warehouse-employee"></a><span data-ttu-id="3e5dd-156">Per diventare un impiegato warehouse</span><span class="sxs-lookup"><span data-stu-id="3e5dd-156">To make yourself a warehouse employee</span></span>

  1. <span data-ttu-id="3e5dd-157">Scegliere la prima icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Impiegati warehouse** e quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-157">Choose the ![Lightbulb that opens the Tell Me feature first](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Warehouse Employees**, and then choose the related link.</span></span>  
  2. <span data-ttu-id="3e5dd-158">Selezionare il campo **ID utente** , quindi il proprio account utente nella pagina **Impiegati warehouse**.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-158">Choose the **User ID** field, and select your own user account on the **Warehouse Employees** page.</span></span>
  3. <span data-ttu-id="3e5dd-159">Nel campo **Codice ubicazione** selezionare SUD.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-159">In the **Location Code** field, choose SOUTH.</span></span>  
  4. <span data-ttu-id="3e5dd-160">Selezionare il campo **Impostazione predefinita**, quindi selezionare il pulsante **Sì**.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-160">Select the **Default** field, and then select the **Yes** button.</span></span>  

### <a name="making-item-1928-s-available"></a><span data-ttu-id="3e5dd-161">Rendere disponibile l'articolo 1928-S</span><span class="sxs-lookup"><span data-stu-id="3e5dd-161">Making Item 1928-S Available</span></span>

<span data-ttu-id="3e5dd-162">Per rendere l'articolo 1928-S disponibile nell'ubicazione SUD seguire i passaggi di seguito riportati:</span><span class="sxs-lookup"><span data-stu-id="3e5dd-162">To make item 1928-S available at the SOUTH location follow these steps:</span></span>  

  1. <span data-ttu-id="3e5dd-163">Scegliere la seconda icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Registrazioni magazzino** e quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-163">Choose the ![Lightbulb that opens the Tell Me feature second](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Item Journals**, and then choose the related link.</span></span>  
  2. <span data-ttu-id="3e5dd-164">Aprire il giornale di default e quindi creare due righe registrazioni magazzino con le informazioni seguenti sulla data di lavoro (23 gennaio).</span><span class="sxs-lookup"><span data-stu-id="3e5dd-164">Open the default journal, and then create two item journal lines with the following information about the work date (January 23).</span></span>  

        |<span data-ttu-id="3e5dd-165">Tipo movimento</span><span class="sxs-lookup"><span data-stu-id="3e5dd-165">Entry Type</span></span>|<span data-ttu-id="3e5dd-166">Numero di articolo</span><span class="sxs-lookup"><span data-stu-id="3e5dd-166">Item Number</span></span>|<span data-ttu-id="3e5dd-167">Cod. ubicazione</span><span class="sxs-lookup"><span data-stu-id="3e5dd-167">Location Code</span></span>|<span data-ttu-id="3e5dd-168">Codice collocazione</span><span class="sxs-lookup"><span data-stu-id="3e5dd-168">Bin Code</span></span>|<span data-ttu-id="3e5dd-169">Quantità</span><span class="sxs-lookup"><span data-stu-id="3e5dd-169">Quantity</span></span>|  
        |----------------|-----------------|-------------------|--------------|--------------|  
        |<span data-ttu-id="3e5dd-170">Rettifica positiva</span><span class="sxs-lookup"><span data-stu-id="3e5dd-170">Positive Adjmt.</span></span>|<span data-ttu-id="3e5dd-171">1928-S</span><span class="sxs-lookup"><span data-stu-id="3e5dd-171">1928-S</span></span>|<span data-ttu-id="3e5dd-172">SUD</span><span class="sxs-lookup"><span data-stu-id="3e5dd-172">SOUTH</span></span>|<span data-ttu-id="3e5dd-173">S-01-0001</span><span class="sxs-lookup"><span data-stu-id="3e5dd-173">S-01-0001</span></span>|<span data-ttu-id="3e5dd-174">20</span><span class="sxs-lookup"><span data-stu-id="3e5dd-174">20</span></span>|  
        |<span data-ttu-id="3e5dd-175">Rettifica positiva</span><span class="sxs-lookup"><span data-stu-id="3e5dd-175">Positive Adjmt.</span></span>|<span data-ttu-id="3e5dd-176">1928-S</span><span class="sxs-lookup"><span data-stu-id="3e5dd-176">1928-S</span></span>|<span data-ttu-id="3e5dd-177">SUD</span><span class="sxs-lookup"><span data-stu-id="3e5dd-177">SOUTH</span></span>|<span data-ttu-id="3e5dd-178">S-01-0002</span><span class="sxs-lookup"><span data-stu-id="3e5dd-178">S-01-0002</span></span>|<span data-ttu-id="3e5dd-179">20</span><span class="sxs-lookup"><span data-stu-id="3e5dd-179">20</span></span>|  

        <span data-ttu-id="3e5dd-180">Per impostazione predefinita, il campo **Codice collocazione** nelle righe vendite sono nascosti, quindi occorre visualizzarlo.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-180">By default, the **Bin Code** field on the sales lines are hidden, so you must display it.</span></span> <span data-ttu-id="3e5dd-181">Per fare ciò è necessario personalizzare la pagina.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-181">To do this you need to personalize the page.</span></span> <span data-ttu-id="3e5dd-182">Per ulteriori informazioni, vedere [Per avviare la personalizzazione di una pagina tramite il banner Personalizzazione](ui-personalization-user.md#to-start-personalizing-a-page-through-the-personalizing-banner).</span><span class="sxs-lookup"><span data-stu-id="3e5dd-182">For more information, see [To start personalizing a page through the Personalizing banner](ui-personalization-user.md#to-start-personalizing-a-page-through-the-personalizing-banner).</span></span>

  3. <span data-ttu-id="3e5dd-183">Selezionare **Azioni**, quindi **Registrazione** e infine scegliere **Registra**.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-183">Choose **Actions**, then **Posting**, and then choose **Post**.</span></span>  
  4. <span data-ttu-id="3e5dd-184">Selezionare il pulsante **Sì**.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-184">Select the **Yes** button.</span></span>  

## <a name="creating-the-sales-order"></a><span data-ttu-id="3e5dd-185">Creazione dell'ordine di vendita</span><span class="sxs-lookup"><span data-stu-id="3e5dd-185">Creating the Sales Order</span></span>

<span data-ttu-id="3e5dd-186">Gli ordini di vendita sono il tipo più comune di documenti origine in uscita.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-186">Sales orders are the most common type of outbound source document.</span></span>  

### <a name="to-create-the-sales-order"></a><span data-ttu-id="3e5dd-187">Per creare l'ordine di vendita</span><span class="sxs-lookup"><span data-stu-id="3e5dd-187">To create the sales order</span></span>

1. <span data-ttu-id="3e5dd-188">Scegliere la terza icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Ordini vendita** e quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-188">Choose the ![Lightbulb that opens the Tell Me feature third](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>  
2. <span data-ttu-id="3e5dd-189">Scegliere l'azione **Nuovo**.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-189">Choose the **New** action.</span></span>  
3. <span data-ttu-id="3e5dd-190">Creare un ordine di vendita per il fornitore 10000 alla data di lavoro (23 gennaio) con la riga di ordine di vendita seguente.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-190">Create a sales order for customer 10000 on the work date (January 23) with the following sales order line.</span></span>  

    |<span data-ttu-id="3e5dd-191">Articolo</span><span class="sxs-lookup"><span data-stu-id="3e5dd-191">Item</span></span>|<span data-ttu-id="3e5dd-192">Cod. ubicazione</span><span class="sxs-lookup"><span data-stu-id="3e5dd-192">Location Code</span></span>|<span data-ttu-id="3e5dd-193">Quantità</span><span class="sxs-lookup"><span data-stu-id="3e5dd-193">Quantity</span></span>|  
    |----|-------------|--------|  
    |<span data-ttu-id="3e5dd-194">1928-S</span><span class="sxs-lookup"><span data-stu-id="3e5dd-194">1928-S</span></span>|<span data-ttu-id="3e5dd-195">SUD</span><span class="sxs-lookup"><span data-stu-id="3e5dd-195">SOUTH</span></span>|<span data-ttu-id="3e5dd-196">30</span><span class="sxs-lookup"><span data-stu-id="3e5dd-196">30</span></span>|  

     <span data-ttu-id="3e5dd-197">Comunicare alla warehouse che l'ordine di vendita è pronto per la gestione warehouse.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-197">Proceed to notify the warehouse that the sales order is ready for warehouse handling.</span></span>  

4. <span data-ttu-id="3e5dd-198">Scegliere l'azione **Rilascia**.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-198">Choose the **Release** action.</span></span>  

    <span data-ttu-id="3e5dd-199">Gianni procede al prelievo e alla spedizione degli articoli venduti.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-199">John proceeds to pick and ship the sold items.</span></span>  

## <a name="picking-and-shipping-items"></a><span data-ttu-id="3e5dd-200">Prelievo e spedizione articoli</span><span class="sxs-lookup"><span data-stu-id="3e5dd-200">Picking and Shipping Items</span></span>

<span data-ttu-id="3e5dd-201">Nella pagina **Prelievo magazzino** è possibile gestire tutte le attività di warehouse in uscita per un documento origine specifico, ad esempio un ordine di vendita.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-201">On the **Inventory Pick** page, you can manage all outbound warehouse activities for a specific source document, such as a sales order.</span></span> [!INCLUDE[tooltip-inline-tip_md](includes/tooltip-inline-tip_md.md)]  

### <a name="to-pick-and-ship-items"></a><span data-ttu-id="3e5dd-202">Per prelevare gli articoli e procedere alla spedizione</span><span class="sxs-lookup"><span data-stu-id="3e5dd-202">To pick and ship items</span></span>

1. <span data-ttu-id="3e5dd-203">Scegliere la quarta icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Prelievi magazzino** e quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-203">Choose the ![Lightbulb that opens the Tell Me feature fourth](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Inventory Picks**, and then choose the related link.</span></span>  
2. <span data-ttu-id="3e5dd-204">Scegliere l'azione **Nuovo**.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-204">Choose the **New** action.</span></span>  

    <span data-ttu-id="3e5dd-205">Assicurarsi che il campo **Nr.**</span><span class="sxs-lookup"><span data-stu-id="3e5dd-205">Make sure that the **No.**</span></span> <span data-ttu-id="3e5dd-206">della Scheda dettaglio **Generale** sia compilato.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-206">field on the **General** FastTab is filled in.</span></span>
3. <span data-ttu-id="3e5dd-207">Selezionare il campo **Documento origine**, quindi selezionare **Ordine vendita**.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-207">Select the **Source Document** field, and then select **Sales Order**.</span></span>  
4. <span data-ttu-id="3e5dd-208">Selezionare il campo **Nr. origine**, selezionare la riga per la vendita al cliente 10000 e fare clic sul pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-208">Select the **Source No.** field, select the line for the sale to customer 10000, and then choose the **OK** button.</span></span>  

    <span data-ttu-id="3e5dd-209">In alternativa, scegliere l'azione **Prendi documento origine**, quindi selezionare l'ordine di vendita.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-209">Alternatively, choose the **Get Source Document** action, and then select the sales order.</span></span>  
5. <span data-ttu-id="3e5dd-210">Scegliere l'azione **Autocompil. qtà da gestire**.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-210">Choose the **Autofill Qty. to Handle** action.</span></span>  

    <span data-ttu-id="3e5dd-211">In alternativa, nel campo **Qtà da gestire** immettere 10 e 20 rispettivamente nelle due righe di prelievo magazzino.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-211">Alternatively, in the **Qty. to Handle** field, enter 10 and 20 respectively on the two inventory pick lines.</span></span>  
6. <span data-ttu-id="3e5dd-212">Scegliere l'azione **Registra**, selezionare **Spedizione**, quindi scegliere il pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-212">Choose the **Post** action, select **Ship**, and then choose the **OK** button.</span></span>  

    <span data-ttu-id="3e5dd-213">Le 30 Lampade Amsterdam ora sono registrate come prelevati dalle collocazioni S-01-0001 e S-01-0002 e viene creato un movimento contabile articolo negativo che riflette la spedizione di vendita registrata.</span><span class="sxs-lookup"><span data-stu-id="3e5dd-213">The 30 Amsterdam Lamps are now registered as picked from bins S-01-0001 and S-01-0002, and a negative item ledger entry is created reflecting the posted sales shipment.</span></span>  

## <a name="see-also"></a><span data-ttu-id="3e5dd-214">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="3e5dd-214">See Also</span></span>

[<span data-ttu-id="3e5dd-215">Prelevare articoli con prelievi magazzino</span><span class="sxs-lookup"><span data-stu-id="3e5dd-215">Pick Items with Inventory Picks</span></span>](warehouse-how-to-pick-items-with-inventory-picks.md)  
[<span data-ttu-id="3e5dd-216">Prelevare articoli per la spedizione warehouse</span><span class="sxs-lookup"><span data-stu-id="3e5dd-216">Pick Items for Warehouse Shipment</span></span>](warehouse-how-to-pick-items-for-warehouse-shipment.md)  
[<span data-ttu-id="3e5dd-217">Impostare le warehouse di base con aree di operazioni</span><span class="sxs-lookup"><span data-stu-id="3e5dd-217">Set Up Basic Warehouses with Operations Areas</span></span>](warehouse-how-to-set-up-basic-warehouses-with-operations-areas.md)  
[<span data-ttu-id="3e5dd-218">Spostare componenti in un'area di operazione nelle configurazioni di warehouse di base</span><span class="sxs-lookup"><span data-stu-id="3e5dd-218">Move Components to an Operation Area in Basic Warehouse Configurations</span></span>](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md)  
[<span data-ttu-id="3e5dd-219">Prelevare per la produzione o l'assemblaggio</span><span class="sxs-lookup"><span data-stu-id="3e5dd-219">Pick for Production or Assembly</span></span>](warehouse-how-to-pick-for-production.md)  
[<span data-ttu-id="3e5dd-220">Spostare articoli ad hoc nelle configurazioni della warehouse di base</span><span class="sxs-lookup"><span data-stu-id="3e5dd-220">Move Items Ad Hoc in Basic Warehouse Configurations</span></span>](warehouse-how-to-move-items-ad-hoc-in-basic-warehousing.md)  
[<span data-ttu-id="3e5dd-221">Dettagli di progettazione: Flusso warehouse in uscita</span><span class="sxs-lookup"><span data-stu-id="3e5dd-221">Design Details: Outbound Warehouse Flow</span></span>](design-details-outbound-warehouse-flow.md)  
[<span data-ttu-id="3e5dd-222">Procedure dettagliate per i processi aziendali</span><span class="sxs-lookup"><span data-stu-id="3e5dd-222">Business Process Walkthroughs</span></span>](walkthrough-business-process-walkthroughs.md)  
<span data-ttu-id="3e5dd-223">[Utilizzo di [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="3e5dd-223">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  


[!INCLUDE[footer-include](includes/footer-banner.md)]
