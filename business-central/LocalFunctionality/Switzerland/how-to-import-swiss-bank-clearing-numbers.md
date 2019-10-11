---
title: Come importare numeri di clearing bancari svizzeri
description: I numeri di clearing bancari sono numeri univoci usati per identificare ogni agenzia o filiale nella directory delle banche. Questa informazioni è necessaria per effettuare un pagamento elettronico. Il file può essere scaricato dal sito Web SIX Interbank Clearing.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 3b2bcbe6baaf833c1f6bd17d26805420a605591e
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 10/01/2019
ms.locfileid: "2301033"
---
# <a name="import-swiss-bank-clearing-numbers"></a><span data-ttu-id="d651e-105">Importare numeri di clearing svizzeri</span><span class="sxs-lookup"><span data-stu-id="d651e-105">Import Swiss Bank Clearing Numbers</span></span>
<span data-ttu-id="d651e-106">I numeri di clearing bancari sono numeri univoci usati per identificare ogni agenzia o filiale nella directory delle banche.</span><span class="sxs-lookup"><span data-stu-id="d651e-106">Bank clearing numbers are unique numbers used to identify each bank agency or branch in the bank directory.</span></span> <span data-ttu-id="d651e-107">Questa informazioni è necessaria per effettuare un pagamento elettronico.</span><span class="sxs-lookup"><span data-stu-id="d651e-107">This information is required for electronic payment.</span></span> <span data-ttu-id="d651e-108">Il file può essere scaricato dal sito Web [SIX Interbank Clearing](https://go.microsoft.com/fwlink/?LinkId=145121).</span><span class="sxs-lookup"><span data-stu-id="d651e-108">The file can be downloaded from the [SIX Interbank Clearing](https://go.microsoft.com/fwlink/?LinkId=145121) website.</span></span>  

<span data-ttu-id="d651e-109">È possibile importare il file Bank Master di numeri di clearing, ovvero il file ufficiale dei numeri di clearing bancari, per aggiornare le informazioni sui numeri di clearing nella directory delle banche.</span><span class="sxs-lookup"><span data-stu-id="d651e-109">You can import the BC Bank Master file—the official Swiss bank clearing number file—to update the bank clearing number information in the bank directory.</span></span> <span data-ttu-id="d651e-110">Quando si importa il file dei numeri di clearing bancari, i dati vengono inseriti nella tabella **Directory banche** e i dati esistenti vengono sovrascritti.</span><span class="sxs-lookup"><span data-stu-id="d651e-110">When you import the bank clearing number file, the data is imported to the **Bank Directory** table, and the existing data is overwritten.</span></span> <span data-ttu-id="d651e-111">Dopo aver importato il file dei numeri di clearing bancari, è possibile definire il numero di filiale aggiornato per clienti e fornitori.</span><span class="sxs-lookup"><span data-stu-id="d651e-111">After importing the bank clearing number file, you can define the updated bank branch number for customers and vendors.</span></span> <span data-ttu-id="d651e-112">Per ulteriori informazioni, vedere le tabelle Conti correnti clienti e Conti correnti fornitori.</span><span class="sxs-lookup"><span data-stu-id="d651e-112">For more information, see the Customer Bank Account table and the Vendor Bank Account table.</span></span>  

## <a name="to-import-swiss-bank-clearing-numbers"></a><span data-ttu-id="d651e-113">Per importare numeri di clearing svizzeri</span><span class="sxs-lookup"><span data-stu-id="d651e-113">To import Swiss bank clearing numbers</span></span>  

1.  <span data-ttu-id="d651e-114">Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Directory banche**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="d651e-114">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Directory**, and choose the related link.</span></span>  
2.  <span data-ttu-id="d651e-115">Scegliere l'azione **Importa directory banche**.</span><span class="sxs-lookup"><span data-stu-id="d651e-115">Choose the **Import Bank Directory** action.</span></span>  
3.  <span data-ttu-id="d651e-116">Nella pagina **Importa directory banche**, nella Scheda dettaglio **Opzioni** selezionare il campo **Aggiorna automaticamente numeri di clearing** per aggiornare i numeri di clearing bancari in modo automatico.</span><span class="sxs-lookup"><span data-stu-id="d651e-116">On the **Import Bank Directory** page, on the **Options** FastTab, select the **Automatically Update Clearing Numbers** field to update the bank clearing numbers automatically.</span></span>  
4.  <span data-ttu-id="d651e-117">Scegliere il pulsante **Stampa** o il pulsante **Anteprima** per importare i numeri di clearing bancari, quindi nella pagina **Apri** individuare il file scaricato dal sito Web SIX Interbank Clearing.</span><span class="sxs-lookup"><span data-stu-id="d651e-117">Choose the **Print** button or the **Preview** button to import the bank clearing numbers, and then, on the **Open** page, locate the file that you have downloaded from the SIX Interbank Clearing website.</span></span>
5. <span data-ttu-id="d651e-118">Scegliere il pulsante **Apri**.</span><span class="sxs-lookup"><span data-stu-id="d651e-118">Choose the **Open** button.</span></span>  

    <span data-ttu-id="d651e-119">Se si sceglie il pulsante **Stampa**, il contenuto del file verrà stampato.</span><span class="sxs-lookup"><span data-stu-id="d651e-119">If you choose the **Print** button, the contents of the file will be printed.</span></span> <span data-ttu-id="d651e-120">Se si sceglie il pulsante **Anteprima**, la tabella **Directory banche** verrà aggiornata e verrà visualizzato un report con i numeri di clearing modificati.</span><span class="sxs-lookup"><span data-stu-id="d651e-120">If you choose the **Preview** button, the **Bank Directory** table will be updated and a report that has clearing numbers that have changed will be displayed.</span></span>  

<span data-ttu-id="d651e-121">La procedura seguente descrive come definire i numeri di filiale bancaria per i conti correnti dei clienti, ma gli stessi passaggi si applicano anche per definire i numeri di filiale per i conti correnti dei fornitori.</span><span class="sxs-lookup"><span data-stu-id="d651e-121">The following procedure describes how to define bank branch numbers for customer bank accounts, but the same steps also apply for defining bank branch numbers for vendor bank accounts.</span></span>  

## <a name="to-define-bank-branch-numbers-for-customer-bank-accounts"></a><span data-ttu-id="d651e-122">Per definire i numeri di filiale bancaria per i conti correnti dei clienti</span><span class="sxs-lookup"><span data-stu-id="d651e-122">To define bank branch numbers for customer bank accounts</span></span>  

1.  <span data-ttu-id="d651e-123">Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Clienti**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="d651e-123">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Customers**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="d651e-124">Selezionare il cliente per cui creare informazioni di conto corrente, quindi scegliere l'azione **C/C bancari**.</span><span class="sxs-lookup"><span data-stu-id="d651e-124">Select the customer for whom you want to create bank account information, and then choose the **Bank Accounts** action.</span></span>  
3.  <span data-ttu-id="d651e-125">Nella pagina **Lista C/C bancari clienti**, selezionare il conto corrente bancario richiesto e scegliere l'azione **Modifica**.</span><span class="sxs-lookup"><span data-stu-id="d651e-125">On the **Customer Bank Account List** page, select the required bank account, and then choose the **Edit** action.</span></span>  
4.  <span data-ttu-id="d651e-126">Nella scheda dettaglio **Generale**, nel campo **Nr. filiale banca**</span><span class="sxs-lookup"><span data-stu-id="d651e-126">On the **General** FastTab, in the **Bank Branch No.**</span></span> <span data-ttu-id="d651e-127">selezionare il numero dell'agenza o filiale bancaria.</span><span class="sxs-lookup"><span data-stu-id="d651e-127">field, select the number of the bank agency or branch.</span></span>  
5.  <span data-ttu-id="d651e-128">Scegliere il pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="d651e-128">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="d651e-129">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="d651e-129">See Also</span></span>  
 <span data-ttu-id="d651e-130">[Pagamenti elettronici svizzeri](swiss-electronic-payments.md) </span><span class="sxs-lookup"><span data-stu-id="d651e-130">[Swiss Electronic Payments](swiss-electronic-payments.md) </span></span>  
 [<span data-ttu-id="d651e-131">Impostare i conti correnti bancari</span><span class="sxs-lookup"><span data-stu-id="d651e-131">Set Up Bank Accounts</span></span>](../../bank-how-setup-bank-accounts.md)
