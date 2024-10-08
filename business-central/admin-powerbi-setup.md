---
title: Abilitazione dell'integrazione di Power BI con Business Central
description: 'Scopri come impostare la connessione a Power BI. Con i report Power BI puoi ottenere informazioni dettagliate, business intelligence e KPI dai dati di Business Central.'
author: jswymer
ms.topic: get-started
ms.search.keywords: 'Power BI, setup, analysis, reporting, financial report, business intelligence, KPI'
ms.date: 01/28/2024
ms.author: jswymer
ms.service: dynamics-365-business-central
ms.custom: bap-template
ms.reviewer: jswymer
---
# <a name="enabling-power-bi-integration-with-"></a>Abilitazione dell'integrazione di Power BI con [!INCLUDE[prod_short](includes/prod_short.md)]

[!INCLUDE[azure-ad-to-microsoft-entra-id](~/../shared-content/shared/azure-ad-to-microsoft-entra-id.md)]

Questo articolo descrive come preparare [!INCLUDE[prod_short](includes/prod_short.md)] per l'integrazione con Power BI. [!INCLUDE[prod_short](includes/prod_short.md)] online è già abilitato per l'integrazione, sebbene ci siano alcune informazioni sulle licenze che si potrebbe voler leggere. Per [!INCLUDE[prod_short](includes/prod_short.md)] locale sarà stato configurato l'ambiente a cui connettere Power BI prima che gli utenti possano lavorarci.

## <a name="power-bi-licensing"></a><a name="license"></a>Licenze Power BI

Con [!INCLUDE[prod_short](includes/prod_short.md)], gli utenti ottengono una licenza Power BI che fornisce l'accesso alle funzionalità più comuni in [!INCLUDE[prod_short](includes/prod_short.md)] e Power BI. È anche possibile acquistare una licenza Power BI Pro che fornisce accesso a funzionalità aggiuntive. La tabella seguente fornisce una panoramica delle funzionalità disponibili con ciascuna licenza.

|Licenza Power|Visualizzare report|Creare report|Condividere report|Aggiornare report| App [!INCLUDE[prod_short](includes/prod_short.md)]|
|-------------|--------||
|Power BI gratuito|![un segno di spunta.](media/check.png)|![un altro segno di spunta](media/check.png)|(limitato)|(limitato)||
|Power BI Pro|![ancora un altro segno di spunta.](media/check.png)|![è un segno di spunta](media/check.png)|![ancora un segno di spunta](media/check.png)|(esteso)|![ultimo segno di spunta](media/check.png)|

Per ulteriori informazioni, vedere [Concedere in licenza il servizio Power BI per gli utenti dell'organizzazione](/power-bi/admin/service-admin-licensing-organization) o [Iscriversi al servizio Power BI come utente singolo](/power-bi/fundamentals/service-self-service-signup-for-power-bi).

## <a name="expose-data-through-api-or-odata-web-services"></a><a name="exposedata"></a>Esporre i dati tramite API o servizi web OData

Business Central offre due modi per esporre i dati che possono essere usati dai report Power BI: pagine o query API e servizi web Open Data Protocol (OData).

### <a name="api-pages-and-queries"></a>Pagine e query API

> **APPLICABILE A:** Solo Business Central Online

Gli sviluppatori possono definire oggetti pagina e oggetti query di tipo *API*. In questo modo, possono esporre i dati dalle tabelle del database tramite un servizio REST supportato da webhook, abilitato per OData v4. Questo tipo di dati non può essere visualizzato nell'interfaccia utente, ma è destinato alla creazione di servizi di integrazione affidabili.

Business Central online è disponibile con una serie di API integrate, che è possibile utilizzare per ottenere dati per le entità aziendali più comuni, come clienti, articoli, ordini di vendita e altro. Non è richiesto alcun lavoro aggiuntivo o configurazione per utilizzare queste API come origine dati per report Power BI. Per ulteriori informazioni su queste API, vedi [API Business Central V2.0](/dynamics365/business-central/dev-itpro/api-reference/v2.0/).

Business Central online supporta anche le API personalizzate. Gli sviluppatori di applicazioni delle soluzioni Business Central possono creare le proprie pagine e query API e comprimerle in app. Puoi installare le app nel tuo tenant. Una volta installate, puoi utilizzare le pagine API per il tuo report Power BI, come faresti con le API integrate (v2.0). Per ulteriori informazioni su come creare un'API esponendo pagine o query, vedi [Sviluppo di un'API personalizzata](/dynamics365/business-central/dev-itpro/developer/devenv-develop-custom-api).

> [!IMPORTANT]
> A partire da febbraio 2022, i report Power BI per [!INCLUDE[prod_short](includes/prod_short.md)] online provengono da una replica del database di sola lettura secondaria per motivi di prestazioni. Di conseguenza, gli sviluppatori AL dovrebbero evitare di progettare pagine API che apportano modifiche al database mentre le pagine aprono o caricano record. In particolare, considera il codice dei trigger AL: OnInit, OnOpenPage, OnFindRecord, OnNextRecord, OnAfterGetRecord e OnAfterGetCurrRecord. Queste modifiche al database, in alcuni casi, possono causare problemi di prestazioni e impedire l'aggiornamento dei dati del report. Per ulteriori informazioni, vedi [Articoli sulle prestazioni per gli sviluppatori](/dynamics365/business-central/dev-itpro/performance/performance-developer?branch=main#writing-efficient-web-services) nel contenuto per gli sviluppatori di Business Central.
>
> In rari casi, il comportamento causerà un errore quando un utente tenta di ottenere dati dall'API per un report in Power BI Desktop. Tuttavia, se sono necessarie modifiche al database nell'API personalizzata, gli utenti Power BI Desktop possono forzare il comportamento. Per ulteriori informazioni, vedi [Creare report Power BI per visualizzare i dati di Business Central](across-how-use-financials-data-source-powerbi.md#fixing-problems).

### <a name="odata-web-services"></a>Servizi Web OData

È possibile pubblicare oggetti dell'applicazione Business Central, come codeunit, pagine e query, come [servizi web OData](/dynamics365/business-central/dev-itpro/webservices/odata-web-services). Con Business Central online, sono disponibili molti servizi Web pubblicati per impostazione predefinita. Un modo agevole di individuare i *servizi Web* consiste nel cercarli in [!INCLUDE[prod_short](includes/prod_short.md)]. Nella pagina **Servizi web**, assicurarsi che il campo **Pubblica** sia selezionato per i servizi web elencati sopra. Per ulteriori informazioni sulla pubblicazione di servizi Web, vedere [Pubblicare un servizio Web](across-how-publish-web-service.md).

Per informazioni su cosa è possibile fare per garantire le migliori prestazioni dei servizi Web, come visto dal Business Central Server (l'endpoint) e dal consumatore (il client), leggere [Scrittura di servizi Web efficienti](/dynamics365/business-central/dev-itpro/performance/performance-developer#writing-efficient-web-services).

### <a name="choosing-whether-to-use-api-pages-or-odata-web-services"></a>Scegliere se utilizzare le pagine API o i servizi web OData

Quando possibile, ti invitiamo a utilizzare le pagine API invece del servizio web OData. Le pagine API sono più veloci nel caricamento dei dati nei report Power BI rispetto ai servizi Web OData. Inoltre, sono più flessibili perché ti consentono di ottenere dati dai campi della tabella che non sono definiti in un oggetto pagina.

<!--## <a name="setup"></a>Set up [!INCLUDE[prod_short](includes/prod_short.md)] on-premises for Power BI integration

This section explains the requirements for a [!INCLUDE[prod_short](includes/prod_short.md)] on-premises deployment to integrate with Power BI.

1. Configure either [NavUserPassword](/dynamics365/business-central/dev-itpro/administration/authenticating-users-with-navuserpassword) or [Microsoft Entra ID](/dynamics365/business-central/dev-itpro/administration/authenticating-users-with-azure-ad-overview) as the authentication method for the deployment.  
    
    > [!NOTE]
    > Power BI integration doesn't support Windows authentication and is not supported on Windows Client.

2. Enable OData web services and the ODataV4 endpoint.

    OData web service must be enabled on the [!INCLUDE[server](includes/server.md)], and OData port opened in firewall. For more information, see [Configuring Business Central Server - OData Web Services](/dynamics365/business-central/dev-itpro/administration/configure-server-instance#ODataServices).

    The local server must be accessible from the Internet.

3. Give [!INCLUDE[prod_short](includes/prod_short.md)] user accounts a web service access key.

    A web service access key is only needed to view [!INCLUDE[prod_short](includes/prod_short.md)] data in Power BI. You can assign a web service access key to each user account. Or instead, create a specific account with a web service access key for use by all users. For more information, see [Web Services Authentication](/dynamics365/business-central/dev-itpro/webservices/web-services-authentication#generate-a-web-service-access-key).

    <!--
    > [!IMPORTANT]
    > With [!INCLUDE[prod_short](../developer/includes/prod_short.md)] online, the use of access keys (Basic Auth) for web service authentication is [deprecated](/dynamics365/business-central/dev-itpro/upgrade/deprecated-features-w1#accesskeys). We recommend that you use OAuth2 instead. For more information, see [Use OAuth to Authorize Business Central Web Services](/dynamics365/business-central/dev-itpro/webservices/authenticate-web-services-using-oauth).-->

<!--4. Create an application registration for [!INCLUDE[prod_short](includes/prod_short.md)] in Microsoft Azure.

    To view Power BI reports embedded in [!INCLUDE[prod_short](includes/prod_short.md)] pages, an application must be registered for [!INCLUDE[prod_short](includes/prod_short.md)] in Microsoft Azure. The registered application needs permission to Power BI services. At a minimum, the app requires  **User.ReadWrite.All** permission. For users to view reports from shared Power BI workspaces, the app requires **Workspace.Read.All** permission. For more information, see [Registering [!INCLUDE[prod_short](includes/prod_short.md)] On-Premises in Microsoft Entra ID for Integrating with Other Services](/dynamics365/business-central/dev-itpro/administration/register-app-azure).

    > [!NOTE]
    > If your deployment uses NavUserPassword authentication, [!INCLUDE[prod_short](includes/prod_short.md)] connects to the same Power BI service for all users. You'll specify this service account as part of registering the application. With Microsoft Entra authentication, [!INCLUDE[prod_short](includes/prod_short.md)] connects to the Power BI service associated with the individual user accounts.

    <!-- Windows authentication can also be used but you can't get data from BC in Power BI -->
<!--5. Make the initial connection from Business Central to Power BI.

    Before end-users can use Power BI in [!INCLUDE[prod_short](includes/prod_short.md)], an Azure application administrator will have to give consent to the Power BI service.

    To make the initial connection, open [!INCLUDE[prod_short](includes/prod_short.md)], and run **Get Started with Power BI** from the Home page. This action will lead you through the consent process, and check your Power BI license. When prompted sign in using an Microsoft Entra admin account. For more information, see [Connect to Power BI - one time only](across-working-with-powerbi.md#connect).-->

## <a name="setting-up-dataflows"></a>Impostazione dei flussi di dati

I flussi di dati ti consentono di acquisire, trasformare e caricare dati in un'area di lavoro Power BI e quindi utilizzare i dati come base per i tuoi report. In alcuni casi questi flussi di dati possono riscontrare errori temporanei durante l'esecuzione di un aggiornamento pianificato. Il messaggio di errore è simile a questo:`DataSource.Error: OData: Unable to read data from the transport connection: An existing connection was forcibly closed by the remote host.` 

Utilizzando PowerAutomate, puoi impostare nuovi tentativi per questa situazione. Per ulteriori informazioni, vedi [Riprovare automaticamente un flusso di dati in caso di errore](/power-query/dataflows/automatically-retry-dataflow).

## <a name="see-also"></a>Vedere anche

[Business Central e Power BI](admin-powerbi.md)  
[Componente di integrazione Power BI e panoramica dell'architettura per [!INCLUDE[prod_short](includes/prod_short.md)]](admin-powerbi-overview.md)  
[Power BI per i consumatori](/power-bi/consumer/end-user-consumer)  
[Il "nuovo look" del servizio Power BI](/power-bi/service-new-look)  
[Avvio rapido: connettersi ai dati in Power BI Desktop](/power-bi/desktop-quickstart-connect-to-data)  
[Documentazione di Power BI](/power-bi/)  
[Business Intelligence](bi.md)  
[Preparazione al business](ui-get-ready-business.md)  
[Importazione dei dati aziendali da altri sistemi contabili](across-import-data-configuration-packages.md)  
[Impostazione di [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md)  
[Usare [!INCLUDE[prod_short](includes/prod_short.md)] come origine dati di Power BI](across-how-use-financials-data-source-powerbi.md)  
[Usare [!INCLUDE[prod_short](includes/prod_short.md)] come origine dati di Power Apps](across-how-use-financials-data-source-powerapps.md)  
[Usare [!INCLUDE[prod_short](includes/prod_short.md)] in Power Automate](across-how-use-financials-data-source-flow.md)  




[!INCLUDE[footer-include](includes/footer-banner.md)]
