---
title: Domande frequenti sulle visualizzazioni elenco
description: Informazioni dettagliate sul salvataggio di filtri come visualizzazioni elenco.
author: mikebcMSFT
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: list, filter, pane, views
ms.date: 01/01/2019
ms.author: mikebc
ms.openlocfilehash: d2caa1d9b84d99c0b43a70bca1c45da81138f7b9
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 10/01/2019
ms.locfileid: "2316851"
---
# <a name="list-views-faq"></a><span data-ttu-id="8cfe9-103">Domande frequenti sulle visualizzazioni elenco</span><span class="sxs-lookup"><span data-stu-id="8cfe9-103">List Views FAQ</span></span>
<span data-ttu-id="8cfe9-104">Questo argomento contiene le risposte alle domande più frequenti sull'utilizzo di visualizzazioni elenco e sul salvataggio di filtri poste da utenti esperti.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-104">This topic answers questions that our advanced users often ask about working with list views and saving filters.</span></span>  

### <a name="how-do-views-handle-expressions"></a><span data-ttu-id="8cfe9-105">In che modo le visualizzazioni gestiscono le espressioni?</span><span class="sxs-lookup"><span data-stu-id="8cfe9-105">How do views handle expressions?</span></span>
<span data-ttu-id="8cfe9-106">Quando si salva una visualizzazione che include filtri con espressioni, come intervalli di date, operatori, parole chiave o token di filtro, viene salvata l'espressione ma non i valori risultanti.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-106">When saving a view that includes filters with expressions, such as date ranges, operators, keywords or filter tokens, the expression and not the resulting values is saved.</span></span> <span data-ttu-id="8cfe9-107">Ad esempio, il salvataggio di una visualizzazione che filtra in base al campo **Data di creazione** con l'espressione **-1W..today** troverà sempre record relativi alla data corrente, anche quando alla visualizzazione si accede il mese successivo.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-107">For example, saving a view that filters on the **Created Date** field with the expression **-1W..today** will always find records relative to the current date, even when the view is accessed next month.</span></span>

### <a name="where-are-list-views-saved"></a><span data-ttu-id="8cfe9-108">Dove vengono salvate le visualizzazioni elenco?</span><span class="sxs-lookup"><span data-stu-id="8cfe9-108">Where are list views saved?</span></span>
<span data-ttu-id="8cfe9-109">Analogamente alle operazioni eseguite per nascondere un campo o riorganizzare il menu di navigazione, le visualizzazioni elenco fanno parte della personalizzazione dell'utente e sono archiviate nel database.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-109">Similarly to hiding a field or reordering your navigation menu, list views are a part of user personalization and are stored in the database.</span></span> <span data-ttu-id="8cfe9-110">L'annullamento dell'intera personalizzazione in un elenco rimuoverà in modo permanente anche le visualizzazioni personali e ulteriori personalizzazioni come il riordino delle visualizzazioni.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-110">Clearing all personalization on a list will also permanently remove your personal views and clear additional personalization such as re-ordering of views.</span></span> <span data-ttu-id="8cfe9-111">Per ulteriori informazioni, vedere [Personalizzare l'area di lavoro](ui-personalization-user.md).</span><span class="sxs-lookup"><span data-stu-id="8cfe9-111">For more information see [Personalize your workspace](ui-personalization-user.md).</span></span>

### <a name="why-dont-i-have-a-save-icon"></a><span data-ttu-id="8cfe9-112">Perché non è presente un'icona Salva?</span><span class="sxs-lookup"><span data-stu-id="8cfe9-112">Why don't I have a Save icon?</span></span>
<span data-ttu-id="8cfe9-113">L'icona Salva e il menu delle opzioni non sono visualizzati insieme alle visualizzazioni nel riquadro filtri se la personalizzazione è disabilitata per un ruolo utente.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-113">The save icon and options menu are not displayed alongside views in the filter pane if personalization is disabled for a user role.</span></span> <span data-ttu-id="8cfe9-114">Gli utenti che non hanno la personalizzazione abilitata sono comunque in grado di accedere alle visualizzazioni di sistema che sono una parte standard della pagina, nonché di modificare o creare altri filtri.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-114">Users who do not have personalization enabled are still able to access system views that are a standard part of the page, modify or create more filters.</span></span>

### <a name="on-which-page-types-can-i-use-list-views"></a><span data-ttu-id="8cfe9-115">In quali tipi di pagina è possibile utilizzare visualizzazioni elenco?</span><span class="sxs-lookup"><span data-stu-id="8cfe9-115">On which page types can I use list views?</span></span>
<span data-ttu-id="8cfe9-116">Le visualizzazioni sono disponibili solo nelle pagine di elenchi e fogli di lavoro.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-116">Views are only available on list and worksheet pages.</span></span>

### <a name="are-views-also-available-on-other-form-factors"></a><span data-ttu-id="8cfe9-117">Le visualizzazioni sono disponibili anche in altri fattori di forma?</span><span class="sxs-lookup"><span data-stu-id="8cfe9-117">Are views also available on other form factors?</span></span>
<span data-ttu-id="8cfe9-118">Sì.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-118">Yes.</span></span> <span data-ttu-id="8cfe9-119">Tutte le visualizzazioni salvate nel browser desktop o nell'applicazione desktop saranno disponibili anche nel tablet o nello smartphone.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-119">Any views you save on your desktop browser or desktop app will also be available on your tablet or smartphone.</span></span> <span data-ttu-id="8cfe9-120">Non è possibile modificare o personalizzare visualizzazioni in dispositivi mobili.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-120">You cannot modify or personalize views on mobile devices.</span></span>

### <a name="are-my-personal-views-always-accessible"></a><span data-ttu-id="8cfe9-121">Le visualizzazioni personali sono sempre accessibili?</span><span class="sxs-lookup"><span data-stu-id="8cfe9-121">Are my personal views always accessible?</span></span>
<span data-ttu-id="8cfe9-122">Le stesse visualizzazioni sono disponibili in una pagina di elenco se vi si accede dal menu di navigazione, tramite la finestra della **funzionalità delle informazioni** o tramite un collegamento URL alla pagina elenco.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-122">The same views are available on a list page if you access it from the navigation menu, through the **Tell Me** window, or through a URL link to the list page.</span></span> <span data-ttu-id="8cfe9-123">Le visualizzazioni non sono disponibili in parti di elenco, ricerche o ogni volta che una pagina di elenco viene visualizzata come finestra di dialogo.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-123">Views are not available in list parts, lookups or whenever a list page is displayed as a dialog.</span></span>

### <a name="how-do-i-return-a-view-to-its-original-filters-after-modifying-them"></a><span data-ttu-id="8cfe9-124">Come è possibile ripristinare i filtri originali di una visualizzazione dopo averli modificati?</span><span class="sxs-lookup"><span data-stu-id="8cfe9-124">How do I return a view to its original filters after modifying them?</span></span>
<span data-ttu-id="8cfe9-125">Nella parte inferiore del riquadro filtri, selezionare l'azione **Reimposta filtri** per annullare le modifiche ai filtri apportate alla visualizzazione e ripristinare i campi filtrati e i criteri di filtro originali.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-125">At the bottom of the filter pane, choose the **Reset filters** action to clear filter changes you have made to the view and return to its original filtered fields and filter criteria.</span></span>

### <a name="what-is-the-difference-between-hiding-and-removing-views"></a><span data-ttu-id="8cfe9-126">Qual è la differenza tra nascondere e rimuovere le visualizzazioni?</span><span class="sxs-lookup"><span data-stu-id="8cfe9-126">What is the difference between hiding and removing views?</span></span>
<span data-ttu-id="8cfe9-127">La rimozione di una visualizzazione eliminerà definitivamente quella visualizzazione.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-127">Removing a view will permanently delete that view.</span></span> <span data-ttu-id="8cfe9-128">Quando si nasconde una visualizzazione, questa viene rimossa temporaneamente dal riquadro filtri, ma è possibile renderla di nuovo visibile in seguito scegliendo l'azione **Mostra**.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-128">Hiding a view allows you to temporarily hide it from the filter pane, but you can unhide it again later by choosing the **Show** action.</span></span>

### <a name="how-can-i-share-my-views-with-others"></a><span data-ttu-id="8cfe9-129">Come è possibile condividere le visualizzazioni con altri utenti?</span><span class="sxs-lookup"><span data-stu-id="8cfe9-129">How can I share my views with others?</span></span>
[!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="8cfe9-130">non fornisce un modo di condividere la visualizzazione elenco precisa, ma è possibile condividere i filtri correnti di modo che altri utenti possano visualizzare un elenco di record simile.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-130">does not provide a way to share the precise list view, but you can share your current filters so that other users can see a similar list of records.</span></span> <span data-ttu-id="8cfe9-131">Nel browser desktop, copiare semplicemente l'URL e condividerlo con i colleghi.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-131">In your desktop browser, simply copy the URL and share it with your colleagues.</span></span> <span data-ttu-id="8cfe9-132">La condivisione dei filtri non garantisce al destinatario un set di filtri identico a quello visualizzato nel proprio browser.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-132">Sharing filters is not guaranteed to give the recipient an identical set of filters that you see in your browser.</span></span>

### <a name="can-i-search-for-views-in-the-tell-me-window"></a><span data-ttu-id="8cfe9-133">È possibile cercare visualizzazioni nella finestra della funzionalità delle informazioni?</span><span class="sxs-lookup"><span data-stu-id="8cfe9-133">Can I search for views in the Tell Me window?</span></span>
<span data-ttu-id="8cfe9-134">No.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-134">No.</span></span> <span data-ttu-id="8cfe9-135">La finestra della **funzionalità delle informazioni** visualizza solo i risultati della ricerca per la pagina, ma è comunque possibile accedere alla visualizzazione preferita dalla pagina.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-135">The **Tell Me** window only displays search results for the page, but you are only a step away from getting to your favorite view once you navigate to the page.</span></span>

### <a name="what-is-shared-layout"></a><span data-ttu-id="8cfe9-136">Cos'è un layout condiviso?</span><span class="sxs-lookup"><span data-stu-id="8cfe9-136">What is shared layout?</span></span>
<span data-ttu-id="8cfe9-137">Tutte le visualizzazioni in una pagina di elenco condividono un layout di colonna comune che include le colonne che vengono visualizzate, la relativa sequenza, larghezza, riquadro di blocco e impostazioni Accesso rapido.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-137">All views on a list page share a common column layout that includes which columns are displayed, their sequence, width, freeze pane and Quick Entry settings.</span></span> <span data-ttu-id="8cfe9-138">La personalizzazione di qualsiasi layout di colonna influirà anche su altre visualizzazioni che condividono lo stesso layout nella pagina di elenco.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-138">Personalizing any of the column layout will also affect other views sharing the same layout on the list page.</span></span>

<span data-ttu-id="8cfe9-139">Alcune visualizzazioni di sistema possono avere layout univoci delle colonne nell'elenco.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-139">Some system views can have unique layouts of the columns in the list.</span></span> <span data-ttu-id="8cfe9-140">Ad esempio, potrebbero riorganizzare le colonne per visualizzare solo le colonne più pertinenti a quella visualizzazione.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-140">For example, they could re-arrange columns to display only the columns most relevant to that view.</span></span> <span data-ttu-id="8cfe9-141">È possibile identificare quali visualizzazioni hanno layout univoci scegliendo l'icona ![Mostra altre opzioni](media/show-more-options-icon.png "Mostra altre opzioni") e deselezionando la casella di controllo **Layout condiviso** se questa è selezionata.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-141">You can identify which views have unique layouts by choosing the ![Show more options](media/show-more-options-icon.png "Show more options") icon and observing that the **Shared layout** check box is not selected.</span></span> <span data-ttu-id="8cfe9-142">Come utente, è possibile personalizzare il layout di colonna di una visualizzazione con un layout univoco senza che ciò influisca sulle altre visualizzazioni nella pagina di elenco.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-142">As a user, you can personalize the column layout for a view with unique layout without it affecting any of the other views on the list page.</span></span> <span data-ttu-id="8cfe9-143">Solo gli sviluppatori possono definire un layout di colonna univoco per una visualizzazione che inizialmente ha un layout condiviso.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-143">Only developers can define a unique column layout for a view that initially has a shared layout.</span></span>

### <a name="what-does-the-show-system-filters-link-do"></a><span data-ttu-id="8cfe9-144">Qual è la funzione del collegamento Mostra filtri di sistema?</span><span class="sxs-lookup"><span data-stu-id="8cfe9-144">What does the Show System Filters link do?</span></span>
<span data-ttu-id="8cfe9-145">In alcune pagine di elenco, il riquadro filtri visualizzerà **Mostra filtri di sistema** nella parte inferiore quando la pagina include filtri specificati dal sistema.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-145">On some list pages, the filter pane will display **Show system filters** at the bottom of the filter pane when the page includes filters specified by the system.</span></span> <span data-ttu-id="8cfe9-146">Questi filtri speciali sono in genere utilizzati per visualizzare record basati sul contesto corrente, ad esempio quando un elenco di ordini deve essere filtrato per un cliente specifico.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-146">These special filters are typically used to display records based on the current context, such as when a list of orders has to be filtered for a specific customer.</span></span>

<span data-ttu-id="8cfe9-147">I filtri di sistema sono impostati dagli sviluppatori utilizzando il gruppo di filtri 0.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-147">System filters are set by developers using filter group 0.</span></span> <span data-ttu-id="8cfe9-148">Per dettagli tecnici sui filtri di sistema, vedere [Funzione Filtergroup](https://docs.microsoft.com/en-us/dynamics-nav/filtergroup-function--record-)</span><span class="sxs-lookup"><span data-stu-id="8cfe9-148">For technical details about system filters, see [Filtergroup Function](https://docs.microsoft.com/en-us/dynamics-nav/filtergroup-function--record-)</span></span>

### <a name="i-see-multiple-views-on-my-page-but-i-did-not-create-them-where-did-they-come-from"></a><span data-ttu-id="8cfe9-149">La pagina contiene varie visualizzazioni non create dall'utente.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-149">I see multiple views on my page, but I did not create them.</span></span> <span data-ttu-id="8cfe9-150">Qual è la loro origine?</span><span class="sxs-lookup"><span data-stu-id="8cfe9-150">Where did they come from?</span></span>
<span data-ttu-id="8cfe9-151">Le visualizzazioni presenti in un qualsiasi elenco sono una combinazione delle visualizzazioni personali e delle visualizzazioni di sistema.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-151">The views you see on any list are a combination of your personal views together with system views.</span></span> <span data-ttu-id="8cfe9-152">Le visualizzazioni di sistema possono essere originate dall'applicazione aziendale, dalle estensioni oppure possono essere specifiche del ruolo se l'elenco è stato personalizzato per il proprio ruolo.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-152">System views may originate from the business application, from extensions, or may be role-specific if the list was customized for your role.</span></span>

### <a name="why-do-some-views-provide-fewer-options"></a><span data-ttu-id="8cfe9-153">Perché alcune visualizzazioni presentano meno opzioni?</span><span class="sxs-lookup"><span data-stu-id="8cfe9-153">Why do some views provide fewer options?</span></span>
<span data-ttu-id="8cfe9-154">Alcune visualizzazioni forniscono solo l'opzione di salvare una copia della visualizzazione, mentre altre non consentono il salvataggio delle modifiche alla visualizzazione.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-154">Some views only provide the option to save a copy of the view, while others do not allow saving changes to the view.</span></span> <span data-ttu-id="8cfe9-155">Il modo in cui la visualizzazione è stata creata determina le opzioni disponibili per quella visualizzazione.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-155">How the view was created determines the options available to that view.</span></span> <span data-ttu-id="8cfe9-156">Le visualizzazioni possono essere create in vari modi:</span><span class="sxs-lookup"><span data-stu-id="8cfe9-156">Views can be created in multiple ways:</span></span>
- <span data-ttu-id="8cfe9-157">Visualizzazioni personali salvate</span><span class="sxs-lookup"><span data-stu-id="8cfe9-157">Personal views that you saved</span></span>
- <span data-ttu-id="8cfe9-158">Visualizzazioni di sistema che sono una parte standard dell'applicazione aziendale o che vengono aggiunte dalle estensioni o dalle visualizzazioni specifiche del ruolo.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-158">System views that are a standard part of the business application, or added by extensions or role-specific views.</span></span> <span data-ttu-id="8cfe9-159">A differenza delle visualizzazioni personali, non è possibile salvare le modifiche ai filtri nelle visualizzazioni di sistema.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-159">Unlike personal views, you cannot save changes to filters back to that system view.</span></span>
- <span data-ttu-id="8cfe9-160">Visualizzazioni di sistema legacy che sono una parte standard dell'applicazione aziendale ma che sono state create utilizzando versioni precedenti di [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="8cfe9-160">Legacy system views that are a standard part of the business application but were created using older versions of [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="8cfe9-161">Queste visualizzazioni offrono molte meno opzioni.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-161">These views offer significantly fewer options.</span></span> <span data-ttu-id="8cfe9-162">È possibile salvarle solo come nuova visualizzazione e non possono nemmeno essere nascoste o riordinate.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-162">You can only save them as a new view and cannot hide or reorder them either.</span></span> <span data-ttu-id="8cfe9-163">Da notare che le visualizzazioni di sistema legacy verranno sospese in un futuro aggiornamento di [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="8cfe9-163">Note that legacy system views will be discontinued in a future update to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

### <a name="how-do-i-convert-legacy-system-views"></a><span data-ttu-id="8cfe9-164">Come si convertono le visualizzazioni di sistema legacy?</span><span class="sxs-lookup"><span data-stu-id="8cfe9-164">How do I convert legacy system views?</span></span>
<span data-ttu-id="8cfe9-165">Le visualizzazioni di sistema legacy sono visualizzazioni elenco che sono state create dagli sviluppatori nelle versioni precedenti di [!INCLUDE[d365fin](includes/d365fin_md.md)] mediante posizionamento delle stesse nella pagina Gestione ruolo utente.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-165">Legacy system views are list views that were created by developers in older versions of [!INCLUDE[d365fin](includes/d365fin_md.md)] by placing them on the Role Center page.</span></span> <span data-ttu-id="8cfe9-166">Queste visualizzazioni sono ora visualizzate direttamente nella pagina di elenco ma offrono un'esperienza meno qualitativa e un numero significativamente inferiore di opzioni.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-166">These views are now displayed directly on the list page but offer a degraded experience and significantly fewer options.</span></span> <span data-ttu-id="8cfe9-167">È possibile convertire una visualizzazione di sistema legacy in una visualizzazione personale completamente personalizzabile salvandola come nuova visualizzazione.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-167">You can convert a legacy system view to a personal view that is fully customizable, simply by saving that legacy view as a new view.</span></span> <span data-ttu-id="8cfe9-168">Allo stesso modo, gli amministratori possono scegliere di convertire visualizzazioni di sistema legacy specifiche del ruolo personalizzando il ruolo utente e salvando la visualizzazione legacy come nuova visualizzazione specifica del ruolo.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-168">Similarly, administrators can choose to convert role-specific legacy system views by customizing the user role and saving the legacy view as a new role-specific view.</span></span>

<span data-ttu-id="8cfe9-169">Da notare che le visualizzazioni di sistema legacy verranno sospese in un futuro aggiornamento di [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="8cfe9-169">Note that legacy system views will be discontinued in a future update to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

### <a name="others-in-my-organization-need-similar-list-views-as-standard-what-can-i-do"></a><span data-ttu-id="8cfe9-170">Altri utenti nell'organizzazione necessitano di visualizzazioni elenco simili.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-170">Others in my organization need similar list views as standard.</span></span> <span data-ttu-id="8cfe9-171">Come si deve procedere?</span><span class="sxs-lookup"><span data-stu-id="8cfe9-171">What can I do?</span></span>
<span data-ttu-id="8cfe9-172">L'utilizzo di visualizzazioni personali è rapido ed efficace, ma [!INCLUDE[d365fin](includes/d365fin_md.md)] fornisce strumenti aggiuntivi per definire visualizzazioni elenco necessarie a ruoli utente specifici o a tutti gli utenti nell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-172">Working with personal views is quick and effective, but [!INCLUDE[d365fin](includes/d365fin_md.md)] provides additional tools to define list views needed by specific user roles or all users in the organization.</span></span>
 - <span data-ttu-id="8cfe9-173">Gli sviluppatori possono personalizzare l'ambiente e creare visualizzazioni elenco nelle estensioni per tutti gli utenti nell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-173">Developers can customize the environment and create list views in extensions for all users in the organization.</span></span>
 - <span data-ttu-id="8cfe9-174">Gli utenti non programmatori come gli amministratori o i responsabili di reparto possono creare visualizzazioni elenco specifiche del ruolo quando personalizzano un ruolo dalla pagina **Profili (ruoli)**.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-174">Non-coders such as administrators or department managers, can create role-specific list views when customizing a role from the **Profiles (Roles)** page.</span></span>

### <a name="i-work-with-multiple-languages-how-do-i-translate-the-name-of-the-view"></a><span data-ttu-id="8cfe9-175">Come è possibile tradurre il nome della visualizzazione?</span><span class="sxs-lookup"><span data-stu-id="8cfe9-175">I work with multiple languages: how do I translate the name of the view?</span></span>
<span data-ttu-id="8cfe9-176">Quando si salva una nuova visualizzazione o si rinomina una visualizzazione esistente, è necessario immettere un nome riconoscibile e significativo per quella visualizzazione.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-176">When saving a new view or renaming an existing view, you must enter a recognizable and meaningful name for that view.</span></span> <span data-ttu-id="8cfe9-177">Il nome viene salvato per la lingua corrente e verrà visualizzato anche quando si utilizza [!INCLUDE[d365fin](includes/d365fin_md.md)] in altre lingue.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-177">The name is saved for your current language and will be displayed also when you or other users work with [!INCLUDE[d365fin](includes/d365fin_md.md)] in different languages.</span></span> <span data-ttu-id="8cfe9-178">Per fornire nomi di visualizzazioni tradotti, è necessario cambiare lingua nella pagina **Impostazioni personali** e quindi rinominare la visualizzazione. In questo modo, si memorizzerà il nome tradotto nella nuova lingua.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-178">To provide translated view names, you must switch language using the **My Settings** page and then rename the view, which will store the translated name in the new language.</span></span>

### <a name="do-views-with-expressions-work-in-all-languages"></a><span data-ttu-id="8cfe9-179">Le visualizzazioni con espressioni sono utilizzabili con tutte le lingue?</span><span class="sxs-lookup"><span data-stu-id="8cfe9-179">Do views with expressions work in all languages?</span></span>
<span data-ttu-id="8cfe9-180">Le espressioni che utilizzano solo simboli, come "**|**" o **..**, sono considerate sicure in qualsiasi lingua.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-180">Expressions that only use symbols, such as '**|**' or **..**, are considered safe for users to access in any language.</span></span> <span data-ttu-id="8cfe9-181">Le visualizzazioni con espressioni che includono lettere, parole chiave o token di filtro sono utilizzabili solo con la lingua in cui sono state create.</span><span class="sxs-lookup"><span data-stu-id="8cfe9-181">Any views with expressions that include letters, keywords or filter tokens will only work for the language in which they were authored.</span></span>


### <a name="see-also"></a><span data-ttu-id="8cfe9-182">Vedere anche</span><span class="sxs-lookup"><span data-stu-id="8cfe9-182">See Also</span></span>  
[<span data-ttu-id="8cfe9-183">Salvare e personalizzare visualizzazioni elenco</span><span class="sxs-lookup"><span data-stu-id="8cfe9-183">Save and Personalize List Views</span></span>](ui-views.md)  
<span data-ttu-id="8cfe9-184">[Individuazione di funzionalità e informazioni](ui-search.md)  </span><span class="sxs-lookup"><span data-stu-id="8cfe9-184">[Finding Features and Information](ui-search.md)  </span></span>  
[<span data-ttu-id="8cfe9-185">Ricerca, filtro e ordinamento</span><span class="sxs-lookup"><span data-stu-id="8cfe9-185">Sorting, Searching and Filtering</span></span>](ui-enter-criteria-filters.md)  