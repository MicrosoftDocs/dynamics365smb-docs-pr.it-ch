---
title: 'Procedura: Importare codici postali svizzeri'
description: È possibile importare l'ultimo file di codice postale e utilizzarlo per aggiornare la tabella CAP. Il file di codice postale può essere scaricato dal sito Web dei codici postali svizzeri. Dopo l'importazione del codice postale più recente, è possibile definire i codici postali per i clienti o i fornitori.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: e28c04fd4d59bc099ab2a051129a05d9a01ef4bb
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 04/01/2020
ms.locfileid: "3189119"
---
# <a name="import-swiss-post-codes"></a><span data-ttu-id="af2a9-105">Importare codici postali svizzeri</span><span class="sxs-lookup"><span data-stu-id="af2a9-105">Import Swiss Post Codes</span></span>
<span data-ttu-id="af2a9-106">È possibile importare l'ultimo file di codice postale e utilizzarlo per aggiornare la tabella **CAP**.</span><span class="sxs-lookup"><span data-stu-id="af2a9-106">You can import the latest post code file and use it to update the **Post Code** table.</span></span> <span data-ttu-id="af2a9-107">Il file di codice postale può essere scaricato dal sito Web dei [codici postali svizzeri](https://go.microsoft.com/fwlink/?LinkId=150292).</span><span class="sxs-lookup"><span data-stu-id="af2a9-107">The post code file can be downloaded from the [Swiss Post](https://go.microsoft.com/fwlink/?LinkId=150292) website.</span></span> <span data-ttu-id="af2a9-108">Dopo l'importazione del codice postale più recente, è possibile definire i codici postali per i clienti o i fornitori.</span><span class="sxs-lookup"><span data-stu-id="af2a9-108">After importing the latest post code, you can define post codes for customers or vendors.</span></span> <span data-ttu-id="af2a9-109">Per ulteriori informazioni, vedere [Registrare nuovi fornitori](../../purchasing-how-register-new-vendors.md).</span><span class="sxs-lookup"><span data-stu-id="af2a9-109">For more information, see [Register New Vendors](../../purchasing-how-register-new-vendors.md).</span></span>  

## <a name="to-import-post-codes"></a><span data-ttu-id="af2a9-110">Per importare i codici postali</span><span class="sxs-lookup"><span data-stu-id="af2a9-110">To import post codes</span></span>  

1.  <span data-ttu-id="af2a9-111">Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "Icona della funzionalità Cerca pagina o report"), immettere **NPA**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="af2a9-111">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Post Codes**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="af2a9-112">Selezionare l'azione **Importa codici postali**.</span><span class="sxs-lookup"><span data-stu-id="af2a9-112">Choose the **Import Post Codes** action.</span></span>  
3.  <span data-ttu-id="af2a9-113">Nella pagina **Importa codici postali** nel campo **Nome file** immettere il nome del file di codice postale da importare nella tabella **CAP**.</span><span class="sxs-lookup"><span data-stu-id="af2a9-113">On the **Import Post Codes** page, in the **Filename** field, enter the name of the post code file that you want to import to the **Post Code** table.</span></span>  
4.  <span data-ttu-id="af2a9-114">Scegliere il pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="af2a9-114">Choose the **OK** button.</span></span>  

    <span data-ttu-id="af2a9-115">Le informazioni più recenti sui codici postali vengono importate.</span><span class="sxs-lookup"><span data-stu-id="af2a9-115">The latest post code information is imported.</span></span>  

<span data-ttu-id="af2a9-116">Di seguito viene descritto come definire i codici postali per i clienti, ma gli stessi passaggi si applicano anche per definire i codici postali per i fornitori.</span><span class="sxs-lookup"><span data-stu-id="af2a9-116">The following procedure describes how to define post codes for customers, but the same steps also apply to defining post codes for vendors.</span></span>  

## <a name="to-define-post-codes-for-customers"></a><span data-ttu-id="af2a9-117">Per definire i codici postali per i clienti</span><span class="sxs-lookup"><span data-stu-id="af2a9-117">To define post codes for customers</span></span>  

1.  <span data-ttu-id="af2a9-118">Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "Icona della funzionalità Cerca pagina o report"), immettere **Clienti**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="af2a9-118">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Customers**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="af2a9-119">Selezionare il cliente per cui definire un codice postale, quindi scegliere l'azione **Modifica**.</span><span class="sxs-lookup"><span data-stu-id="af2a9-119">Select the customer for whom you want to define a post code, and then choose the **Edit** action.</span></span>  
3.  <span data-ttu-id="af2a9-120">Nella Scheda dettaglio **Generale** della pagina **Scheda cliente**, nel campo **CAP** selezionare il codice postale per l'indirizzo del cliente.</span><span class="sxs-lookup"><span data-stu-id="af2a9-120">On the **Customer Card** page, on the **General** FastTab, in the **Post Code** field, select the post code for the customer's address.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="af2a9-121">Una volta selezionato il codice postale, i campi **Città** e **Codice paese** vengono popolati automaticamente con le informazioni della tabella **CAP**.</span><span class="sxs-lookup"><span data-stu-id="af2a9-121">When you select the post code, the **City** and **Country/Region Code** fields populate automatically with the information from the **Post Code** table.</span></span> <span data-ttu-id="af2a9-122">Per ulteriori informazioni, vedere [Registrare nuovi clienti](../../sales-how-register-new-customers.md).</span><span class="sxs-lookup"><span data-stu-id="af2a9-122">For more information, see [Register New Customers](../../sales-how-register-new-customers.md).</span></span>  

4.  <span data-ttu-id="af2a9-123">Scegliere il pulsante **OK**.</span><span class="sxs-lookup"><span data-stu-id="af2a9-123">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="af2a9-124">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="af2a9-124">See Also</span></span>   
 <span data-ttu-id="af2a9-125">[Documenti di acquisto e di vendita per la Svizzera](swiss-purchase-documents-and-sales-documents.md) </span><span class="sxs-lookup"><span data-stu-id="af2a9-125">[Swiss Purchase Documents and Sales Documents](swiss-purchase-documents-and-sales-documents.md) </span></span>  
 <span data-ttu-id="af2a9-126">[Stampare una lista prelievi magazzino da un ordine di vendita](how-to-print-an-inventory-picking-list-from-a-sales-order.md) </span><span class="sxs-lookup"><span data-stu-id="af2a9-126">[Print an Inventory Picking List from a Sales Order](how-to-print-an-inventory-picking-list-from-a-sales-order.md) </span></span>  
 [<span data-ttu-id="af2a9-127">Registrare nuovi fornitori</span><span class="sxs-lookup"><span data-stu-id="af2a9-127">Register New Vendors</span></span>](../../purchasing-how-register-new-vendors.md)  
