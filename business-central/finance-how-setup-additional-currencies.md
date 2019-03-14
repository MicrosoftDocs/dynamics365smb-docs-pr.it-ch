---
title: Impostazione di valute addizionali | Microsoft Docs
description: "La contabilità generale è impostata per utilizzare la valuta locale (VL) e un'altra valuta viene impostata come valuta addizionale, con un tasso di cambio corrente assegnato."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: multiple currencies
ms.date: 01/07/2019
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: a98027c3ef3171491f84197897f93cbed4e288c2
ms.openlocfilehash: 294ed8019b12287e4b4ad59d46e842e4022a637f
ms.contentlocale: it-ch
ms.lasthandoff: 01/07/2019

---
# <a name="set-up-an-additional-reporting-currency"></a><span data-ttu-id="af231-103">Impostare una valuta contabile addizionale</span><span class="sxs-lookup"><span data-stu-id="af231-103">Set Up an Additional Reporting Currency</span></span>
<span data-ttu-id="af231-104">Con l'espandersi delle attività delle società in un numero sempre maggiore di paesi, diventa importante poter esaminare e riportare dati finanziari in più di una valuta.</span><span class="sxs-lookup"><span data-stu-id="af231-104">As companies operate in increasingly more countries/regions, it becomes more important that they are able to review and report financial data in more than one currency.</span></span>

<span data-ttu-id="af231-105">La contabilità generale è impostata per utilizzare la valuta locale (VL) ma è anche possibile impostarla per l'uso di un'altra valuta con un tasso di cambio corrente assegnato.</span><span class="sxs-lookup"><span data-stu-id="af231-105">Your general ledger is set up to use your local currency (LCY), but you can set it up to also use another currency with a current exchange rate assigned.</span></span> <span data-ttu-id="af231-106">Se si imposta una seconda valuta come valuta contabile addizionale, in [!INCLUDE[d365fin](includes/d365fin_md.md)] gli importi in ogni movimento C/G e in tutti gli altri movimenti, ad esempio i movimenti IVA, vengono registrati automaticamente sia nella valuta locale che nella valuta addizionale.</span><span class="sxs-lookup"><span data-stu-id="af231-106">By designating a second currency as a so-called additional reporting currency, [!INCLUDE[d365fin](includes/d365fin_md.md)] will automatically record amounts in both LCY and this additional reporting currency on each G/L entry and other entries, such as VAT entries.</span></span>

> [!Warning]
> <span data-ttu-id="af231-107">La funzionalità Valuta contabile addizionale non deve essere utilizzata come base per la conversione del rendiconto finanziario.</span><span class="sxs-lookup"><span data-stu-id="af231-107">The Additional Reporting Currency functionality should not be used as a basis for financial statement translation.</span></span> <span data-ttu-id="af231-108">Questo strumento non consente di eseguire la conversione dei rendiconti finanziari delle filiali estere come parte del consolidamento di una società.</span><span class="sxs-lookup"><span data-stu-id="af231-108">It is not a tool that can perform translation of foreign subsidiary financial statements as part of a company consolidation.</span></span> <span data-ttu-id="af231-109">La valuta contabile addizionale può essere utilizzata soltanto per creare report in un'altra valuta, come se tale valuta fosse quella locale della società.</span><span class="sxs-lookup"><span data-stu-id="af231-109">The additional reporting currency can only be used to prepare reports in another currency, as if that currency was the company’s local currency.</span></span>

## <a name="displaying-reports-and-amounts-in-the-additional-reporting-currency"></a><span data-ttu-id="af231-110">Visualizzazione di report e importi nella valuta addizionale</span><span class="sxs-lookup"><span data-stu-id="af231-110">Displaying Reports and Amounts in the Additional Reporting Currency</span></span>
<span data-ttu-id="af231-111">L'utilizzo di una valuta addizionale può essere utile per il processo di creazione di report di una società nei seguenti casi:</span><span class="sxs-lookup"><span data-stu-id="af231-111">Using an additional reporting currency can assist the reporting process for a company in the following cases:</span></span>

- <span data-ttu-id="af231-112">Società di paesi non UE che effettuano numerose transazioni con società di paesi UE.</span><span class="sxs-lookup"><span data-stu-id="af231-112">Companies in non-EU countries/regions that have a high proportion of transactions with EU country/region companies.</span></span> <span data-ttu-id="af231-113">In questo caso, la società non UE potrebbe desiderare di creare report in euro per semplificare l'utilizzo dei report finanziari da parte dei partner commerciali UE.</span><span class="sxs-lookup"><span data-stu-id="af231-113">In this case, the non-EU company may also wish to report in euro to make its financial reports more usable for EU trade partners.</span></span>
- <span data-ttu-id="af231-114">Società che desiderano visualizzare i report in una valuta maggiormente utilizzata a livello internazionale rispetto alla propria valuta locale.</span><span class="sxs-lookup"><span data-stu-id="af231-114">Companies that also wish to display reports in a more internationally traded currency than their own local currency.</span></span>

<span data-ttu-id="af231-115">Vari report finanziari sono basati sui movimenti C/G.</span><span class="sxs-lookup"><span data-stu-id="af231-115">Several financial reports are based on G/L entries.</span></span> <span data-ttu-id="af231-116">Per visualizzare i dati del report nella valuta contabile addizionale, selezionare semplicemente il campo **Mostra importi in valuta contabile addizionale** nella Scheda dettaglio **Opzioni** per il relativo report CG.</span><span class="sxs-lookup"><span data-stu-id="af231-116">To display report data in the additional reporting currency, you simply place a check mark in the **Show Amounts in Add. Reporting Currency** field on the **Options** FastTab for the relevant G/L report.</span></span>

## <a name="adjusting-exchange-rates"></a><span data-ttu-id="af231-117">Rettifica di tassi di cambio</span><span class="sxs-lookup"><span data-stu-id="af231-117">Adjusting Exchange Rates</span></span>
<span data-ttu-id="af231-118">Poiché i tassi di cambio oscillano costantemente, gli equivalenti in valuta addizionale nel sistema devono essere rettificati periodicamente.</span><span class="sxs-lookup"><span data-stu-id="af231-118">Because exchange rates fluctuate constantly, additional currency equivalents in your system must be adjusted periodically.</span></span> <span data-ttu-id="af231-119">Se queste rettifiche non vengono apportate, gli importi che sono stati convertiti da valute estere (o addizionali) e registrati nella contabilità generale in valuta locale possono essere fuorvianti.</span><span class="sxs-lookup"><span data-stu-id="af231-119">If these adjustments are not done, amounts that have been converted from foreign (or additional) currencies and posted to the general ledger in LCY may be misleading.</span></span> <span data-ttu-id="af231-120">Inoltre, i movimenti quotidiani registrati prima dell'immissione di un tasso di cambio quotidiano nel programma devono essere aggiornati dopo l'immissione delle informazioni su tale tasso di cambio.</span><span class="sxs-lookup"><span data-stu-id="af231-120">In addition, daily entries posted before a daily exchange rate is entered into the program must be updated after the daily exchange rate information is entered.</span></span> <span data-ttu-id="af231-121">Il processo batch **Rettifica tassi di cambio** viene utilizzato per rettificare i tassi di cambio dei movimenti cliente, fornitore e conti C/C bancari registrati.</span><span class="sxs-lookup"><span data-stu-id="af231-121">The **Adjust Exchange Rates** batch job is used to adjust the exchange rates of posted customer, vendor and bank account entries.</span></span> <span data-ttu-id="af231-122">Consente inoltre di aggiornare gli importi nella valuta contabile addizionale nei movimenti C/G.</span><span class="sxs-lookup"><span data-stu-id="af231-122">It can also update additional reporting currency amounts on G/L entries.</span></span> <span data-ttu-id="af231-123">Per ulteriori informazioni, vedere [Aggiornare i tassi di cambio valuta](finance-how-update-currencies.md).</span><span class="sxs-lookup"><span data-stu-id="af231-123">For more information, see [Update Currency Exchange Rates](finance-how-update-currencies.md).</span></span>

## <a name="setting-up-an-additional-reporting-currency"></a><span data-ttu-id="af231-124">Impostare una valuta contabile addizionale</span><span class="sxs-lookup"><span data-stu-id="af231-124">Setting Up an Additional Reporting Currency</span></span>
<span data-ttu-id="af231-125">Seguire questa procedura per impostare una valuta contabile addizionale:</span><span class="sxs-lookup"><span data-stu-id="af231-125">To set up an additional reporting currency, you must follow these steps:</span></span>

-   <span data-ttu-id="af231-126">Specificare i conti C/G per la registrazione delle rettifiche al tasso di cambio.</span><span class="sxs-lookup"><span data-stu-id="af231-126">Specify general ledger accounts for posting exchange rate adjustments.</span></span>  
-   <span data-ttu-id="af231-127">Specificare il metodo della rettifica tasso di cambio per tutti i conti C/G.</span><span class="sxs-lookup"><span data-stu-id="af231-127">Specify the exchange rate adjustment method for all general ledger accounts.</span></span>  
-   <span data-ttu-id="af231-128">Specificare il metodo di rettifica del tasso di cambio per i movimenti IVA.</span><span class="sxs-lookup"><span data-stu-id="af231-128">Specify the exchange rate adjustment method for VAT entries.</span></span>  
-   <span data-ttu-id="af231-129">Attivare la valuta contabile addizionale.</span><span class="sxs-lookup"><span data-stu-id="af231-129">Activate the additional reporting currency.</span></span>  

### <a name="to-specify-general-ledger-accounts-for-posting-exchange-rate-adjustments"></a><span data-ttu-id="af231-130">Per specificare i conti C/G per la registrazione delle rettifiche tasso di cambio.</span><span class="sxs-lookup"><span data-stu-id="af231-130">To specify general ledger accounts for posting exchange rate adjustments</span></span>  

1. <span data-ttu-id="af231-131">Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Valute** e quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="af231-131">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Currencies**, and then choose the related link.</span></span>  
2. <span data-ttu-id="af231-132">Nella pagina **Valute** riempire i seguenti campi per la valuta contabile addizionale.</span><span class="sxs-lookup"><span data-stu-id="af231-132">On the **Currencies** page, fill in the following fields for the additional reporting currency.</span></span>  

|<span data-ttu-id="af231-133">Campo</span><span class="sxs-lookup"><span data-stu-id="af231-133">Field</span></span>|<span data-ttu-id="af231-134">Description</span><span class="sxs-lookup"><span data-stu-id="af231-134">Description</span></span>|  
|---------------------------------|---------------------------------------|  
|<span data-ttu-id="af231-135">**Conto utili CG realizzati**</span><span class="sxs-lookup"><span data-stu-id="af231-135">**Realized GL Gains Account**</span></span>|<span data-ttu-id="af231-136">Il conto CoGe nel quale verranno registrate i profitti del tasso di cambio per le rettifiche valutarie tra la valuta locale e la valuta contabile addizionale.</span><span class="sxs-lookup"><span data-stu-id="af231-136">The general ledger account to which exchange rate gains for currency adjustments between LCY and the additional reporting currency will be posted.</span></span>|  
|<span data-ttu-id="af231-137">**Conto perdite CG realizzate**</span><span class="sxs-lookup"><span data-stu-id="af231-137">**Realized GL Losses Account**</span></span>|<span data-ttu-id="af231-138">Il conto CoGe nel quale verranno registrate le perdite del tasso di cambio per le rettifiche valutarie tra la valuta locale e la valuta contabile addizionale.</span><span class="sxs-lookup"><span data-stu-id="af231-138">The general ledger account to which exchange rate losses for currency adjustments between LCY and the additional reporting currency will be posted.</span></span>|  
|<span data-ttu-id="af231-139">**Conto guadagni residui**</span><span class="sxs-lookup"><span data-stu-id="af231-139">**Residual Gains Account**</span></span>|<span data-ttu-id="af231-140">Il conto CoGe in cui registrare gli importi residui che rappresentano dei profitti nel caso in cui si effettui la registrazione nell'area di applicazione contabilità generale sia nella valuta locale che nella valuta contabile addizionale.</span><span class="sxs-lookup"><span data-stu-id="af231-140">The general ledger account to which residual amounts that are gains are posted if you post in the general ledger application area in both LCY and an additional reporting currency.</span></span>|  
|<span data-ttu-id="af231-141">**Conto perdite residue**</span><span class="sxs-lookup"><span data-stu-id="af231-141">**Residual Losses Account**</span></span>|<span data-ttu-id="af231-142">Il conto CoGe in cui registrare gli importi residui che rappresentano delle perdite nel caso in cui si effettui la registrazione nell'area di applicazione contabilità generale sia nella valuta locale che nella valuta contabile addizionale.</span><span class="sxs-lookup"><span data-stu-id="af231-142">The general ledger account to which residual amounts that are losses are posted if you post in the general ledger application area in both LCY and an additional reporting currency.</span></span>|

> [!NOTE]  
>  <span data-ttu-id="af231-143">Gli importi residui possono verificarsi quando gli importi in dare e in avere convertiti dalla valuta locale in una valuta addizionale vengono arrotondati da [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="af231-143">Residual amounts can occur when [!INCLUDE[d365fin](includes/d365fin_md.md)] rounds debit and credit amounts that have been converted from LCY to an additional reporting currency.</span></span>  

<span data-ttu-id="af231-144">Per ogni conto C/G, è necessario specificare in che modo gli importi C/G per il conto verranno rettificati in caso di fluttuazioni del tasso di cambio tra la valuta locale e quella contabile addizionale.</span><span class="sxs-lookup"><span data-stu-id="af231-144">For each general ledger account, you must specify how general ledger amounts for that account will be adjusted for exchange rate fluctuations between LCY and the additional reporting currency.</span></span>  

### <a name="to-specify-the-exchange-rate-adjustment-method-for-all-general-ledger-accounts"></a><span data-ttu-id="af231-145">Per specificare il metodo della rettifica tasso di cambio per tutti i conti C/G</span><span class="sxs-lookup"><span data-stu-id="af231-145">To specify the exchange rate adjustment method for all general ledger accounts</span></span>  
1. <span data-ttu-id="af231-146">Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Piano dei conti** e quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="af231-146">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Accounts**, and then choose the related link.</span></span>  
2. <span data-ttu-id="af231-147">Nella pagina **Piano dei conti**, selezionare il conto pertinente quindi scegliere l'azione **Modifica**.</span><span class="sxs-lookup"><span data-stu-id="af231-147">On the **Chart of Accounts** page, select the relevant account, and then choose the **Edit** action.</span></span>  
3. <span data-ttu-id="af231-148">Nella pagina **Scheda conto GL** selezionare il metodo pertinente nel campo **Rettifica tasso di cambio**.</span><span class="sxs-lookup"><span data-stu-id="af231-148">On the **GL Account Card** page, select the relevant method in the **Exchange Rate Adjustment** field.</span></span>  

    <span data-ttu-id="af231-149">Se si effettua la registrazione in una valuta addizionale, specificare nel campo **Rettifica tasso di cambio** in che modo verrà rettificato il conto C/G per le fluttuazioni del tasso di cambio tra la valuta locale e quella contabile addizionale.</span><span class="sxs-lookup"><span data-stu-id="af231-149">If you post in an additional reporting currency, specify in the **Exchange Rate Adjustment** field how this general ledger account will be adjusted for exchange-rate fluctuations between LCY and the additional reporting currency.</span></span> <span data-ttu-id="af231-150">Nella tabella seguente vengono indicate le opzioni che è possibile scegliere.</span><span class="sxs-lookup"><span data-stu-id="af231-150">The following table shows the options to choose from.</span></span>  

    |<span data-ttu-id="af231-151">Campo</span><span class="sxs-lookup"><span data-stu-id="af231-151">Field</span></span>|<span data-ttu-id="af231-152">Descrizione</span><span class="sxs-lookup"><span data-stu-id="af231-152">Decription</span></span>|  
    |----------------------------------|---------------------------------------|  
    |<span data-ttu-id="af231-153">**No Rettifica**</span><span class="sxs-lookup"><span data-stu-id="af231-153">**No Adjustment**</span></span>|<span data-ttu-id="af231-154">Non viene effettuata alcuna rettifica del tasso di cambio per il movimento C/G.</span><span class="sxs-lookup"><span data-stu-id="af231-154">No exchange rate adjustment is made to the general ledger account.</span></span> <span data-ttu-id="af231-155">Questa è l'opzione predefinita.</span><span class="sxs-lookup"><span data-stu-id="af231-155">This is the default option.</span></span><br /><br /> <span data-ttu-id="af231-156">**NOTA:** TQuesta opzione deve essere selezionata se il tasso di cambio tra la valuta locale e quella contabile addizionale è sempre fisso.</span><span class="sxs-lookup"><span data-stu-id="af231-156">**NOTE:** This option should be selected if the exchange rate between the LCY and additional reporting currency is always fixed.</span></span>|  
    |<span data-ttu-id="af231-157">**Rettifica Importo**</span><span class="sxs-lookup"><span data-stu-id="af231-157">**Adjust Amount**</span></span>|<span data-ttu-id="af231-158">L'importo VL verrà rettificato per tutti gli utili e le perdite del tasso di cambio.</span><span class="sxs-lookup"><span data-stu-id="af231-158">The LCY amount is adjusted for any exchange rate gains or losses.</span></span> <span data-ttu-id="af231-159">Tali utili o perdite verranno registrati nel conto C/G nel campo **Importo** e nel campo **Conto utili C/G realizzati** o **Conto perdite C/G realizzate** della pagina **Valute** dei conti specificati per gli utili o le perdite.</span><span class="sxs-lookup"><span data-stu-id="af231-159">Exchange rate gains or losses are posted to the general ledger account in the **Amount** field and to the accounts you specified for gains or losses in the **Realized G/L Gains Account** and **Realized G/L Losses Account** fields on the **Currencies** page.</span></span>|  
    |<span data-ttu-id="af231-160">**Rettifica Importo in Valuta-Addiz.**</span><span class="sxs-lookup"><span data-stu-id="af231-160">**Adjust Additional-Currency Amount**</span></span>|<span data-ttu-id="af231-161">La valuta contabile addizionale verrà rettificata per tutti gli utili e le perdite del tasso di cambio.</span><span class="sxs-lookup"><span data-stu-id="af231-161">The additional reporting currency is adjusted for any exchange rate gains or losses.</span></span> <span data-ttu-id="af231-162">Tali utili o perdite verranno registrati nel conto C/G nel campo **Importo in valuta addiz.** e nel campo **Conto utili C/G realizzati** o **Conto perdite C/G realizzate** della pagina **Valute** dei conti specificati per gli utili o le perdite.</span><span class="sxs-lookup"><span data-stu-id="af231-162">Exchange rate gains or losses are posted to the general ledger account in the **Additional-Currency Amount** field and to the accounts you specified for gains or losses in the **Realized G/L Gains Account** and **Realized G/L Losses Account** fields on the **Currencies** page.</span></span>|  

    <span data-ttu-id="af231-163">Gli utili e le perdite di conversione vengono registrati quando si esegue il processo batch **Rettifica tassi di cambio**.</span><span class="sxs-lookup"><span data-stu-id="af231-163">Exchange rate gains and losses are posted when you run the **Adjust Exchange Rates** batch job.</span></span> <span data-ttu-id="af231-164">Durante il processo batch, viene individuato il tasso di cambio di rettifica nella pagina **Tassi di cambio valuta**, quindi vengono messi a confronto gli importi nei campi **Importo** e **Importo in valuta addiz.** nel movimento C/G per determinare se vi è un utile o una perdita di conversione.</span><span class="sxs-lookup"><span data-stu-id="af231-164">In that batch job, the adjustment exchange rate is identified on the **Currency Exchange Rates** page, and then the amounts in the **Amount** and **Additional-Currency Amount** fields on the general ledger entry are compared to determine whether there is an exchange rate gain or loss.</span></span> <span data-ttu-id="af231-165">Nel processo batch viene utilizzata l'opzione selezionata nel campo **Rettifica tasso di cambio** per determinare come calcolare e registrare gli utili o le perdite di conversione nei conti C/G.</span><span class="sxs-lookup"><span data-stu-id="af231-165">The batch job uses the option that you select in the **Exchange Rate Adjustment** field to determine how to calculate and post exchange rate gains or losses for general ledger accounts.</span></span>  

4.  <span data-ttu-id="af231-166">Chiudere la pagina **Scheda conto C/G**.</span><span class="sxs-lookup"><span data-stu-id="af231-166">Close the **G/L Account Card** page.</span></span>  

### <a name="to-specify-exchange-rate-adjustment-method-for-vat-entries"></a><span data-ttu-id="af231-167">Per specificare il metodo di rettifica del tasso di cambio per i movimenti IVA</span><span class="sxs-lookup"><span data-stu-id="af231-167">To specify exchange rate adjustment method for VAT entries</span></span>  
1. <span data-ttu-id="af231-168">Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Setup contabilità generale** e quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="af231-168">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Ledger Setup**, and then choose the related link.</span></span>  
2. <span data-ttu-id="af231-169">Nella pagina **Setup contabilità generale** selezionare il metodo pertinente nel campo **Rettif. tasso di cambio IVA**.</span><span class="sxs-lookup"><span data-stu-id="af231-169">On the **General Ledger Setup** page, select the relevant method in the **VAT Exchange Rate Adjustment** field.</span></span>  
3. <span data-ttu-id="af231-170">Se si effettua la registrazione in una valuta addizionale, è possibile specificare nel campo **Rettif. tasso di cambio IVA** in che modo verranno rettificati i conti impostati per la registrazione IVA nella pagina **Setup registrazioni IVA** per le fluttuazioni del tasso di cambio tra la valuta locale e quella addizionale.</span><span class="sxs-lookup"><span data-stu-id="af231-170">If you post in an additional reporting currency, you can specify in the **VAT Exchange Rate Adjustment** field how the accounts set up for VAT posting on the **VAT Posting Setup** page will be adjusted for exchange-rate fluctuations between LCY and the additional reporting currency.</span></span>  

    <span data-ttu-id="af231-171">Quando si esegue il processo batch **Rettifica tassi di cambio**, viene individuato il tasso di cambio di rettifica nella pagina **Tassi di cambio valuta**, quindi vengono messi a confronto gli importi nei campi **Importo** e **Importo in valuta addiz.** nel movimento IVA per determinare se vi è un utile o una perdita di conversione.</span><span class="sxs-lookup"><span data-stu-id="af231-171">When you run the **Adjust Exchange Rates** batch job, the adjustment exchange rate is identified on the **Currency Exchange Rate** page and then the amounts in the **Amount** and **Additional-Currency Amount** fields on the VAT entry are compared to determine if there is an exchange rate gain or loss.</span></span> <span data-ttu-id="af231-172">L'opzione selezionata in questo campo viene utilizzata dal processo batch per determinare come registrare gli utili e le perdite di conversione per i conti IVA.</span><span class="sxs-lookup"><span data-stu-id="af231-172">The batch job uses the option that you select in this field to determine how to post exchange rate gains or losses for VAT accounts.</span></span>  

    <span data-ttu-id="af231-173">Sono disponibili le stesse tre opzioni disponibili per i movimenti C/G, ma in questo caso i movimenti rettificati saranno i movimenti IVA.</span><span class="sxs-lookup"><span data-stu-id="af231-173">You have the same options as with general ledger entries but in this case the entries adjusted will be the VAT entries.</span></span> <span data-ttu-id="af231-174">Nella tabella seguente vengono indicate le opzioni che è possibile scegliere.</span><span class="sxs-lookup"><span data-stu-id="af231-174">The following table shows the options to choose from.</span></span>

    |<span data-ttu-id="af231-175">Campo</span><span class="sxs-lookup"><span data-stu-id="af231-175">Field</span></span>|<span data-ttu-id="af231-176">Description</span><span class="sxs-lookup"><span data-stu-id="af231-176">Description</span></span>|  
    |----------------------------------|---------------------------------------|  
    |<span data-ttu-id="af231-177">**No Rettifica**</span><span class="sxs-lookup"><span data-stu-id="af231-177">**No Adjustment**</span></span>|<span data-ttu-id="af231-178">Non viene effettuata alcuna rettifica del tasso di cambio per il movimento C/G.</span><span class="sxs-lookup"><span data-stu-id="af231-178">No exchange rate adjustment is made to the general ledger account.</span></span> <span data-ttu-id="af231-179">Questa è l'opzione predefinita.</span><span class="sxs-lookup"><span data-stu-id="af231-179">This is the default option.</span></span>|  
    |<span data-ttu-id="af231-180">**Rettifica Importo**</span><span class="sxs-lookup"><span data-stu-id="af231-180">**Adjust Amount**</span></span>|<span data-ttu-id="af231-181">L'importo VL verrà rettificato per tutti gli utili e le perdite del tasso di cambio.</span><span class="sxs-lookup"><span data-stu-id="af231-181">The LCY amount is adjusted for any exchange rate gains or losses.</span></span> <span data-ttu-id="af231-182">Tali utili o perdite verranno registrati nel conto C/G nel campo **Importo** e nel campo **Conto utili C/G realizzati** o **Conto perdite C/G realizzate** della pagina **Valute** dei conti specificati per gli utili o le perdite.</span><span class="sxs-lookup"><span data-stu-id="af231-182">Exchange rate gains or losses are posted to the general ledger account in the **Amount** field and to the accounts you specified for gains or losses in the **Realized G/L Gains Account** and **Realized G/L Losses Account** fields on the **Currencies** page.</span></span>|  
    |<span data-ttu-id="af231-183">**Rettifica Importo in Valuta-Addiz.**</span><span class="sxs-lookup"><span data-stu-id="af231-183">**Adjust Additional-Currency Amount**</span></span>|<span data-ttu-id="af231-184">La valuta contabile addizionale verrà rettificata per tutti gli utili e le perdite del tasso di cambio.</span><span class="sxs-lookup"><span data-stu-id="af231-184">The additional reporting currency is adjusted for any exchange rate gains or losses.</span></span> <span data-ttu-id="af231-185">Tali utili o perdite verranno registrati nel conto C/G nel campo **Importo in valuta addiz.** e nel campo **Conto utili C/G realizzati** o **Conto perdite C/G realizzate** della pagina **Valute** dei conti specificati per gli utili o le perdite.</span><span class="sxs-lookup"><span data-stu-id="af231-185">Exchange rate gains or losses are posted to the general ledger account in the **Additional-Currency Amount** field and to the accounts you specified for gains or losses in the **Realized G/L Gains Account** and **Realized G/L Losses Account** fields on the **Currencies** page.</span></span>|  

### <a name="to-activate-the-additional-reporting-currency"></a><span data-ttu-id="af231-186">Per attivare la valuta contabile addizionale</span><span class="sxs-lookup"><span data-stu-id="af231-186">To activate the additional reporting currency</span></span>  
1. <span data-ttu-id="af231-187">Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Setup contabilità generale** e quindi scegliere il collegamento correlato.</span><span class="sxs-lookup"><span data-stu-id="af231-187">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Ledger Setup**, and then choose the related link.</span></span>  
2. <span data-ttu-id="af231-188">Nella pagina **Setup contabilità generale** scegliere il campo **Valuta contabile addizionale** per selezionare la valuta addizionale in cui si desidera effettuare la registrazione.</span><span class="sxs-lookup"><span data-stu-id="af231-188">On the **General Ledger Setup** page, choose the **Additional Reporting Currency** field to select the additional currency that you want to report in.</span></span>  
3. <span data-ttu-id="af231-189">Quando si esce dal campo, verrà visualizzato un messaggio di conferma in [!INCLUDE[d365fin](includes/d365fin_md.md)] in cui sono descritti gli effetti dell'attivazione della valuta contabile addizionale.</span><span class="sxs-lookup"><span data-stu-id="af231-189">When you leave the field, [!INCLUDE[d365fin](includes/d365fin_md.md)] displays a confirmation message describing the effects of activating the additional reporting currency.</span></span>  
4. <span data-ttu-id="af231-190">Selezionare il pulsante **Sì** per confermare che si desidera attivare la valuta.</span><span class="sxs-lookup"><span data-stu-id="af231-190">Choose the **Yes** button to confirm that you want to activate the currency.</span></span>  
5. <span data-ttu-id="af231-191">Verrà aperto il processo batch **Rett. valuta cont. aggiuntiva**.</span><span class="sxs-lookup"><span data-stu-id="af231-191">The **Adjust Add. Reporting Currency** batch job opens.</span></span>

    <span data-ttu-id="af231-192">Con questo processo è possibile convertire gli importi VL nei movimenti esistenti nella valuta contabile addizionale.</span><span class="sxs-lookup"><span data-stu-id="af231-192">This batch job converts LCY amounts on existing entries to the additional reporting currency.</span></span> <span data-ttu-id="af231-193">Nel processo batch viene utilizzato un tasso di cambio predefinito copiato dal tasso di cambio valido alla data di lavoro nella pagina **Tassi di cambio valuta**.</span><span class="sxs-lookup"><span data-stu-id="af231-193">The batch job uses a default exchange rate copied from the exchange rate that is valid on the work date on the **Currency Exchange Rates** page.</span></span> <span data-ttu-id="af231-194">Gli importi residui che si verificano nella conversione della valuta locale in valuta contabile addizionale vengono registrati nei conti utili e nei conti perdite residui specificati nella pagina **Valute**.</span><span class="sxs-lookup"><span data-stu-id="af231-194">Residual amounts that occur on conversion of LCY to additional reporting currency are posted to the residual gains and losses accounts specified on the **Currencies** page.</span></span> <span data-ttu-id="af231-195">La data di registrazione e il numero di documento di questi movimenti saranno gli stessi del movimento C/G originale.</span><span class="sxs-lookup"><span data-stu-id="af231-195">The posting date and document number for these entries are the same as for the original general ledger entry.</span></span> <span data-ttu-id="af231-196">Dopo la registrazione di tutti questi movimenti residui, con il processo batch viene registrato un movimento di arrotondamento alla data di chiusura di ogni anno chiuso nel conto profitti/perdite.</span><span class="sxs-lookup"><span data-stu-id="af231-196">After all these residual entries are posted, the batch job posts a rounding entry on the closing date of each closed year to the retained earnings account.</span></span> <span data-ttu-id="af231-197">In questo modo viene garantito che il saldo finale dei conti di entrata di ogni anno chiuso sia 0, sia in valuta locale sia nella valuta contabile addizionale.</span><span class="sxs-lookup"><span data-stu-id="af231-197">This is to make sure that the ending balance of the income accounts for each closed years is 0 in both LCY and the additional reporting currency.</span></span>
6. <span data-ttu-id="af231-198">Compilare i campi come necessario.</span><span class="sxs-lookup"><span data-stu-id="af231-198">Fill in the fields as necessary.</span></span> [!INCLUDE [tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]      
7. <span data-ttu-id="af231-199">Scegliere **OK** per eseguire il processo batch.</span><span class="sxs-lookup"><span data-stu-id="af231-199">Choose the **OK** button to run the batch job.</span></span>  

<span data-ttu-id="af231-200">Dopo avere eseguito il processo batch, gli importi nei seguenti movimenti esistenti saranno espressi sia nella valuta locale che in quella addizionale:</span><span class="sxs-lookup"><span data-stu-id="af231-200">After running the batch job, amounts on the following existing entries will be in both LCY and in the additional reporting currency:</span></span>  

- <span data-ttu-id="af231-201">Movimenti C/G</span><span class="sxs-lookup"><span data-stu-id="af231-201">General ledger entries</span></span>  
- <span data-ttu-id="af231-202">Mov. collegamento articoli</span><span class="sxs-lookup"><span data-stu-id="af231-202">Item application entries</span></span>  
- <span data-ttu-id="af231-203">Movimenti IVA</span><span class="sxs-lookup"><span data-stu-id="af231-203">VAT entries</span></span>  
- <span data-ttu-id="af231-204">Movimenti cont. commesse</span><span class="sxs-lookup"><span data-stu-id="af231-204">Job ledger entries</span></span>  
- <span data-ttu-id="af231-205">Movimenti valorizzazione</span><span class="sxs-lookup"><span data-stu-id="af231-205">Value entries</span></span>  
- <span data-ttu-id="af231-206">Righe degli ordini di produzione</span><span class="sxs-lookup"><span data-stu-id="af231-206">Production order lines</span></span>  
- <span data-ttu-id="af231-207">Movimenti contabili ordini di produzione</span><span class="sxs-lookup"><span data-stu-id="af231-207">Production order ledger entries</span></span>  

<span data-ttu-id="af231-208">Per tutti i movimenti futuri dello stesso tipo gli importi verranno inoltre registrati sia nella valuta locale che in quella addizionale.</span><span class="sxs-lookup"><span data-stu-id="af231-208">In addition, all future entries of the same type will have amounts recorded in both LCY and the additional reporting currency.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="af231-209">Il campo **Valuta contabile addizionale** verrà attivata solo dopo aver fatto clic sul pulsante **OK** nel processo batch **Rett. valuta cont. addizionale**.</span><span class="sxs-lookup"><span data-stu-id="af231-209">The **Add. Reporting Currency** field will only be activated after you choose the **OK** button in the **Adjust Add. Reporting Currency** batch job.</span></span>  

## <a name="see-also"></a><span data-ttu-id="af231-210">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="af231-210">See Also</span></span>
[<span data-ttu-id="af231-211">Aggiornare i tassi di cambio valuta</span><span class="sxs-lookup"><span data-stu-id="af231-211">Update Currency Exchange Rates</span></span>](finance-how-update-currencies.md)  
[<span data-ttu-id="af231-212">Chiusura di anni e periodi</span><span class="sxs-lookup"><span data-stu-id="af231-212">Closing Years and Periods</span></span>](year-close-years-periods.md)  
<span data-ttu-id="af231-213">[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="af231-213">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
