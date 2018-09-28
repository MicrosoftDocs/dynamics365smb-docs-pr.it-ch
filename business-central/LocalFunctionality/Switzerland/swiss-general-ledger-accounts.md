---
title: "Conti di contabilità generale per la Svizzera"
description: I miglioramenti svizzeri includono funzioni speciali di conto C/G.
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
ms.openlocfilehash: f9ae0951b0821cf330d22e810abce56002cd8339
ms.contentlocale: it-ch
ms.lasthandoff: 09/28/2018

---
# <a name="swiss-general-ledger-accounts"></a><span data-ttu-id="a22ab-103">Conti di contabilità generale per la Svizzera</span><span class="sxs-lookup"><span data-stu-id="a22ab-103">Swiss General Ledger Accounts</span></span>
[!INCLUDE[d365fin](../../includes/d365fin_md.md)] <span data-ttu-id="a22ab-104">include i miglioramenti svizzeri per i conti C/G.</span><span class="sxs-lookup"><span data-stu-id="a22ab-104"> includes Swiss enhancements to general ledger accounts.</span></span>

- <span data-ttu-id="a22ab-105">Gestire i saldi in valuta estera di un conto bancario nella contabilità generale.</span><span class="sxs-lookup"><span data-stu-id="a22ab-105">Maintain the foreign currency balances of a bank account in the general ledger.</span></span>  
- <span data-ttu-id="a22ab-106">Ordinare i numeri di conto della contabilità generale nella finestra **Piano dei conti**.</span><span class="sxs-lookup"><span data-stu-id="a22ab-106">Sort general ledger account numbers in the **Chart of Accounts** window.</span></span>  
- <span data-ttu-id="a22ab-107">Visualizzare l'anteprima degli effetti che avrebbe la contabilizzazione delle registrazioni COGE sui saldi di alcuni conti di contabilità generale prima di effettuarla effettivamente.</span><span class="sxs-lookup"><span data-stu-id="a22ab-107">Preview the effects that posting general journals would have on the balances of certain general ledger accounts before actually posting them.</span></span>  

## <a name="general-ledger-accounts-and-general-journals"></a><span data-ttu-id="a22ab-108">Conti di contabilità generale e registrazioni COGE</span><span class="sxs-lookup"><span data-stu-id="a22ab-108">General Ledger Accounts and General Journals</span></span>  
<span data-ttu-id="a22ab-109">Le aziende hanno spesso conti bancari diversi per le valute estere e hanno un conto C/G per ogni conto bancario.</span><span class="sxs-lookup"><span data-stu-id="a22ab-109">Companies often have different bank accounts for foreign currencies, and have a general ledger account for each bank account.</span></span> <span data-ttu-id="a22ab-110">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], è possibile impostare le informazioni relative al codice valuta e al saldo in valuta estera nella finestra **Piano dei conti**.</span><span class="sxs-lookup"><span data-stu-id="a22ab-110">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you can set up currency code and foreign currency balance information in the **Chart of Accounts** window.</span></span> <span data-ttu-id="a22ab-111">Ciò consente di mantenere il saldo originale in valuta estera di un conto bancario.</span><span class="sxs-lookup"><span data-stu-id="a22ab-111">This allows you to maintain the original foreign currency balance of a bank account.</span></span> <span data-ttu-id="a22ab-112">Per ulteriori informazioni, vedere [Finestra Piano dei Conti](assetId:///fa407624-b670-44b6-8397-91aa606e4c39) e [Tabella Conto C/G](assetId:///a65c2b09-9bb2-43db-8c53-c047bfc49777).</span><span class="sxs-lookup"><span data-stu-id="a22ab-112">For more information, see [Chart of Accounts Window](assetId:///fa407624-b670-44b6-8397-91aa606e4c39) and [G/L Account Table](assetId:///a65c2b09-9bb2-43db-8c53-c047bfc49777).</span></span>  

<span data-ttu-id="a22ab-113">Ad esempio, un'azienda ha due conti bancari: uno per la valuta locale (VL) e uno per gli euro (EUR).</span><span class="sxs-lookup"><span data-stu-id="a22ab-113">For example, a company has two bank accounts: one for local currency (LCY) and one for euros (EUR).</span></span> <span data-ttu-id="a22ab-114">È necessario creare un conto C/G per ciascun conto bancario.</span><span class="sxs-lookup"><span data-stu-id="a22ab-114">You must create a general ledger account for each bank account.</span></span> <span data-ttu-id="a22ab-115">Per il conto in EUR, definire il codice valuta come **EUR** e contabilizzare le registrazioni in EUR o VL.</span><span class="sxs-lookup"><span data-stu-id="a22ab-115">For the EUR account, define the currency code as **EUR** and post journals in EUR or LCY.</span></span>  

<span data-ttu-id="a22ab-116">Quando cambia il tasso di cambio per EUR e VL, è possibile aggiornare e modificare il saldo in valuta locale per il conto C/G EUR usando il processo di batch di rettifica dei tassi di cambio.</span><span class="sxs-lookup"><span data-stu-id="a22ab-116">When the exchange rate for EUR and LCY changes, you can update and adjust the local currency balance for the EUR general ledger account using the adjust exchange rates batch job.</span></span> <span data-ttu-id="a22ab-117">Questo processo batch crea e registra i movimenti di rettifica della valuta nella contabilità generale e aggiorna il saldo VL.</span><span class="sxs-lookup"><span data-stu-id="a22ab-117">This batch job creates and posts currency adjustment entries to the general ledger and updates the LCY balance.</span></span>  

## <a name="data-type-for-general-ledger-accounts"></a><span data-ttu-id="a22ab-118">Tipo di dati per i conti C/G</span><span class="sxs-lookup"><span data-stu-id="a22ab-118">Data Type for General Ledger Accounts</span></span>  
<span data-ttu-id="a22ab-119">Il tipo di dati è impostato su un testo per il numero di conto C/G o il codice conto per supportare i requisiti di ordinamento per il piano dei conti comune Kontenrahmen Käfer (KMU) svizzero standardizzato.</span><span class="sxs-lookup"><span data-stu-id="a22ab-119">The data type is set to text for the general ledger account number or account code to support the sorting requirements for the standardized Swiss Kontenrahmen Käfer (KMU) common chart of accounts.</span></span> <span data-ttu-id="a22ab-120">Per ulteriori informazioni, vedere [Finestra Piano dei conti](assetId:///fa407624-b670-44b6-8397-91aa606e4c39).</span><span class="sxs-lookup"><span data-stu-id="a22ab-120">For more information, see [Chart of Accounts Window](assetId:///fa407624-b670-44b6-8397-91aa606e4c39).</span></span> <span data-ttu-id="a22ab-121">La lista dei numeri di conto viene ordinata in base al tipo di dati di testo.</span><span class="sxs-lookup"><span data-stu-id="a22ab-121">The account numbers list is sorted based on the text data type.</span></span> <span data-ttu-id="a22ab-122">Il piano di conti KMU contiene i seguenti numeri di conto:</span><span class="sxs-lookup"><span data-stu-id="a22ab-122">The KMU chart of accounts contains the following account numbers:</span></span>  

- <span data-ttu-id="a22ab-123">1176</span><span class="sxs-lookup"><span data-stu-id="a22ab-123">1176</span></span>  
- <span data-ttu-id="a22ab-124">119.0</span><span class="sxs-lookup"><span data-stu-id="a22ab-124">119.0</span></span>  
- <span data-ttu-id="a22ab-125">1190</span><span class="sxs-lookup"><span data-stu-id="a22ab-125">1190</span></span>  

## <a name="viewing-temporary-balances-in-general-journals"></a><span data-ttu-id="a22ab-126">Visualizzazione di saldi temporanei nelle registrazioni di contabilità generale</span><span class="sxs-lookup"><span data-stu-id="a22ab-126">Viewing Temporary Balances in General Journals</span></span>  
<span data-ttu-id="a22ab-127">Prima di contabilizzare una registrazione COGE è possibile visualizzare l'anteprima degli effetti che avrebbe la contabilizzazione sui saldi di alcuni conti di contabilità generale.</span><span class="sxs-lookup"><span data-stu-id="a22ab-127">Before posting a general journal you can preview the effect that posting would have on the balances of certain general ledger accounts.</span></span> <span data-ttu-id="a22ab-128">È possibile aprire una finestra di statistiche che mostra i saldi dei conti e i saldi delle righe attive che includevano i valori non registrati per la registrazione corrente.</span><span class="sxs-lookup"><span data-stu-id="a22ab-128">You can open a statistics window that shows the balances of the accounts, and the balances of the active lines that included the unposted values for the current journal.</span></span> <span data-ttu-id="a22ab-129">Per ulteriori informazioni, vedere [Visualizzare i saldi temporanei nelle registrazioni di contabilità generale](how-to-view-temporary-balances-in-general-ledger-journals.md).</span><span class="sxs-lookup"><span data-stu-id="a22ab-129">For more information, see [View Temporary Balances in General Ledger Journals](how-to-view-temporary-balances-in-general-ledger-journals.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="a22ab-130">Vedi anche</span><span class="sxs-lookup"><span data-stu-id="a22ab-130">See Also</span></span>  
 <span data-ttu-id="a22ab-131">[Visualizzare i saldi temporanei nelle registrazioni di contabilità generale](how-to-view-temporary-balances-in-general-ledger-journals.md) </span><span class="sxs-lookup"><span data-stu-id="a22ab-131">[View Temporary Balances in General Ledger Journals](how-to-view-temporary-balances-in-general-ledger-journals.md) </span></span>  
 [<span data-ttu-id="a22ab-132">Funzionalità locale per la Svizzera</span><span class="sxs-lookup"><span data-stu-id="a22ab-132">Switzerland Local Functionality</span></span>](switzerland-local-functionality.md)

