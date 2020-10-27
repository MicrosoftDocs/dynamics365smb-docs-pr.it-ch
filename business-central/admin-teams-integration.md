---
title: Gestione dell'integrazione Microsoft Teams con Business Central | Microsoft Docs
description: Gestione dell'integrazione di Business Central con Microsoft Teams.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Teams, MS Teams, Microsoft Teams, Skype, Link, Microsoft 365, collaborate, collaboration, teamwork
ms.date: 10/08/2020
ms.author: jswymer
ms.openlocfilehash: 3c04dfb2f77eba906b2567ca9438849e1cc20861
ms.sourcegitcommit: 4bca699d2a5ce182eb5572d72fac4fb478c4f293
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 10/12/2020
ms.locfileid: "3989377"
---
# <a name="managing-microsoft-teams-integration-with-business-central"></a><span data-ttu-id="883ed-103">Gestione dell'integrazione di Microsoft Teams con Business Central</span><span class="sxs-lookup"><span data-stu-id="883ed-103">Managing Microsoft Teams Integration with Business Central</span></span>

[!INCLUDE [teams_preview.md](includes/teams_preview.md)]

<span data-ttu-id="883ed-104">Questo articolo fornisce una panoramica di ciò che è possibile fare come amministratore per controllare l'integrazione di Microsoft Teams con [!INCLUDE [prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="883ed-104">This article provides an overview of what you can do as an administrator to control Microsoft Teams integration with [!INCLUDE [prodshort](includes/prodshort.md)].</span></span>

## <a name="in-microsoft-teams"></a><span data-ttu-id="883ed-105">In Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="883ed-105">In Microsoft Teams</span></span>

### <a name="minimum-requirements"></a><span data-ttu-id="883ed-106">Requisiti minimi</span><span class="sxs-lookup"><span data-stu-id="883ed-106">Minimum requirements</span></span>

<span data-ttu-id="883ed-107">Questa sezione descrive i requisiti minimi per il funzionamento dell'app [!INCLUDE [prodshort](includes/prodshort.md)] in Teams.</span><span class="sxs-lookup"><span data-stu-id="883ed-107">This section describes the minimum requirements for the [!INCLUDE [prodshort](includes/prodshort.md)] app features to work in Teams.</span></span>

- <span data-ttu-id="883ed-108">Licenze richieste</span><span class="sxs-lookup"><span data-stu-id="883ed-108">Required licenses</span></span>

    <span data-ttu-id="883ed-109">Questa tabella offre una panoramica delle licenze necessarie per il funzionamento dell'app [!INCLUDE [prodshort](includes/prodshort.md)] in Teams.</span><span class="sxs-lookup"><span data-stu-id="883ed-109">This table gives you an overview of the licenses needed for the [!INCLUDE [prodshort](includes/prodshort.md)] app features to work in Teams.</span></span>

    |<span data-ttu-id="883ed-110">Quale</span><span class="sxs-lookup"><span data-stu-id="883ed-110">What</span></span>|<span data-ttu-id="883ed-111">Licenza Teams</span><span class="sxs-lookup"><span data-stu-id="883ed-111">Teams license</span></span>|<span data-ttu-id="883ed-112">Licenza Business Central</span><span class="sxs-lookup"><span data-stu-id="883ed-112">Business Central license</span></span>|
    |----|---|---|
    |<span data-ttu-id="883ed-113">Incollare un collegamento a un record [!INCLUDE [prodshort](includes/prodshort.md)] in una conversazione e inviarla come scheda.</span><span class="sxs-lookup"><span data-stu-id="883ed-113">Paste a link to a [!INCLUDE [prodshort](includes/prodshort.md)] record into a conversation, and send it as a card.</span></span>|<span data-ttu-id="883ed-114">![segno di spunta](media/check.png "selezionato")</span><span class="sxs-lookup"><span data-stu-id="883ed-114">![check mark](media/check.png "check")</span></span>|<span data-ttu-id="883ed-115">![segno di spunta](media/check.png "selezionato")</span><span class="sxs-lookup"><span data-stu-id="883ed-115">![check mark](media/check.png "check")</span></span>|
    |<span data-ttu-id="883ed-116">Visualizzare una scheda di un record [!INCLUDE [prodshort](includes/prodshort.md)] in una conversazione.</span><span class="sxs-lookup"><span data-stu-id="883ed-116">View a card of a [!INCLUDE [prodshort](includes/prodshort.md)] record in a conversation.</span></span>|<span data-ttu-id="883ed-117">![segno di spunta](media/check.png "selezionato")</span><span class="sxs-lookup"><span data-stu-id="883ed-117">![check mark](media/check.png "check")</span></span>||
    |<span data-ttu-id="883ed-118">Visualizzare altri dettagli di una scheda per un record [!INCLUDE [prodshort](includes/prodshort.md)] in una conversazione.</span><span class="sxs-lookup"><span data-stu-id="883ed-118">View more details of card for a [!INCLUDE [prodshort](includes/prodshort.md)] record in a conversation.</span></span>|<span data-ttu-id="883ed-119">![segno di spunta](media/check.png "selezionato")</span><span class="sxs-lookup"><span data-stu-id="883ed-119">![check mark](media/check.png "check")</span></span>|<span data-ttu-id="883ed-120">![segno di spunta](media/check.png "selezionato")</span><span class="sxs-lookup"><span data-stu-id="883ed-120">![check mark](media/check.png "check")</span></span>|

- <span data-ttu-id="883ed-121">Consentire le anteprime URL</span><span class="sxs-lookup"><span data-stu-id="883ed-121">Allow URL previews</span></span>

    <span data-ttu-id="883ed-122">L'impostazione dei criteri **Consenti anteprime URL** deve essere attivata.</span><span class="sxs-lookup"><span data-stu-id="883ed-122">**Allow URL previews** policy setting must be turned on.</span></span> <span data-ttu-id="883ed-123">In caso contrario, non è possibile generare una scheda per i collegamenti di Business Central incollati in una conversazione di Teams.</span><span class="sxs-lookup"><span data-stu-id="883ed-123">Otherwise, a card can't be generated for Business Central links pasted into a Teams conversation.</span></span> <span data-ttu-id="883ed-124">Per ulteriori informazioni su questa impostazione, vedere [Gestire i criteri di messaggistica in Teams](/microsoftteams/messaging-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="883ed-124">For more information about this setting, see [Manage messaging policies in Teams](/microsoftteams/messaging-policies-in-teams).</span></span>

### <a name="managing-the-business-central-app-optional"></a><span data-ttu-id="883ed-125">Gestione dell'app Business Central (opzionale)</span><span class="sxs-lookup"><span data-stu-id="883ed-125">Managing the Business Central app (optional)</span></span>

<span data-ttu-id="883ed-126">In qualità di amministratore di Teams, è possibile gestire tutte le app per l'organizzazione, inclusa l'app [!INCLUDE [prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="883ed-126">As a Teams administrator, you can manage all apps for your organization, including the [!INCLUDE [prodshort](includes/prodshort.md)] app.</span></span> <span data-ttu-id="883ed-127">È possibile approvare o installare l'app [!INCLUDE [prodshort](includes/prodshort.md)] per l'organizzazione, impedire all'utente di installare l'app e altro ancora.</span><span class="sxs-lookup"><span data-stu-id="883ed-127">You can approve or install the [!INCLUDE [prodshort](includes/prodshort.md)] app for your organization, block user's from installing the app, and more.</span></span>

<span data-ttu-id="883ed-128">Per ulteriori informazioni, vedere i seguenti articoli nella documentazione di Microsoft Teams:</span><span class="sxs-lookup"><span data-stu-id="883ed-128">For more information, see the following articles in the Microsoft Teams documentation:</span></span>

- [<span data-ttu-id="883ed-129">Gestire le app nell'interfaccia di amministrazione di Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="883ed-129">Manage your apps in the Microsoft Teams admin center</span></span>](https://docs.microsoft.com/MicrosoftTeams/manage-apps)
- [<span data-ttu-id="883ed-130">Gestire i criteri di configurazione dell'app in Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="883ed-130">Manage app setup policies in Microsoft Teams</span></span>](https://docs.microsoft.com/microsoftteams/teams-app-setup-policies)

## <a name="in-prodshort"></a><span data-ttu-id="883ed-131">In [!INCLUDE [prodshort](includes/prodshort.md)]</span><span class="sxs-lookup"><span data-stu-id="883ed-131">In [!INCLUDE [prodshort](includes/prodshort.md)]</span></span>

### <a name="minimum-requirements"></a><span data-ttu-id="883ed-132">Requisiti minimi</span><span class="sxs-lookup"><span data-stu-id="883ed-132">Minimum requirements</span></span>

- <span data-ttu-id="883ed-133">Versione di [!INCLUDE [prodshort](includes/prodshort.md)]:</span><span class="sxs-lookup"><span data-stu-id="883ed-133">[!INCLUDE [prodshort](includes/prodshort.md)] version:</span></span>

    <span data-ttu-id="883ed-134">Secondo ciclo di rilascio del 2020 (versione 17) di [!INCLUDE [prodshort](includes/prodshort.md)] o successiva.</span><span class="sxs-lookup"><span data-stu-id="883ed-134">[!INCLUDE [prodshort](includes/prodshort.md)] 2020 release wave 2 (version 17) or later.</span></span> <span data-ttu-id="883ed-135">L'integrazione di Teams è supportata solo per [!INCLUDE [prodshort](includes/prodshort.md)] online, non in locale.</span><span class="sxs-lookup"><span data-stu-id="883ed-135">Teams integration is only supported for [!INCLUDE [prodshort](includes/prodshort.md)] online; not on-premises.</span></span>

- <span data-ttu-id="883ed-136">La codeunit **2718 Provider di riepilogo pagine** è pubblicata come servizio Web:</span><span class="sxs-lookup"><span data-stu-id="883ed-136">Codeunit **2718 Page Summary Provider** is published as a web service:</span></span>

    <span data-ttu-id="883ed-137">Questa codeunit viene pubblicata come servizio Web per impostazione predefinita.</span><span class="sxs-lookup"><span data-stu-id="883ed-137">This codeunit is published as a web service by default.</span></span> <span data-ttu-id="883ed-138">La codeunit fa parte dell'applicazione di sistema [!INCLUDE [prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="883ed-138">The codeunit is part of the [!INCLUDE [prodshort](includes/prodshort.md)] system application.</span></span> <span data-ttu-id="883ed-139">Viene utilizzata per ottenere i dati del campo per una pagina [!INCLUDE [prodshort](includes/prodshort.md)] aggiunta a una conversazione di Teams.</span><span class="sxs-lookup"><span data-stu-id="883ed-139">It's used to get the field data for a [!INCLUDE [prodshort](includes/prodshort.md)] page added to a Teams conversation.</span></span> 

- <span data-ttu-id="883ed-140">Autorizzazioni utente:</span><span class="sxs-lookup"><span data-stu-id="883ed-140">User permissions:</span></span>

    <span data-ttu-id="883ed-141">Per la maggior parte, le pagine e i dati che gli utenti possono visualizzare e modificare in una conversazione di Teams sono controllati dalle autorizzazioni in [!INCLUDE [prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="883ed-141">For the most part, the pages and data that users can view and edit in a Teams conversation is controlled by their permissions in [!INCLUDE [prodshort](includes/prodshort.md)].</span></span>
    
    - <span data-ttu-id="883ed-142">Per incollare un collegamento [!INCLUDE [prodshort](includes/prodshort.md)] in una conversazione di Teams e farlo espandere in una scheda, gli utenti devono disporre almeno dell'autorizzazione di lettura sulla pagina e sui relativi dati.</span><span class="sxs-lookup"><span data-stu-id="883ed-142">To paste a [!INCLUDE [prodshort](includes/prodshort.md)] link into a Teams conversation and have it expand into a card, users must have at least read permission on the page and its data.</span></span>
    - <span data-ttu-id="883ed-143">Una volta che una scheda è stata inviata a una conversazione, qualsiasi utente in quella conversazione può visualizzare quella scheda senza autorizzazione per Business Central.</span><span class="sxs-lookup"><span data-stu-id="883ed-143">Once a card is submitted into a conversation, any user in that conversation can view that card without permission to Business Central.</span></span>
    - <span data-ttu-id="883ed-144">Per visualizzare ulteriori dettagli per una scheda o aprire il record in [!INCLUDE [prodshort](includes/prodshort.md)], gli utenti devono disporre dell'autorizzazione di lettura sulla pagina e sui suoi dati.</span><span class="sxs-lookup"><span data-stu-id="883ed-144">To view more details for a card or open the record in [!INCLUDE [prodshort](includes/prodshort.md)], users must have read permission on the page and its data.</span></span>
    - <span data-ttu-id="883ed-145">Per modificare i dati, l'utente deve disporre delle autorizzazioni per la modifica.</span><span class="sxs-lookup"><span data-stu-id="883ed-145">To change data, user's need modify permissions.</span></span>
    
    <span data-ttu-id="883ed-146">Per informazioni sulle autorizzazioni, vedere [Assegnare autorizzazioni a utenti e gruppi](ui-define-granular-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="883ed-146">For information about permissions, see [Assign Permissions to Users and Groups](ui-define-granular-permissions.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="883ed-147">Vedere anche</span><span class="sxs-lookup"><span data-stu-id="883ed-147">See Also</span></span>
[<span data-ttu-id="883ed-148">Panoramica dell'integrazione di Business Central e Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="883ed-148">Business Central and Microsoft Teams Integration Overview</span></span>](across-teams-overview.md)  
<span data-ttu-id="883ed-149">[Installare l'app [!INCLUDE [prodshort](includes/prodshort.md)] per Microsoft Teams](across-install-app-for-teams.md)</span><span class="sxs-lookup"><span data-stu-id="883ed-149">[Install the [!INCLUDE [prodshort](includes/prodshort.md)] App for Microsoft Teams](across-install-app-for-teams.md)</span></span>  
[<span data-ttu-id="883ed-150">Sviluppo per l'integrazione di Teams</span><span class="sxs-lookup"><span data-stu-id="883ed-150">Developing for Teams Integration</span></span>](/dynamics365/business-central/dev-itpro/developer/devenv-develop-for-teams)  
[<span data-ttu-id="883ed-151">Introduzione</span><span class="sxs-lookup"><span data-stu-id="883ed-151">Getting Started</span></span>](product-get-started.md)  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  
