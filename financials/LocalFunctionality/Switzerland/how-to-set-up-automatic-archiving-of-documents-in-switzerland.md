---
title: Come impostare l'archiviazione automatica dei documenti in Svizzera
description: "È possibile impostare l'archiviazione automatica di documenti di vendita e di acquisto, ad esempio offerte, ordini programmati e ordini, prima di eliminarli."
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
ms.sourcegitcommit: b34f276a764f0e828fbc1f015429df9852242a4c
ms.openlocfilehash: 09fca5cba94bed83b862cd8bb9d4b5be895c509d
ms.contentlocale: it-ch
ms.lasthandoff: 03/22/2018

---
# <a name="set-up-automatic-archiving-of-documents-in-switzerland"></a><span data-ttu-id="40626-103">Impostare l'archiviazione automatica dei documenti in Svizzera</span><span class="sxs-lookup"><span data-stu-id="40626-103">Set Up Automatic Archiving of Documents in Switzerland</span></span>
<span data-ttu-id="40626-104">È possibile impostare l'archiviazione automatica di documenti di vendita e di acquisto, ad esempio offerte, ordini programmati e ordini, prima di eliminarli.</span><span class="sxs-lookup"><span data-stu-id="40626-104">You can set up automatic archiving of sales documents and purchase documents—such as quotes, blanket orders, and orders—before you delete documents.</span></span>  

<span data-ttu-id="40626-105">La procedura seguente descrive come impostare l'archiviazione automatica dei documenti di vendita, ma gli stessi passaggi si applicano anche a documenti di acquisto.</span><span class="sxs-lookup"><span data-stu-id="40626-105">The following procedure describes how to set up automatic archiving of sales documents, but the same steps apply to purchase documents.</span></span>  

## <a name="to-set-up-automatic-archiving-of-documents"></a><span data-ttu-id="40626-106">Per impostare l'archiviazione automatica dei documenti</span><span class="sxs-lookup"><span data-stu-id="40626-106">To set up automatic archiving of documents</span></span>  

1.  <span data-ttu-id="40626-107">Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Setup contabilità clienti e vendite**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="40626-107">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales & Receivables Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="40626-108">Nella Scheda dettaglio **Archiviazione** della finestra **Setup contabilità clienti e vendite** compilare i campi come descritto nella tabella riportata di seguito.</span><span class="sxs-lookup"><span data-stu-id="40626-108">On the **Sales & Receivables Setup** window, on the **Archiving** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="40626-109">Campo</span><span class="sxs-lookup"><span data-stu-id="40626-109">Field</span></span>|<span data-ttu-id="40626-110">Descrizione</span><span class="sxs-lookup"><span data-stu-id="40626-110">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="40626-111">**Archiviazione Offerta Vendita**</span><span class="sxs-lookup"><span data-stu-id="40626-111">**Archiving Sales Quote**</span></span>|<span data-ttu-id="40626-112">**Mai** per non archiviare mai offerte di vendita quando vengono eliminate.</span><span class="sxs-lookup"><span data-stu-id="40626-112">**Never** to never archive sales quotes when they are deleted.</span></span><br /><br /> <span data-ttu-id="40626-113">-o-</span><span class="sxs-lookup"><span data-stu-id="40626-113">–or–</span></span><br /><br /> <span data-ttu-id="40626-114">**Domanda** per chiedere all'utente di scegliere se archiviare le offerte di vendita quando vengono eliminate.</span><span class="sxs-lookup"><span data-stu-id="40626-114">**Question** to prompt the user to choose whether to archive sales quotes when they are deleted.</span></span><br /><br /> <span data-ttu-id="40626-115">-o-</span><span class="sxs-lookup"><span data-stu-id="40626-115">–or–</span></span><br /><br /> <span data-ttu-id="40626-116">**Sempre** per non archiviare automaticamente le offerte di vendita quando vengono eliminate.</span><span class="sxs-lookup"><span data-stu-id="40626-116">**Always** to archive sales quotes automatically when they are deleted.</span></span>|  
    |<span data-ttu-id="40626-117">**Archiviazione ordini di vendita programmati**</span><span class="sxs-lookup"><span data-stu-id="40626-117">**Archiving Blanket Sales Orders**</span></span>|<span data-ttu-id="40626-118">Selezionare questa opzione per archiviare automaticamente gli ordini di vendita programmati ogni volta che vengono eliminati.</span><span class="sxs-lookup"><span data-stu-id="40626-118">Select to archive blanket sales orders automatically each time they are deleted.</span></span>|  
    |<span data-ttu-id="40626-119">**Ordini archiviati e ordini di reso**</span><span class="sxs-lookup"><span data-stu-id="40626-119">**Arch. Orders and Ret. Orders**</span></span>|<span data-ttu-id="40626-120">Selezionare questa opzione per archiviare automaticamente gli ordini di vendita ogni volta che vengono eliminati.</span><span class="sxs-lookup"><span data-stu-id="40626-120">Select to automatically archive sales orders each time they are deleted.</span></span>|  
    |<span data-ttu-id="40626-121">**Log interazione automatico**</span><span class="sxs-lookup"><span data-stu-id="40626-121">**Automatic Interaction Log**</span></span>|<span data-ttu-id="40626-122">Selezionare questa opzione per creare automaticamente un movimento per il contatto nel log interazione quando viene registrato un ordine di vendita o una spedizione parziale o quando un'offerta di vendita viene convertita in un ordine di vendita.</span><span class="sxs-lookup"><span data-stu-id="40626-122">Select to automatically create an entry for the contact in the interaction log when a sales order or partial shipment is posted, or when a sales quote is converted into a sales order.</span></span> <span data-ttu-id="40626-123">**Nota**: questo campo non è disponibile nella pagina **Setup contabilità fornitori e acquisti**.</span><span class="sxs-lookup"><span data-stu-id="40626-123">**Note:**  This field is not available on the **Purchases & Payables Setup** page.</span></span>|  

3.  <span data-ttu-id="40626-124">Scegliere il pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="40626-124">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="40626-125">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="40626-125">See Also</span></span>  
 <span data-ttu-id="40626-126">[Documenti di acquisto e di vendita per la Svizzera](swiss-purchase-documents-and-sales-documents.md) </span><span class="sxs-lookup"><span data-stu-id="40626-126">[Swiss Purchase Documents and Sales Documents](swiss-purchase-documents-and-sales-documents.md) </span></span>  
 <span data-ttu-id="40626-127">[Importare codici postali svizzeri](how-to-import-swiss-post-codes.md) </span><span class="sxs-lookup"><span data-stu-id="40626-127">[Import Swiss Post Codes](how-to-import-swiss-post-codes.md) </span></span>  
 <span data-ttu-id="40626-128">[Stampare una lista prelievi magazzino da un ordine di vendita](how-to-print-an-inventory-picking-list-from-a-sales-order.md) </span><span class="sxs-lookup"><span data-stu-id="40626-128">[Print an Inventory Picking List from a Sales Order](how-to-print-an-inventory-picking-list-from-a-sales-order.md) </span></span>  
 [<span data-ttu-id="40626-129">Stampare ordini di vendita e acquisto durante la registrazione batch</span><span class="sxs-lookup"><span data-stu-id="40626-129">Print Sales and Purchase Orders During Batch Posting</span></span>](how-to-print-sales-and-purchase-orders-during-batch-posting.md)

