---
title: Impostare condizioni interessi finanziari
description: Informazioni su come impostare Business Central in modo da poter informare i clienti degli addebiti aggiuntivi inviando note addebito interessi.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: payment due, debt, overdue, fee, charge
ms.date: 12/03/2020
ms.author: edupont
ms.openlocfilehash: dad02adfb6cc0a0ebb6d950b67f2e092b3313c59
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 02/15/2021
ms.locfileid: "5377105"
---
# <a name="set-up-finance-charge-terms"></a><span data-ttu-id="6d133-103">Impostare condizioni interessi finanziari</span><span class="sxs-lookup"><span data-stu-id="6d133-103">Set Up Finance Charge Terms</span></span>

<span data-ttu-id="6d133-104">Quando un cliente non effettua il pagamento entro la data di scadenza, è possibile fare in modo che gli addebiti per interessi vengano calcolati automaticamente e aggiunti agli importi insoluti nel conto del cliente.</span><span class="sxs-lookup"><span data-stu-id="6d133-104">When a customer does not pay by the due date, you can have finance charges calculated automatically and add them to the overdue amounts on the customer's account.</span></span> <span data-ttu-id="6d133-105">È possibile informare i clienti degli interessi aggiunti mediante l'invio di note di addebito interessi.</span><span class="sxs-lookup"><span data-stu-id="6d133-105">You can inform customers of the added charges by sending finance charge memos.</span></span> <span data-ttu-id="6d133-106">Tuttavia, impostare dapprima un codice che rappresenta ogni calcolo di addebito interessi.</span><span class="sxs-lookup"><span data-stu-id="6d133-106">But first, you must set up a code that represents each finance charge calculation.</span></span> <span data-ttu-id="6d133-107">Immettere quindi questo codice nel campo Codice condizioni di addebito interessi nelle schede cliente.</span><span class="sxs-lookup"><span data-stu-id="6d133-107">Then you can enter this code in the Fin. Charge Terms Code field on customer cards.</span></span>  

## <a name="finance-charge-terms"></a><span data-ttu-id="6d133-108">Condizioni interessi finanziari</span><span class="sxs-lookup"><span data-stu-id="6d133-108">Finance charge terms</span></span>

<span data-ttu-id="6d133-109">È necessario impostare le condizioni interessi finanziari per ogni calcolo di addebito interessi e quindi assegnare le condizioni nel campo **Codice condizioni di addebito interessi** nella pagina **Cliente**.</span><span class="sxs-lookup"><span data-stu-id="6d133-109">You must set up finance charge terms for each finance charge calculation, and then assign the terms to the customer in the **Fin. Charge Terms Code** field on the **Customer** page.</span></span>

<span data-ttu-id="6d133-110">È possibile calcolare gli addebiti interessi utilizzando il metodo del saldo giornaliero medio oppure il metodo del saldo dovuto.</span><span class="sxs-lookup"><span data-stu-id="6d133-110">Finance charges can be calculated using either the average daily balance or the balance due methods.</span></span>

* <span data-ttu-id="6d133-111">Saldo giornaliero medio</span><span class="sxs-lookup"><span data-stu-id="6d133-111">Average daily balance</span></span>  
  
  <span data-ttu-id="6d133-112">Viene considerato il numero di giorni che il pagamento è dovuto:</span><span class="sxs-lookup"><span data-stu-id="6d133-112">The number of days the payment is overdue is taken into account:</span></span>  
  <span data-ttu-id="6d133-113">*Metodo Saldo giornaliero medio* - *Addebito interessi* = *Importo insoluto* x *(Giorni in arretrato / Periodo di interesse)* x *(Tasso di interesse/100)*</span><span class="sxs-lookup"><span data-stu-id="6d133-113">*Average Daily Balance method* - *Finance Charge* = *Overdue Amount* x *(Days Overdue / Interest Period)* x *(Interest Rate/100)*</span></span>

* <span data-ttu-id="6d133-114">Saldo scaduto</span><span class="sxs-lookup"><span data-stu-id="6d133-114">Balance due</span></span>  
  
  <span data-ttu-id="6d133-115">L'addebito interessi è una percentuale dell'importo insoluto:</span><span class="sxs-lookup"><span data-stu-id="6d133-115">The finance charge is a percentage of the overdue amount:</span></span>  
  <span data-ttu-id="6d133-116">*Metodo del saldo dovuto* - *Addebito interessi* = *Importo insoluto* x *(Tasso di interesse / 100)*</span><span class="sxs-lookup"><span data-stu-id="6d133-116">*Balance Due method* - *Finance Charge* = *Overdue Amount* x *(Interest Rate / 100)*</span></span>

<span data-ttu-id="6d133-117">Inoltre ogni condizione nella tabella Condiz.Interessi Finanziari è collegata a una sottotabella, detta tabella Testi addebiti interessi.</span><span class="sxs-lookup"><span data-stu-id="6d133-117">Additionally, each term in the Finance Charge Terms table is linked to a subtable, the Finance Charge Text table.</span></span> <span data-ttu-id="6d133-118">Per ciascun gruppo di condizioni interessi finanziari, è possibile creare un testo iniziale e/o uno finale da includere nella nota di addebito degli interessi.</span><span class="sxs-lookup"><span data-stu-id="6d133-118">For each set of finance charge terms, you can define a beginning and/or an ending text to include on the finance charge memo.</span></span>

### <a name="to-set-up-finance-charge-terms"></a><span data-ttu-id="6d133-119">Per impostare le condizioni di addebito degli interessi</span><span class="sxs-lookup"><span data-stu-id="6d133-119">To set up finance charge terms</span></span>

1. <span data-ttu-id="6d133-120">Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Condiz. interessi finanziari** e quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="6d133-120">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Finance Charge Terms**, and then choose the related link.</span></span>  
2. <span data-ttu-id="6d133-121">Compilare i campi, se necessario.</span><span class="sxs-lookup"><span data-stu-id="6d133-121">Fill in the fields as necessary.</span></span>
3. <span data-ttu-id="6d133-122">Per utilizzare più di una combinazione di condizioni interessi finanziari, impostare un codice per ciascuno di essi.</span><span class="sxs-lookup"><span data-stu-id="6d133-122">To use more than one combination of finance charge terms, set up a code for each one.</span></span>

    <span data-ttu-id="6d133-123">Per ogni condizione di interessi finanziari, è possibile specificare singole condizioni, tra cui oneri addizionali sia in VL sia in valuta estera.</span><span class="sxs-lookup"><span data-stu-id="6d133-123">For each finance charge term, you can specify individual conditions that can include additional fees in both LCY and in foreign currency.</span></span> <span data-ttu-id="6d133-124">È possibile definire oneri addizionali in valuta estera per ogni condizione nella pagina **Condiz. interessi finanziari**.</span><span class="sxs-lookup"><span data-stu-id="6d133-124">You can define additional fees in foreign currencies for each term on the **Finance Charge Terms** page.</span></span>
4. <span data-ttu-id="6d133-125">Scegliere l'azione **Valute**.</span><span class="sxs-lookup"><span data-stu-id="6d133-125">Choose the **Currencies** action.</span></span>
5. <span data-ttu-id="6d133-126">Nella pagina **Valute per addebito interessi**, specificare per ogni termine un codice valuta e un onere addizionale.</span><span class="sxs-lookup"><span data-stu-id="6d133-126">On the **Currencies for Fin. Chrg. Terms** page, define for each term a currency code and an additional fee.</span></span>

    > [!NOTE]  
    > <span data-ttu-id="6d133-127">Creando addebiti di interessi in una valuta estera, le condizioni per la valuta estera impostate qui verranno utilizzate per creare note di addebito interessi.</span><span class="sxs-lookup"><span data-stu-id="6d133-127">When you create finance charges in a foreign currency, the foreign currency conditions that you set up here will be used to create finance charge memos.</span></span> <span data-ttu-id="6d133-128">Se non sono state impostate condizioni interessi finanziari in valuta estera, verranno utilizzate le condizioni interessi finanziari in valuta locale specificate nella pagina **Condiz. interessi finanziari** e quindi convertite nella relativa valuta.</span><span class="sxs-lookup"><span data-stu-id="6d133-128">If there are no foreign currency finance charge conditions set up, the LCY finance charge conditions specified on the **Finance Charge Terms** page will be used and then converted to the relevant currency.</span></span>

    <span data-ttu-id="6d133-129">Per ciascuna condizione di interessi finanziari è possibile specificare il testo che sarà stampato prima (**Testo Iniziale**) o dopo (**Testo Finale**) nei movimenti nella nota di addebito di interessi.</span><span class="sxs-lookup"><span data-stu-id="6d133-129">For each finance charge term, you can specify text that will be printed before (**Beginning Text**) or after (**Ending Text**) on the entries on the finance charge memo.</span></span>  
6. <span data-ttu-id="6d133-130">Scegliere rispettivamente le azioni **Testo iniziale** o **Testo finale** e compilare la pagina **Testi addebiti interessi**.</span><span class="sxs-lookup"><span data-stu-id="6d133-130">Choose the **Beginning Text** or **Ending Text** actions respectively, and fill on the **Finance Charge Text** page.</span></span>
7. <span data-ttu-id="6d133-131">Per inserire automaticamente i relativi valori nel testo di addebito di interessi risultante, fornire seguenti segnaposti nel campo **Testo**.</span><span class="sxs-lookup"><span data-stu-id="6d133-131">To automatically insert related values in the resulting finance charge text, enter the following placeholders in the **Text** field.</span></span>

|<span data-ttu-id="6d133-132">Segnaposto</span><span class="sxs-lookup"><span data-stu-id="6d133-132">Placeholder</span></span>|<span data-ttu-id="6d133-133">Valore</span><span class="sxs-lookup"><span data-stu-id="6d133-133">Value</span></span>|  
|-----------------|-----------|  
|<span data-ttu-id="6d133-134">%1</span><span class="sxs-lookup"><span data-stu-id="6d133-134">%1</span></span>|<span data-ttu-id="6d133-135">Contenuto del campo **Data documento** della testata della nota di addebito interessi</span><span class="sxs-lookup"><span data-stu-id="6d133-135">Content of the **Document Date** field on the finance charge memo header</span></span>|  
|<span data-ttu-id="6d133-136">%2</span><span class="sxs-lookup"><span data-stu-id="6d133-136">%2</span></span>|<span data-ttu-id="6d133-137">Contenuto del campo **Data scadenza** della testata della nota di addebito interessi</span><span class="sxs-lookup"><span data-stu-id="6d133-137">Content of the **Due Date** field on the finance charge memo header</span></span>|  
|<span data-ttu-id="6d133-138">%3</span><span class="sxs-lookup"><span data-stu-id="6d133-138">%3</span></span>|<span data-ttu-id="6d133-139">Contenuto del campo **Tasso di interesse** nelle condizioni di addebito degli interessi finanziari correlate</span><span class="sxs-lookup"><span data-stu-id="6d133-139">Content of the **Interest Rate** field on the related finance charge terms</span></span>|  
|<span data-ttu-id="6d133-140">%4</span><span class="sxs-lookup"><span data-stu-id="6d133-140">%4</span></span>|<span data-ttu-id="6d133-141">Contenuto del campo **Importo residuo** della testata della nota di addebito interessi</span><span class="sxs-lookup"><span data-stu-id="6d133-141">Content of the **Remaining Amount** field on the finance charge memo header</span></span>|  
|<span data-ttu-id="6d133-142">%5</span><span class="sxs-lookup"><span data-stu-id="6d133-142">%5</span></span>|<span data-ttu-id="6d133-143">Contenuto del campo **Importo interessi** della testata della nota di addebito interessi</span><span class="sxs-lookup"><span data-stu-id="6d133-143">Content of the **Interest Amount** field on the finance charge memo header</span></span>|  
|<span data-ttu-id="6d133-144">%6</span><span class="sxs-lookup"><span data-stu-id="6d133-144">%6</span></span>|<span data-ttu-id="6d133-145">Contenuto del campo **Onere addizionale** della testata della nota di addebito interessi</span><span class="sxs-lookup"><span data-stu-id="6d133-145">Content of the **Additional Fee** field on the finance charge memo header</span></span>|  
|<span data-ttu-id="6d133-146">%7</span><span class="sxs-lookup"><span data-stu-id="6d133-146">%7</span></span>|<span data-ttu-id="6d133-147">Importo totale del sollecito</span><span class="sxs-lookup"><span data-stu-id="6d133-147">The total amount of the reminder</span></span>|  
|<span data-ttu-id="6d133-148">%8</span><span class="sxs-lookup"><span data-stu-id="6d133-148">%8</span></span>|<span data-ttu-id="6d133-149">Contenuto del campo **Codice valuta** della testata della nota di addebito interessi</span><span class="sxs-lookup"><span data-stu-id="6d133-149">Content of the **Currency Code** field on the finance charge memo header</span></span>|  
|<span data-ttu-id="6d133-150">%9</span><span class="sxs-lookup"><span data-stu-id="6d133-150">%9</span></span>|<span data-ttu-id="6d133-151">Contenuto del campo **Data reg.** della testata della nota di addebito interessi</span><span class="sxs-lookup"><span data-stu-id="6d133-151">Content of the **Posting Date** field on the finance charge memo header</span></span>|  

## <a name="see-also"></a><span data-ttu-id="6d133-152">Vedere anche</span><span class="sxs-lookup"><span data-stu-id="6d133-152">See also</span></span>

[<span data-ttu-id="6d133-153">Riscuotere i saldi inevasi</span><span class="sxs-lookup"><span data-stu-id="6d133-153">Collect Outstanding Balances</span></span>](receivables-collect-outstanding-balances.md)  
[<span data-ttu-id="6d133-154">Impostare i termini e i livelli di sollecito</span><span class="sxs-lookup"><span data-stu-id="6d133-154">Set Up Reminder Terms and Levels</span></span>](finance-setup-reminders.md)  
[<span data-ttu-id="6d133-155">Impostazione di dati finanziari</span><span class="sxs-lookup"><span data-stu-id="6d133-155">Setting Up Finance</span></span>](finance-setup-finance.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]