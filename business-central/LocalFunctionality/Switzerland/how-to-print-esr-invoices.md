---
title: 'Procedura: Stampare fatture ESR'
description: "È possibile stampare il bollettino bancario ESR (Einzahlungsschein mit Referenznummer) in diversi modi."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: c614162bcb0146a740152ed03939b8f16112e9ff
ms.contentlocale: it-ch
ms.lasthandoff: 09/28/2018

---
# <a name="print-esr-invoices"></a><span data-ttu-id="1ca5e-103">Stampare fatture ESR</span><span class="sxs-lookup"><span data-stu-id="1ca5e-103">Print ESR Invoices</span></span>
<span data-ttu-id="1ca5e-104">È possibile stampare il bollettino bancario ESR (Einzahlungsschein mit Referenznummer) nei seguenti modi:</span><span class="sxs-lookup"><span data-stu-id="1ca5e-104">You can print an Einzahlungsschein mit Referenznummer (ESR) payment slip in the following ways:</span></span>  

- <span data-ttu-id="1ca5e-105">Incluso nell'ESR della fattura di vendita.</span><span class="sxs-lookup"><span data-stu-id="1ca5e-105">As part of the sales invoice ESR.</span></span>  
- <span data-ttu-id="1ca5e-106">Come documento separato chiamato tagliando ESR.</span><span class="sxs-lookup"><span data-stu-id="1ca5e-106">As a separate document called an ESR coupon.</span></span>  

<span data-ttu-id="1ca5e-107">Il report ESR della fattura di vendita corrisponde alla fattura di vendita accompagnata da un tagliando ESR aggiuntivo.</span><span class="sxs-lookup"><span data-stu-id="1ca5e-107">The sales invoice ESR report corresponds with the sales invoice that is accompanied by an additional ESR coupon.</span></span> <span data-ttu-id="1ca5e-108">Utilizzando il report tagliando ESR di vendita è possibile stampare la distinta di deposito blu.</span><span class="sxs-lookup"><span data-stu-id="1ca5e-108">By using the sales ESR coupon report, you can print the blue deposit slip.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="1ca5e-109">È necessario selezionare una stampante e selezionare le impostazioni durante l'installazione del modulo di pagamento ESR per stampare correttamente la distinta di deposito.</span><span class="sxs-lookup"><span data-stu-id="1ca5e-109">You must select a printer and select settings during the ESR payment module installation to print the deposit slip correctly.</span></span> <span data-ttu-id="1ca5e-110">Per ulteriori informazioni, vedere la tabella Selezioni stampante.</span><span class="sxs-lookup"><span data-stu-id="1ca5e-110">For more information, see the Printer Selection table.</span></span>  

<span data-ttu-id="1ca5e-111">La procedura seguente descrive come stampare le fatture di vendita ESR, ma gli stessi passaggi si applicano anche alla stampa dei tagliandi ESR.</span><span class="sxs-lookup"><span data-stu-id="1ca5e-111">The following procedure describes how to print ESR sales invoices, but the same steps also apply for printing ESR coupons.</span></span>  

## <a name="to-print-esr-invoices"></a><span data-ttu-id="1ca5e-112">Per stampare fatture ESR</span><span class="sxs-lookup"><span data-stu-id="1ca5e-112">To print ESR invoices</span></span>  

1.  <span data-ttu-id="1ca5e-113">Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Fattura ESR**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="1ca5e-113">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Invoice ESR**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="1ca5e-114">Nel processo batch **Fattura di vendita ESR**, nella Scheda dettaglio **Opzioni** compilare i campi come descritto nella tabella seguente.</span><span class="sxs-lookup"><span data-stu-id="1ca5e-114">In the **Sales Invoice ESR** batch job, on the **Options** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="1ca5e-115">Campo</span><span class="sxs-lookup"><span data-stu-id="1ca5e-115">Field</span></span>|<span data-ttu-id="1ca5e-116">Descrizione</span><span class="sxs-lookup"><span data-stu-id="1ca5e-116">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="1ca5e-117">**Nr di copie**</span><span class="sxs-lookup"><span data-stu-id="1ca5e-117">**No. of copies**</span></span>|<span data-ttu-id="1ca5e-118">Immettere il numero richiesto di copie del report.</span><span class="sxs-lookup"><span data-stu-id="1ca5e-118">Enter the required number of report copies.</span></span>|  
    |<span data-ttu-id="1ca5e-119">**Banca ESR**</span><span class="sxs-lookup"><span data-stu-id="1ca5e-119">**ESR Bank**</span></span>|<span data-ttu-id="1ca5e-120">Selezionare il codice bancario ESR da stampare nel report.</span><span class="sxs-lookup"><span data-stu-id="1ca5e-120">Select the ESR bank code that is to be printed in the report.</span></span><br /><br /> <span data-ttu-id="1ca5e-121">Se il valore in questo campo è <Blank> e il codice del metodo di pagamento ESF non è definito nella finestra **Setup ESR**, verrà stampata la banca principale ESR selezionata nella finestra **Setup ESR**.</span><span class="sxs-lookup"><span data-stu-id="1ca5e-121">If the value in this field is <Blank> and the ESR payment method code is not defined in the **ESR Setup** window, then the ESR main bank selected in the **ESR Setup** window will be printed.</span></span>|  
    |<span data-ttu-id="1ca5e-122">**LogInteraction**</span><span class="sxs-lookup"><span data-stu-id="1ca5e-122">**LogInteraction**</span></span>|<span data-ttu-id="1ca5e-123">Specificare se le interazioni con i tuoi contatti verranno registrate.</span><span class="sxs-lookup"><span data-stu-id="1ca5e-123">Specify if the interactions that you have with your contacts will be logged.</span></span>|  
    |<span data-ttu-id="1ca5e-124">**Sistema ESR**</span><span class="sxs-lookup"><span data-stu-id="1ca5e-124">**ESR System**</span></span>|<span data-ttu-id="1ca5e-125">Selezionare il sistema ESR con cui è possibile inviare i nuovi tagliandi ESR ai clienti.</span><span class="sxs-lookup"><span data-stu-id="1ca5e-125">Select the ESR system through which you can send new ESR coupons to customers.</span></span> <span data-ttu-id="1ca5e-126">Per utilizzare il sistema ESR utilizzato dalla banca che hai specificato nel campo **Banca ESR**, selezionare **Basato su banca ESR**.</span><span class="sxs-lookup"><span data-stu-id="1ca5e-126">To use the ESR system that is used by the bank that you have specified in **ESR Bank** field, select **Based on ESR Bank**.</span></span>|  

3.  <span data-ttu-id="1ca5e-127">Scegliere il pulsante **Stampa** per stampare il report oppure scegliere il pulsante **Anteprima** per visualizzarlo sullo schermo.</span><span class="sxs-lookup"><span data-stu-id="1ca5e-127">Choose the **Print** button to print the report or choose the **Preview** button to view it on the screen.</span></span>  

<span data-ttu-id="1ca5e-128">È inoltre possibile ristampare il report ESR della fattura di vendita o il report del tagliando ESR di vendita.</span><span class="sxs-lookup"><span data-stu-id="1ca5e-128">You can also reprint the sales invoice ESR report or sales ESR coupon report.</span></span>  

## <a name="see-also"></a><span data-ttu-id="1ca5e-129">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="1ca5e-129">See Also</span></span>  
 <span data-ttu-id="1ca5e-130">[Pagamenti elettronici svizzeri tramite ESR](swiss-electronic-payments-using-esr.md) </span><span class="sxs-lookup"><span data-stu-id="1ca5e-130">[Swiss Electronic Payments Using ESR](swiss-electronic-payments-using-esr.md) </span></span>  
 [<span data-ttu-id="1ca5e-131">Importare i pagamenti ESR</span><span class="sxs-lookup"><span data-stu-id="1ca5e-131">Import ESR Payments</span></span>](how-to-import-esr-payments.md)

