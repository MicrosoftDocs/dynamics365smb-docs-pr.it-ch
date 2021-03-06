---
title: Domande frequenti su Teams
description: Ottenere risposte ad alcune domande tipiche sull'utilizzo di Teams e Business Central.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Teams, MS Teams, Microsoft Teams, Skype, Link, Microsoft 365, collaborate, collaboration, teamwork, faq, errors
ms.date: 05/19/2021
ms.author: jswymer
ms.openlocfilehash: f3c9626fa73247b2109e5f179aef405e80b44b07
ms.sourcegitcommit: 5a916b0aa0a2eef0c22b5722a0af041757e6d7c2
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 05/19/2021
ms.locfileid: "6074658"
---
# <a name="teams-faq"></a>Domande frequenti su Teams

[!INCLUDE [online_only](includes/online_only.md)]

Questo articolo contiene le risposte ad alcune domande sull'utilizzo di Teams e [!INCLUDE [prod_short](includes/prod_short.md)].

## <a name="general"></a>[Generale](#tab/general)

### <a name="how-do-i-sign-in-to-the-prod_shortmd-app-in-teams"></a>Come si accede all'app [!INCLUDE [prod_short.md](includes/prod_short.md)] in Teams?

Dopo aver installato l'app, ti verrà chiesto di accedere la prima volta che usi l'app, quando incolli un collegamento [!INCLUDE [prod_short.md](includes/prod_short.md)] nella chat di Teams o quando scegli l'azione **Dettagli** in una scheda di Teams. A seconda del client Teams, potrebbe essere necessario immettere le credenziali utilizzate per l'accesso a [!INCLUDE [prod_short.md](includes/prod_short.md)].

### <a name="how-do-i-sign-out-of-the-prod_shortmd-app-in-teams"></a>Come ci si disconnette dall'app [!INCLUDE [prod_short.md](includes/prod_short.md)] in Teams?

Per disconnettersi dall'identità utente corrente in Teams usata per connetterti a [!INCLUDE [prod_short.md](includes/prod_short.md)], vai a qualsiasi casella di composizione della chat, fai clic con il pulsante destro sull'icona [!INCLUDE [prod_short.md](includes/prod_short.md)] sotto la casella, quindi scegli **Impostazioni**. Quando viene visualizzata la finestra, controlla la tua identità attualmente collegata e quindi scegli **Disconnetti**.

### <a name="does-the-app-for-teams-connect-to-prod_shortmd-on-premises"></a>L'app per Teams si connette a [!INCLUDE [prod_short.md](includes/prod_short.md)] in locale? 

No. L'app [!INCLUDE [prod_short.md](includes/prod_short.md)] per Teams funziona solo con [!INCLUDE [prod_short.md](includes/prod_short.md)] Online. Non ci sono piani per supportare i tipi di distribuzione di [!INCLUDE [prod_short.md](includes/prod_short.md)], come locale, cloud ibrido o cloud privato, che Microsoft non ospita o gestisce direttamente.

### <a name="does-the-app-work-with-multiple-companies-and-environments"></a>L'app è utilizzabile con più società e ambienti? 

Sì. Per cercare contatti in un'altra azienda, vai a [Impostazioni](across-teams-settings.md). Quando l'app [!INCLUDE [prod_short.md](includes/prod_short.md)] espande un collegamento in una scheda, il collegamento deve contenere il nome dell'ambiente e dell'azienda affinché l'app corrisponda al record nella società appropriata. Puoi incollare collegamenti a qualsiasi società e ambiente a cui hai accesso nella tua organizzazione e dall'account [!INCLUDE [prod_short.md](includes/prod_short.md)] che hai utilizzato per accedere. I partecipanti alla chat vedranno la scheda. Ma non possono visualizzare i dettagli della scheda a meno che non dispongano delle autorizzazioni per la società o l'ambiente in cui è archiviato il record.

### <a name="in-which-countries-or-regions-is-the-prod_shortmd-app-available"></a>In quali paesi o regioni è disponibile l'app [!INCLUDE [prod_short.md](includes/prod_short.md)]? 

L'app [!INCLUDE [prod_short.md](includes/prod_short.md)] per Teams non è limitata per paese o area geografica. L'app è disponibile in tutti i mercati attualmente supportati dal marketplace di Teams. 

### <a name="does-the-prod_shortmd-app-work-with-any-localization-of-prod_shortmd"></a>L'app [!INCLUDE [prod_short.md](includes/prod_short.md)] è utilizzabile con qualsiasi localizzazione di [!INCLUDE [prod_short.md](includes/prod_short.md)]? 

Sì. L'app è progettata per funzionare con qualsiasi localizzazione di [!INCLUDE [prod_short.md](includes/prod_short.md)], indipendentemente dal fatto che la localizzazione sia offerta direttamente da Microsoft o tramite un partner. Per ulteriori informazioni vedere [Disponibilità nazionale/regionale e lingue supportate](/dynamics365/business-central/dev-itpro/compliance/apptest-countries-and-translations?toc=/dynamics365/business-central/toc.json).

### <a name="which-languages-does-the-prod_shortmd-app-support"></a><a name="language"></a>Quali lingue sono supportate dall'app [!INCLUDE [prod_short.md](includes/prod_short.md)]?

Due cose determinano la lingua utilizzata per le schede e i dettagli delle schede in Teams:

1. La lingua in Teams, visibile nelle impostazioni dell'account in Teams. 
2. La lingua in [!INCLUDE [prod_short.md](includes/prod_short.md)], visibile nel client Web di [!INCLUDE [prod_short.md](includes/prod_short.md)] (vedi [Modificare l'impostazione di base - Lingua](ui-change-basic-settings.md#language)).

Nella tabella seguente viene descritto come l'esperienza differisce per autori e destinatari dei messaggi, a seconda delle impostazioni della lingua e della disponibilità delle lingue.

|Chi|Scheda|Dettagli scheda |
|-|----|--------------| 
|Autore messaggio |Visualizzata nella lingua specificata in Teams. Se [!INCLUDE [prod_short.md](includes/prod_short.md)] non offre la stessa lingua, la scheda è visualizzata in inglese. |Visualizzata nella lingua specificata in [!INCLUDE [prod_short.md](includes/prod_short.md)],  che può includere le lingue di app di lingua fornite dai partner. |
|Destinatario messaggio |Visualizzata nella lingua dell'autore del messaggio. |Visualizzata nella lingua specificata in [!INCLUDE [prod_short.md](includes/prod_short.md)], |

Per l'elenco delle lingue supportate per [!INCLUDE [prod_short.md](includes/prod_short.md)], vedi [Lingue supportate](/dynamics365/business-central/dev-itpro/compliance/apptest-countries-and-translations?toc=/dynamics365/business-central/toc.json#supported-languages).

### <a name="does-the-prod_shortmd-app-work-with-industry-solutions"></a>L'app [!INCLUDE [prod_short.md](includes/prod_short.md)] funziona con le soluzioni del settore?

Sì. Ma solo alcune funzionalità dell'app funzionano con [app Embed](/dynamics365/business-central/dev-itpro/deployment/embed-app-overview):

- L'app funziona con collegamenti basati sul modello **\*.bc.dynamics.com** tipicamente utilizzato con app Embed.
- La Ricerca Contatti non è disponibile per le app Embed che sostituiscono l'applicazione di base di Microsoft.

### <a name="where-can-i-find-teams-integration-inside-the-prod_shortmd-web-client"></a>Dove posso trovare l'integrazione di Teams nel client Web di [!INCLUDE [prod_short.md](includes/prod_short.md)]? 

Al momento non è disponibile l'incorporamento di controlli Teams o la presenza di funzionalità di Teams nel client Web di [!INCLUDE [prod_short.md](includes/prod_short.md)] o in altri client.

### <a name="does-prod_shortmd-work-with-the-teams-mobile-app"></a>[!INCLUDE [prod_short.md](includes/prod_short.md)] è utilizzabile con l'app per dispositivi mobili Teams?

Sì. L'app [!INCLUDE [prod_short.md](includes/prod_short.md)] può essere installata dall'app desktop o dal browser di Teams o da un amministratore per tutti gli utenti. Una volta installata, l'app [!INCLUDE [prod_short.md](includes/prod_short.md)] è automaticamente disponibile in Teams per iOS e Android. Nei dispositivi mobili, puoi visualizzare solo le schede inviate da altri, accedere ai dettagli o visualizzare la scheda per un'esperienza completa nell'app per dispositivi mobili [!INCLUDE [prod_short.md](includes/prod_short.md)]. Non puoi incollare collegamenti che si espandono nelle schede durante la composizione dei messaggi o la ricerca dei contatti. Per i requisiti minimi per i dispositivi mobili, vedi [Requisiti minimi per l'utilizzo di Business Central](product-requirements.md).

### <a name="is-the-prod_shortmd-app-for-teams-the-same-as-the-prod_shortmd-app-for-ios-and-android"></a>L'app [!INCLUDE [prod_short.md](includes/prod_short.md)] per Teams è uguale all'app [!INCLUDE [prod_short.md](includes/prod_short.md)] per iOS e Android?

No. L'app per Teams è un componente aggiuntivo di Microsoft Teams ed è progettata esclusivamente per esperienze collaborative in Teams. Inoltre, l'app per dispositivi mobili [!INCLUDE [prod_short.md](includes/prod_short.md)] offre un'esperienza completa per l'utilizzo dei dati di [!INCLUDE [prod_short.md](includes/prod_short.md)] nei dispositivi mobili.

Gli utenti di dispositivi mobili sono incoraggiati a installare sia l'app per dispositivi mobili che l'app per Teams per usufruire di tutti i vantaggi inerenti all'utilizzo di [!INCLUDE [prod_short.md](includes/prod_short.md)]. Con entrambe le app installate, puoi scegliere l'azione **Apri nuova finestra** in una scheda di Teams per aprire i dettagli della scheda nell'app per dispositivi mobili [!INCLUDE [prod_short.md](includes/prod_short.md)]. Per informazioni sull'installazione di [!INCLUDE [prod_short.md](includes/prod_short.md)] e sull'app per dispositivi mobili Teams, vedi:

- [Installare Business Central sul dispositivo mobile](install-mobile-app.md)
- [Scaricare l'app per dispositivi mobili per Teams](https://support.microsoft.com/office/download-the-mobile-app-for-teams-5940ebdc-0082-4fb1-83c4-751edc23dcb5)

### <a name="does-the-prod_shortmd-app-work-in-all-teams-clients"></a>L'app [!INCLUDE [prod_short.md](includes/prod_short.md)] è utilizzabile in tutti i client Teams?

No. L'app [!INCLUDE [prod_short.md](includes/prod_short.md)] per Teams non è supportata se installata come pacchetto per macOS o Linux. Su queste piattaforme puoi invece accedere a Teams usando un browser supportato.

Per i requisiti minimi in [!INCLUDE [prod_short.md](includes/prod_short.md)], vedi [Requisiti minimi per l'utilizzo di Business Central](product-requirements.md#teams).

Per informazioni sulla scelta dei client Teams e su come installarli, vedi [Installare client per Microsoft Teams](/microsoftteams/get-clients) nella documentazione di Teams.

### <a name="which-teams-client-is-best-for-prod_shortmd"></a>Qual è il migliore client Teams per [!INCLUDE [prod_short.md](includes/prod_short.md)]?

Esistono solo piccole differenze e limitazioni tra i client Teams che possono influire sull'esperienza con l'app [!INCLUDE [prod_short.md](includes/prod_short.md)] per Teams. Quando scegli un client Teams, considera quanto segue:

- Non è possibile accedere alla fotocamera e alla posizione dalla finestra dei dettagli nell'app desktop Teams.
- I numeri di telefono non possono essere attivati dalla finestra dei dettagli in Teams per iOS, Teams per Android o Teams nel browser.
- L'utilizzo di Microsoft Edge con Teams nel browser ti consente di lavorare facilmente in più identità e account accedendo a Teams da diversi profili. Per informazioni sull'utilizzo dei profili in Microsoft Edge, vedi [Accedere e crea più profili in Microsoft Edge](https://support.microsoft.com/office/sign-in-and-create-multiple-profiles-in-microsoft-edge-df94e622-2061-49ae-ad1d-6f0e43ce6435).

### <a name="what-is-the-best-way-for-me-to-demonstrate-prod_shortmd-and-microsoft-teams-to-prospective-customers"></a>Qual è il modo migliore di presentare [!INCLUDE [prod_short.md](includes/prod_short.md)] e Microsoft Teams a potenziali clienti?

Se si è un partner rivenditore, è possibile che si intenda disporre di un ambiente da mostrare ai potenziali clienti nell'ambito di presentazioni prima della vendita. Per non influire sul funzionamento di Microsoft Teams nell'organizzazione, puoi ottenere un account demo di Microsoft 365 all'indirizzo [https://aka.ms/CDX](https://aka.ms/CDX). Questo account ti offre il controllo completo di un'organizzazione Azure indipendente che include Microsoft Teams e [!INCLUDE [prod_short.md](includes/prod_short.md)]. Per ulteriori informazioni, vedi [Preparazione degli ambienti dimostrativi di Dynamics 365 Business Central](/dynamics365/business-central/dev-itpro/administration/demo-environment).

### <a name="does-the-prod_shortmd-app-for-teams-cater-for-my-customization-and-personalization"></a>L'app [!INCLUDE [prod_short.md](includes/prod_short.md)] per Teams consente la personalizzazione?

L'app [!INCLUDE [prod_short.md](includes/prod_short.md)] per Teams può visualizzare schede per collegamenti a pagine e tabelle dei clienti in [!INCLUDE [prod_short.md](includes/prod_short.md)], come le pagine e tabelle originate dalle estensioni personalizzate o da AppSource.

I campi visualizzati in una scheda di Teams possono essere modificati dalle personalizzazioni di [!INCLUDE [prod_short.md](includes/prod_short.md)] installate per l'organizzazione. Le schede non considerano alcuna personalizzazione specifica del ruolo o personalizzazione dell'utente. Tuttavia, la finestra dei dettagli di una scheda mostra i dettagli dei record come visualizzati in [!INCLUDE [prod_short.md](includes/prod_short.md)], comprese eventuali estensioni, personalizzazioni dei ruoli e personalizzazione dell'utente.

Quando si cercano contatti, i campi corrispondenti nella tabella **Contatti** e i campi visualizzati nei risultati della ricerca non sono interessati da alcuna personalizzazione.

### <a name="how-do-the-permissions-required-by-the-app-affect-my-privacy"></a>In che modo le autorizzazioni richieste dall'app influiscono sulla privacy?

Prima di installare l'app [!INCLUDE [prod_short.md](includes/prod_short.md)] per Teams, è possibile rivedere le autorizzazioni minime necessarie per il funzionamento dell'app. Installando l'app, si accetta che l'app disponga dell'autorizzazione per ricevere messaggi e dati forniti e che Teams disponga dell'autorizzazione per archiviare ed elaborare tali messaggi.

Alcune funzionalità di [!INCLUDE [prod_short.md](includes/prod_short.md)] richiedono inoltre l'apertura di collegamenti esterni o l'accesso alla fotocamera o alla posizione geografica. Si supponga ad esempio di voler acquisire una foto di una fattura di acquisto per l'elaborazione. L'app [!INCLUDE [prod_short.md](includes/prod_short.md)] non utilizza queste funzioni senza il consenso dell'utente. L'utilizzo avviene inoltre solo tramite funzionalità specifiche nella finestra **Dettagli**. Quando si utilizza una di queste funzionalità per la prima volta, Teams visualizzerà una finestra di dialogo in cui è richiesto di concedere l'accesso alle funzionalità del dispositivo richieste.

- Nel desktop di Teams rivedere e modificare le autorizzazioni dell'app dalla finestra **Impostazioni**. Selezionare la propria immagine del profilo nella parte superiore dell'app, selezionare **Impostazioni** > **Autorizzazioni**, quindi l'app [!INCLUDE [prod_short.md](includes/prod_short.md)].

- Per Teams nel browser e Teams per iOS o Android, è possibile rivedere o modificare le autorizzazioni tramite le impostazioni del browser o del dispositivo.

> [!NOTE]
> Le funzionalità esatte di [!INCLUDE [prod_short.md](includes/prod_short.md)] che richiedono le autorizzazioni variano in base alle app aggiuntive e alle personalizzazioni applicate all'ambiente di [!INCLUDE [prod_short.md](includes/prod_short.md)] a cui ci si collega.

### <a name="where-can-i-learn-about-my-privacy"></a>Dove posso ottenere informazioni sulla privacy? 

Puoi ottenere informazioni su come Microsoft gestisce i tuoi dati nell'[Informativa sulla privacy di Microsoft](https://go.microsoft.com/fwlink/?linkid=2030602). 

Contatta il tuo amministratore per informazioni su come la tua organizzazione gestisce la privacy dei tuoi dati.

### <a name="how-do-i-uninstall-the-prod_shortmd-app-for-teams"></a>Come si disinstalla l'app [!INCLUDE [prod_short.md](includes/prod_short.md)] per Teams?

Per rimuovere l'app installata, vai a qualsiasi casella di composizione della chat, trova l'icona [!INCLUDE [prod_short.md](includes/prod_short.md)] sotto la casella, fai clic con il pulsante destro del mouse sull'icona e scegli **Disinstalla**.  

### <a name="will-microsoft-continue-to-improve-the-prod_shortmd-app-for-teams"></a>Microsoft continuerà a migliorare l'app [!INCLUDE [prod_short.md](includes/prod_short.md)] per Teams?

In Microsoft, i feedback della nostra variegata comunità di utenti vengono costantemente monitorati e si agisce in base ai migliori suggerimenti. Per informazioni sui miglioramenti futuri dell'app [!INCLUDE [prod_short.md](includes/prod_short.md)] per Teams, vedi il [Piano di rilascio di Dynamics 365](/dynamics365-release-plan/2021wave1/).

Se desideri partecipare al miglioramento dell'app per Teams o hai un'idea che ti permetterebbe di semplificare il tuo lavoro o le tue esperienze collaborative in Teams, aggiungila o vota per quelle esistenti in [https://aka.ms/BusinessCentralIdeas](https://aka.ms/BusinessCentralIdeas).

## <a name="searching-for-contacts"></a>[Ricerca di contatti](#tab/contacts)

### <a name="which-tables-does-the-app-search-in"></a>In quali tabelle l'app esegue la ricerca?

Durante la ricerca dei contatti dall'app [!INCLUDE [prod_short.md](includes/prod_short.md)] per Teams, i termini di ricerca vengono confrontati con i record nella tabella **Contatti** in [!INCLUDE [prod_short.md](includes/prod_short.md)]. 

### <a name="which-fields-in-the-contacts-table-can-i-search"></a>In quali campi della tabella dei contatti posso eseguire la ricerca?

Mentre digiti i termini di ricerca nella casella di ricerca, i termini vengono confrontati con la maggior parte dei campi nella tabella **Contatti**. I campi includono, ad esempio, i campi **N.**, **Nome**, **Indirizzo**, **Nr. di telefono** oppure **Numero di telefono cellulare** e **E-mail**. 

I termini di ricerca non vengono abbinati a nessun campo personalizzato aggiunto alla tabella **Contatti** per app ed estensioni.

### <a name="do-search-results-include-companies-and-persons"></a>I risultati della ricerca includono aziende e persone?

Sì. In [!INCLUDE [prod_short.md](includes/prod_short.md)], i contatti possono essere di tipo **Azienda** o digita **Persona**, dove una o più persone possono essere associate a un'azienda. Nei risultati della ricerca, le aziende e le persone hanno icone diverse.

### <a name="do-contacts-of-any-business-relationship-appear-in-the-results"></a>I contatti di una relazione d'affari compaiono nei risultati?

Sì. Alcuni contatti possono rappresentare clienti o fornitori o entrambi. Gli altri contatti senza una relazione d'affari definita in genere rappresentano i potenziali clienti. Contatti con altre relazioni d'affari, comprese le relazioni personalizzate che hai configurato in [!INCLUDE [prod_short.md](includes/prod_short.md)], verrà visualizzato anche nei risultati della ricerca.

### <a name="can-i-look-up-contact-details-during-meetings"></a>Posso cercare i dettagli di contatto durante le riunioni?

Sì. Puoi cercare le informazioni di contatto, la cronologia delle interazioni e i documenti correlati per il cliente o il fornitore durante una riunione o una chiamata di Teams nella riunione senza uscire da Teams.

In effetti, puoi cercare i dettagli di contatto da qualsiasi punto in Teams usando la casella di comando. Puoi, ad esempio, cercare i dettagli di contatto dal calendario di Teams per aiutarti a configurare le riunioni.

### <a name="how-do-i-view-my-last-interactions-with-a-contact"></a>Come posso visualizzare le mie ultime interazioni con un contatto?

La finestra dei dettagli di un contatto visualizza i movimenti del log delle interazioni. I movimenti del log delle interazioni forniscono la cronologia delle interazioni che l'organizzazione ha avuto con il contatto specifico. Le interazioni possono includere e-mail che hai scambiato, chiamate che hai ricevuto o documenti che hai inviato.

Per visualizzare le interazioni, [!INCLUDE [prod_short.md](includes/prod_short.md)] deve essere configurato per monitorare le interazioni. Per ulteriori informazioni sulla registrazione delle interazioni, vedi [Registra le interazioni con i contatti](marketing-interactions.md).

### <a name="how-do-i-register-a-teams-call-or-meeting-as-an-interaction"></a>Come si registra una chiamata o una riunione di Teams come interazione?

Nella finestra dei dettagli di un contatto, trova l'azione **Crea interazione** e sceglie tra le chiamate in entrata o in uscita come modelli di interazione. Puoi anche creare i tuoi modelli di interazione personalizzati specificamente per l'uso con le conversazioni di Teams.

### <a name="can-i-call-a-contact-from-the-prod_shortmd-app-for-teams"></a>Posso chiamare un contatto dall'app [!INCLUDE [prod_short.md](includes/prod_short.md)] per Teams?

[!INCLUDE [prod_short.md](includes/prod_short.md)] ha un'integrazione limitata alle funzionalità di chiamata di Teams. Non è possibile avviare immediatamente una chiamata VOIP dalla scheda del contatto o dalla finestra dei dettagli del contatto. Tuttavia, quando si visualizzano i dettagli del contatto nell'app desktop Teams, puoi selezionare il campo del numero di telefono per comporre quel numero se Teams è configurato come app di composizione predefinita sul dispositivo. Per comporre numeri di telefono fisso o mobile tramite PSTN, il sistema telefonico tradizionale, Teams richiede l'app Microsoft 365 Business Voice. Per saperne di più, vedi [Cos'è Microsoft 365 Business Voice?](/MicrosoftTeams/business-voice/whats-business-voice).

### <a name="how-do-i-view-recent-documents-for-a-customer-or-vendor"></a>Come si visualizzano i documenti recenti per un cliente o un fornitore?

[!INCLUDE [prod_short.md](includes/prod_short.md)] in genere si riferisce a un contatto con un record cliente o fornitore che a sua volta è correlato ai record delle transazioni commerciali, come offerte di vendita o fatture di acquisto. Per visualizzare i documenti correlati per un contatto, vai alla finestra dei dettagli del contatto, scegli il valore del campo **Relazione d'affari** o utilizza le azioni per passare al cliente o fornitore associato. Nella pagina del cliente o del fornitore, espandi il riquadro FactBox per visualizzare le statistiche per vari documenti in cui è possibile eseguire il drill-down. La tua esperienza potrebbe differire in base alle tue personalizzazioni.

### <a name="how-do-i-search-for-contacts-using-special-characters"></a>Come cerco i contatti che usano caratteri speciali?

Puoi immettere criteri di ricerca utilizzando quasi tutti i caratteri Unicode. Tuttavia, [!INCLUDE [prod_short.md](includes/prod_short.md)] riserva i seguenti simboli per altri usi: **=**, **.**, **\**_ e _*@**. L'utilizzo di questi simboli nei termini di ricerca potrebbe non restituire i risultati previsti. Se non vedi i risultati attesi, racchiudi i simboli nei termini di ricerca tra virgolette singole, ad esempio, **Contoso'='2**.

### <a name="how-can-i-search-contacts-stored-in-a-different-company"></a>Come posso cercare i contatti archiviati in un'altra azienda?

L'app [!INCLUDE [prod_short.md](includes/prod_short.md)] per Teams può cercare clienti, fornitori e altri contatti in una società alla volta.  
Per cercare i contatti archiviati in un altra azienda [!INCLUDE [prod_short.md](includes/prod_short.md)], apri [Impostazioni](across-teams-settings.md), quindi cambia l'ambiente e l'azienda da lì.

### <a name="are-prod_shortmd-contacts-different-than-the-ones-in-the-teams-contacts-screen"></a>I contatti [!INCLUDE [prod_short.md](includes/prod_short.md)] sono diversi da quelli nella schermata dei contatti di Teams?

Sì. I contatti archiviati in [!INCLUDE [prod_short.md](includes/prod_short.md)] rappresentano i contatti commerciali disponibili per la tua organizzazione. Sono contatti con i quali hai una relazione d'affari consolidata e ben definita, oppure contatti che rappresentano potenziali clienti. Questi contatti sono in genere contatti esterni. Al contrario, i contatti visualizzati nell'elenco dei contatti di chiamata di Teams sono i tuoi contatti. Questi contatti non sono necessariamente condivisi con altri nella tua organizzazione e in genere rappresentano i contatti interni alla tua organizzazione.

### <a name="does-prod_shortmd-synchronize-contacts-with-teams"></a>[!INCLUDE [prod_short.md](includes/prod_short.md)] sincronizza i contatti con Teams?

No. I contatti archiviati in [!INCLUDE [prod_short.md](includes/prod_short.md)] rimangono separati dai contatti archiviati in Teams.
Al momento non ci sono piani per sincronizzare i due elenchi insieme.

### <a name="what-is-the-minimum-version-of-prod_shortmd-for-contact-search"></a>Qual è la versione minima di [!INCLUDE [prod_short.md](includes/prod_short.md)] per la ricerca di contatti?

La ricerca dei contatti richiede che tu abbia l'app [!INCLUDE [prod_short.md](includes/prod_short.md)] per Teams versione 1.0.4 o successiva installata e ti stai connettendo agli ambienti [!INCLUDE [prod_short.md](includes/prod_short.md)] della versione 18 o successiva.

### <a name="can-i-search-from-my-mobile-device"></a>Posso eseguire ricerche dal mio dispositivo mobile?

In questo momento la ricerca dei contatti non è disponibile da Teams per iOS e Teams per Android.

### <a name="which-permissions-do-i-need-for-contact-search"></a>Di quali autorizzazioni ho bisogno per la ricerca dei contatti?

Per cercare contatti, è necessaria l'autorizzazione a livello di oggetto per la tabella **Contatti** all'interno dell'azienda [!INCLUDE [prod_short.md](includes/prod_short.md)] in cui si esegue la ricerca. Per visualizzare la finestra dei dettagli di un contatto, è necessaria almeno l'autorizzazione di lettura per la pagina **Contatti** all'interno dell'azienda [!INCLUDE [prod_short.md](includes/prod_short.md)] e qualsiasi altro oggetto correlato.

### <a name="can-i-use-contact-search-if-im-a-delegated-admin"></a>Posso utilizzare la ricerca dei contatti se sono un amministratore delegato?

Sì. Puoi anche cercare contatti e dettagli dei contatti se disponi di un ruolo di amministratore delegato in un'organizzazione.

### <a name="is-contact-search-affected-by-api-limits"></a>La ricerca dei contatti è interessata dai limiti dell'API?

Sì. La ricerca di contatti da Teams si basa sull'API [!INCLUDE [prod_short.md](includes/prod_short.md)] v2.0 ed è soggetta a eventuali limiti API che gestiscono l'utilizzo. Puoi scoprire di più sui limiti nella sezione [Limiti API attuali](/dynamics-nav/api-reference/v2.0/dynamics-current-limits).

### <a name="why-does-it-sometimes-ask-me-to-set-up-the-app"></a>Perché a volte mi chiede di configurare l'app?

Dopo aver effettuato l'accesso all'app [!INCLUDE [prod_short.md](includes/prod_short.md)] per Teams per la prima volta, l'app tenterà di determinare la tua azienda preferita in [!INCLUDE [prod_short.md](includes/prod_short.md)]. Se l'app non è in grado di determinare l'azienda, potresti dover andare a **Impostazioni** e scegliere l'azienda in cui desideri effettuare la ricerca. Questa situazione si verifica, ad esempio, se hai accesso a più società in tutti gli ambienti della tua organizzazione. In questo caso, dovrai scegliere un'azienda prima di poter iniziare la ricerca.  

L'app potrebbe anche richiedere di andare a **Impostazioni** se non si dispone di una sottoscrizione [!INCLUDE [prod_short.md](includes/prod_short.md)], non sono disponibili ambienti [!INCLUDE [prod_short.md](includes/prod_short.md)] o l'account non dispone di una licenza [!INCLUDE [prod_short.md](includes/prod_short.md)].

### <a name="id-like-to-search-for-items-or-records-from-other-tables-can-i-do-this-from-teams"></a>Vorrei eseguire la ricerca di elementi o record da altre tabelle. Posso farlo da Teams?

La ricerca nelle altre tabelle non è possibile in questo momento. L'app [!INCLUDE [prod_short.md](includes/prod_short.md)] per Teams esegue solo la ricerca nell'elenco dei contatti [!INCLUDE [prod_short.md](includes/prod_short.md)], che può includere fornitori, clienti e altri contatti.

Se desideri vedere le funzionalità di ricerca evolversi per includere altre tabelle, incoraggiamo la nostra comunità ad aggiungere un'idea o votare per idee esistenti su https://aka.ms/BusinessCentralIdeas.

## <a name="working-with-cards"></a>[Utilizzo delle schede](#tab/cards)

### <a name="which-types-of-links-does-the-app-support"></a>Quali tipi di collegamento supporta l'app?

L'app [!INCLUDE [prod_short.md](includes/prod_short.md)] per Teams reagisce alla maggior parte dei collegamenti del client Web di [!INCLUDE [prod_short.md](includes/prod_short.md)]. Quando il collegamento fa riferimento a un singolo record in una pagina, la scheda visualizzerà i campi per quel record. I tipi di pagina supportati includono: 

- Pagine scheda, come la scheda Articolo
- Pagine documento, come il documento Ordine vendita
- Pagine ListPlus che rappresentano un singolo record composto da altri record, ad esempio Riconciliazione estratti conto
- Pagine elenco semplici in cui un record non offre la possibilità di eseguire il drill-down in una pagina di dettagli separata, come l'elenco dei codici postali

Quando si incolla un collegamento all'URL del client Web principale, ad esempio https://businesscentral.dynamics.com, la scheda visualizza invece informazioni per consentire ai nuovi utenti di accedere a [!INCLUDE [prod_short.md](includes/prod_short.md)].

### <a name="how-do-i-delete-a-card-i-sent-to-a-chat"></a>Come elimino una scheda che ho inviato a una chat?

Non puoi eliminare una scheda che hai già inviato alla chat. Puoi tuttavia eliminare l'intero messaggio di cui fa parte la scheda.

In qualità di autore del messaggio, puoi eliminare tutti i messaggi inviati alle chat con una persona, un gruppo o un canale, a meno che l'amministratore non abbia impostato criteri che impediscono l'eliminazione dei messaggi. Se moderi un canale come proprietario del canale, il tuo amministratore potrebbe anche averti concesso l'autorizzazione di eliminare tutti i messaggi nel canale, inclusi i messaggi inviati da altri utenti.

L'eliminazione di un messaggio che contiene una scheda non elimina né modifica i dati in [!INCLUDE [prod_short.md](includes/prod_short.md)].

### <a name="do-cards-always-show-up-to-date-information"></a>Le schede mostrano sempre informazioni aggiornate?

No. I valori dei campi in una scheda di Teams, incluse le immagini, sono basati sui dati disponibili al momento dell'invio della scheda alla chat. Le schede di [!INCLUDE [prod_short.md](includes/prod_short.md)] non vengono aggiornate automaticamente in Teams. 

### <a name="will-others-see-my-card-if-they-dont-have-the-prod_shortmd-app-for-teams"></a>Gli altri utenti vedranno la mia scheda se non hanno l'app [!INCLUDE [prod_short.md](includes/prod_short.md)] per Teams? 

Quando scrivi e invii un messaggio in chat che include una scheda, tutti gli utenti vedranno la scheda&mdash;anche se non hanno installato l'app [!INCLUDE [prod_short.md](includes/prod_short.md)] per Teams.

### <a name="how-do-i-find-out-which-company-a-card-in-teams-belongs-to"></a>Come faccio a sapere a quale società appartiene una scheda in Teams?

Se si lavora per più aziende [!INCLUDE [prod_short.md](includes/prod_short.md)], chiedere all'amministratore di abilitare un badge per ogni società. Se abilitato, questo interessante suggerimento viene visualizzato in qualsiasi finestra dei dettagli all'interno di Teams e mostra la società e l'ambiente a cui appartiene il record. Per informazioni su come impostare il badge società, vedere [Per visualizzare un badge società per un rapido accesso alle informazioni della società](ui-change-basic-settings.md#badge).

## <a name="working-with-card-details"></a>[Utilizzo dei dettagli della scheda](#tab/carddetails)

### <a name="where-is-the-save-button-in-the-details-window-in-teams"></a>Dov'è il pulsante Salva nella finestra dei dettagli in Teams?

[!INCLUDE [prod_short.md](includes/prod_short.md)]salva automaticamente le modifiche apportate a qualsiasi campo non appena si esce dal campo. Per uscire da un campo, fai clic/tocca un punto qualsiasi al di fuori del campo o utilizza il tasto TAB per passare al campo successivo. Quando i dati sono visualizzati in una finestra di dialogo all'interno della finestra dei dettagli, è possibile che sia necessario scegliere il pulsante **OK** affinché [!INCLUDE [prod_short.md](includes/prod_short.md)] salvi le modifiche.

### <a name="if-i-choose-to-view-details-for-a-card-will-other-users-see-my-details-window"></a>Se scelgo di visualizzare i dettagli di una scheda, gli altri utenti vedranno la finestra dei dettagli?

No. Tutti gli utenti coinvolti nella chat o nella riunione possono visualizzare la scheda vera e propria, ma solo tu vedi la finestra dei dettagli quando selezioni **Dettagli**. Gli altri utenti devono a loro volta scegliere **Dettagli** se desiderano visualizzare la finestra dei dettagli sul loro dispositivo.

### <a name="can-i-start-a-teams-call-from-the-details-window-in-teams"></a>Posso avviare una chiamata Teams dalla finestra dei dettagli in Teams?

Sì. Se stai usando l'app desktop Teams, avvia una chiamata selezionando il numero collegato in un campo con il numero di telefono, ad esempio **Numero di telefono cellulare** nella scheda **Contatto**. Teams deve essere l'app di composizione designata.

Per chiamare telefoni fissi e cellulari locali o internazionali, Teams richiede una licenza Business Voice per le chiamate aziendali. Inoltre, devi configurare Teams come soluzione per le chiamate. Per saperne di più, vedi [Pianificare la soluzione vocale di Teams](/microsoftteams/cloud-voice-landing-page) nella documentazione di Teams.

### <a name="can-i-print-documents-from-the-details-window-in-teams"></a>Posso stampare documenti dalla finestra dei dettagli in Teams?

Sì. Puoi stampare report e altri documenti utilizzando la funzionalità di stampa di [!INCLUDE [prod_short.md](includes/prod_short.md)] standard e qualsiasi stampante abilitata per il cloud configurata in **Gestione stampante** in [!INCLUDE [prod_short.md](includes/prod_short.md)]. Non è possibile stampare da Teams su stampanti locali note al dispositivo client, ad esempio le stampanti su cui si stampa in genere dal browser. Per questo motivo, non è possibile stampare dalla finestra di anteprima del report, ma solo dalla pagina principale di richiesta del report, direttamente sulle stampanti cloud.

Per ulteriori informazioni sulla configurazione delle stampanti cloud, vedi [Imposta stampanti](ui-specify-printer-selection-reports.md).

### <a name="can-i-access-the-camera-from-the-details-window-in-teams"></a>Posso accedere alla fotocamera dalla finestra dei dettagli in Teams?

Sì. Le funzionalità di [!INCLUDE [prod_short.md](includes/prod_short.md)] nella finestra dei dettagli che utilizzano la fotocamera sono disponibili in tutti i client di Teams.

### <a name="can-i-access-my-location-from-the-details-window-in-teams"></a><a name="location"></a>Posso accedere alla mia posizione dalla finestra dei dettagli in Teams?

Se utilizzi la funzionalità in [!INCLUDE [prod_short.md](includes/prod_short.md)] che consente di accedere alle coordinate della posizione corrente, ad esempio con le mappe, devi utilizzare Teams nel browser o nell'app per dispositivi mobili Teams. La posizione non è disponibile quando si usa l'app desktop Teams. 

## <a name="collaborating-with-guests"></a>[Collaborare con utenti guest](#tab/collaborating)

### <a name="can-i-share-cards-with-users-outside-my-organization"></a>Posso condividere le schede con utenti esterni all'organizzazione?

Sì. Quando componi e invii un messaggio che include una scheda, tutti i destinatari nella chat vedranno la scheda, anche se sono utenti guest o esterni alla tua organizzazione. Gli utenti guest possono anche aprire la finestra dei dettagli se dispongono delle autorizzazioni per accedere a quei dati in [!INCLUDE [prod_short.md](includes/prod_short.md)].

### <a name="is-the-experience-any-different-for-users-that-are-guests"></a>L'esperienza è differenti per gli utenti ospiti?

Sì. Invitare utenti guest esterni alla tua organizzazione a partecipare a una chat o a un canale offre loro un'esperienza simile, ma non identica, rispetto agli utenti nell'organizzazione. Quando un utente guest riceve un messaggio che include una scheda, può visualizzarlo. Gli utenti guest possono anche aprire la finestra dei dettagli se dispongono delle autorizzazioni per accedere a quei dati in [!INCLUDE [prod_short.md](includes/prod_short.md)] e di una licenza [!INCLUDE [prod_short.md](includes/prod_short.md)] nell'organizzazione. Quando un utente guest compone un messaggio, i collegamenti al suo o al tuo [!INCLUDE [prod_short.md](includes/prod_short.md)] non si espanderanno in schede.

Per informazioni su altre similarità e differenze tra utenti guest e membri del team, vedi [Esperienza degli utenti guest in Teams](/MicrosoftTeams/guest-experience) nella documentazione di Teams.

### <a name="how-does-a-guest-user-install-the-prod_shortmd-app"></a>In che modo un utente guest installa l'app [!INCLUDE [prod_short.md](includes/prod_short.md)]? 

Gli utenti guest non hanno accesso al marketplace delle app per installare personalmente le app. Tuttavia, l'app può essere installata automaticamente per tali utenti in base ai criteri della tua organizzazione. Un altro modo per un utente guest di installare l'app [!INCLUDE [prod_short.md](includes/prod_short.md)] è quando riceve un messaggio di chat che include una scheda [!INCLUDE [prod_short.md](includes/prod_short.md)]. In questo caso, l'utente sceglie il pulsante **Dettagli** o il menu nella scheda, quindi installa l'app [!INCLUDE [prod_short.md](includes/prod_short.md)] da utilizzare con l'organizzazione. Dopo aver installato l'app, un utente non riceve automaticamente alcuna autorizzazione per accedere ai dati da [!INCLUDE [prod_short.md](includes/prod_short.md)].

---

## <a name="see-also"></a>Vedere anche

[Panoramica dell'integrazione di [!INCLUDE [prod_short](includes/prod_short.md)] e Microsoft Teams](across-teams-overview.md)  
[Installare l'app [!INCLUDE [prod_short](includes/prod_short.md)] per Microsoft Teams](across-install-app-for-teams.md)  
[Risoluzione dei problemi relativi a Teams](admin-teams-troubleshooting.md)  
[Sviluppo per l'integrazione di Teams](/dynamics365/business-central/dev-itpro/developer/devenv-develop-for-teams)  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  


[!INCLUDE[footer-include](includes/footer-banner.md)]