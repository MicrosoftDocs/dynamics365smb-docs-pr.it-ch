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
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: 9f345827f1cc705727f80d21a00839f221044059
ms.contentlocale: it-ch
ms.lasthandoff: 11/26/2018

---
# <a name="print-esr-invoices"></a><span data-ttu-id="65f46-103">Stampare fatture ESR</span><span class="sxs-lookup"><span data-stu-id="65f46-103">Print ESR Invoices</span></span>
<span data-ttu-id="65f46-104">È possibile stampare il bollettino bancario ESR (Einzahlungsschein mit Referenznummer) nei seguenti modi:</span><span class="sxs-lookup"><span data-stu-id="65f46-104">You can print an Einzahlungsschein mit Referenznummer (ESR) payment slip in the following ways:</span></span>  

- <span data-ttu-id="65f46-105">Incluso nell'ESR della fattura di vendita.</span><span class="sxs-lookup"><span data-stu-id="65f46-105">As part of the sales invoice ESR.</span></span>  
- <span data-ttu-id="65f46-106">Come documento separato chiamato tagliando ESR.</span><span class="sxs-lookup"><span data-stu-id="65f46-106">As a separate document called an ESR coupon.</span></span>  

<span data-ttu-id="65f46-107">Il report ESR della fattura di vendita corrisponde alla fattura di vendita accompagnata da un tagliando ESR aggiuntivo.</span><span class="sxs-lookup"><span data-stu-id="65f46-107">The sales invoice ESR report corresponds with the sales invoice that is accompanied by an additional ESR coupon.</span></span> <span data-ttu-id="65f46-108">Utilizzando il report tagliando ESR di vendita è possibile stampare la distinta di deposito blu.</span><span class="sxs-lookup"><span data-stu-id="65f46-108">By using the sales ESR coupon report, you can print the blue deposit slip.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="65f46-109">È necessario selezionare una stampante e selezionare le impostazioni durante l'installazione del modulo di pagamento ESR per stampare correttamente la distinta di deposito.</span><span class="sxs-lookup"><span data-stu-id="65f46-109">You must select a printer and select settings during the ESR payment module installation to print the deposit slip correctly.</span></span> <span data-ttu-id="65f46-110">Per ulteriori informazioni, vedere la tabella Selezioni stampante.</span><span class="sxs-lookup"><span data-stu-id="65f46-110">For more information, see the Printer Selection table.</span></span>  

<span data-ttu-id="65f46-111">La procedura seguente descrive come stampare le fatture di vendita ESR, ma gli stessi passaggi si applicano anche alla stampa dei tagliandi ESR.</span><span class="sxs-lookup"><span data-stu-id="65f46-111">The following procedure describes how to print ESR sales invoices, but the same steps also apply for printing ESR coupons.</span></span>  

## <a name="to-print-esr-invoices"></a><span data-ttu-id="65f46-112">Per stampare fatture ESR</span><span class="sxs-lookup"><span data-stu-id="65f46-112">To print ESR invoices</span></span>  

1.  <span data-ttu-id="65f46-113">Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Fattura ESR**, quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="65f46-113">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Invoice ESR**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="65f46-114">Nel processo batch **Fattura di vendita ESR**, nella Scheda dettaglio **Opzioni** compilare i campi come descritto nella tabella seguente.</span><span class="sxs-lookup"><span data-stu-id="65f46-114">In the **Sales Invoice ESR** batch job, on the **Options** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="65f46-115">Campo</span><span class="sxs-lookup"><span data-stu-id="65f46-115">Field</span></span>|<span data-ttu-id="65f46-116">Descrizione</span><span class="sxs-lookup"><span data-stu-id="65f46-116">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="65f46-117">**Nr di copie**</span><span class="sxs-lookup"><span data-stu-id="65f46-117">**No. of copies**</span></span>|<span data-ttu-id="65f46-118">Immettere il numero richiesto di copie del report.</span><span class="sxs-lookup"><span data-stu-id="65f46-118">Enter the required number of report copies.</span></span>|  
    |<span data-ttu-id="65f46-119">**Banca ESR**</span><span class="sxs-lookup"><span data-stu-id="65f46-119">**ESR Bank**</span></span>|<span data-ttu-id="65f46-120">Selezionare il codice bancario ESR da stampare nel report.</span><span class="sxs-lookup"><span data-stu-id="65f46-120">Select the ESR bank code that is to be printed in the report.</span></span><br /><br /> <span data-ttu-id="65f46-121">Se il valore in questo campo è <Blank> e il codice del metodo di pagamento ESF non è definito nella pagina **Setup ESR**, verrà stampata la banca principale ESR selezionata nella pagina **Setup ESR**.</span><span class="sxs-lookup"><span data-stu-id="65f46-121">If the value in this field is <Blank> and the ESR payment method code is not defined on the **ESR Setup** page, then the ESR main bank selected on the **ESR Setup** page will be printed.</span></span>|  
    |<span data-ttu-id="65f46-122">**LogInteraction**</span><span class="sxs-lookup"><span data-stu-id="65f46-122">**LogInteraction**</span></span>|<span data-ttu-id="65f46-123">Specificare se le interazioni con i tuoi contatti verranno registrate.</span><span class="sxs-lookup"><span data-stu-id="65f46-123">Specify if the interactions that you have with your contacts will be logged.</span></span>|  
    |<span data-ttu-id="65f46-124">**Sistema ESR**</span><span class="sxs-lookup"><span data-stu-id="65f46-124">**ESR System**</span></span>|<span data-ttu-id="65f46-125">Selezionare il sistema ESR con cui è possibile inviare i nuovi tagliandi ESR ai clienti.</span><span class="sxs-lookup"><span data-stu-id="65f46-125">Select the ESR system through which you can send new ESR coupons to customers.</span></span> <span data-ttu-id="65f46-126">Per utilizzare il sistema ESR utilizzato dalla banca che hai specificato nel campo **Banca ESR**, selezionare **Basato su banca ESR**.</span><span class="sxs-lookup"><span data-stu-id="65f46-126">To use the ESR system that is used by the bank that you have specified in **ESR Bank** field, select **Based on ESR Bank**.</span></span>|  

3.  <span data-ttu-id="65f46-127">Scegliere il pulsante **Stampa** per stampare il report oppure scegliere il pulsante **Anteprima** per visualizzarlo sullo schermo.</span><span class="sxs-lookup"><span data-stu-id="65f46-127">Choose the **Print** button to print the report or choose the **Preview** button to view it on the screen.</span></span>  

<span data-ttu-id="65f46-128">È inoltre possibile ristampare il report ESR della fattura di vendita o il report del tagliando ESR di vendita.</span><span class="sxs-lookup"><span data-stu-id="65f46-128">You can also reprint the sales invoice ESR report or sales ESR coupon report.</span></span>  

## <a name="see-also"></a><span data-ttu-id="65f46-129">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="65f46-129">See Also</span></span>  
 <span data-ttu-id="65f46-130">[Pagamenti elettronici svizzeri tramite ESR](swiss-electronic-payments-using-esr.md) </span><span class="sxs-lookup"><span data-stu-id="65f46-130">[Swiss Electronic Payments Using ESR](swiss-electronic-payments-using-esr.md) </span></span>  
 [<span data-ttu-id="65f46-131">Importare i pagamenti ESR</span><span class="sxs-lookup"><span data-stu-id="65f46-131">Import ESR Payments</span></span>](how-to-import-esr-payments.md)

