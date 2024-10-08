---
title: Ottimizzare Outlook per la Posta in arrivo aziendale
description: Informazioni su come migliorare l'esperienza con la Posta in arrivo aziendale in Business Microsoft Outlook.
author: jswymer
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'Outlook, Microsoft 365, inbox, business inbox, WebView2, Edge, addin, add-in'
ms.date: 12/06/2023
ms.author: jswymer
ms.service: dynamics-365-business-central
ms.reviewer: jswymer
---
# <a name="optimize-outlook-for-your-business-inbox"></a>Ottimizzare Outlook per la Posta in arrivo aziendale

Questo articolo discute le operazioni necessarie per ottenere la migliore esperienza possibile con Posta in arrivo aziendale in Microsoft Outlook. 

## <a name="update-outlook"></a>Aggiorna Outlook

Esegui aggiornamento alla versione di Outlook 2012 o successiva.

> [!NOTE]
> Se non riesci ad aggiornare Outlook alla versione 2012 o successiva, assicurati di eseguire almeno l'aggiornamento alla versione 1905. Ciò impedisce l'esecuzione del componente aggiuntivo di Outlook utilizzando componenti Internet Explorer legacy

### <a name="how-to-check-your-version-of-outlook"></a>Come controllare la tua versione di Outlook

Se utilizzi Office 2019 o Microsoft 365, segui questa guida del supporto Microsoft per verificare la versione di Outlook installata:  

[Informazioni su Office: quale versione di Office sto utilizzando?](https://support.microsoft.com/office/about-office-what-version-of-office-am-i-using-932788b8-a3ce-44bf-bb09-e334518b8b19)

### <a name="how-to-update-outlook"></a>Istruzioni per aggiornare Outlook

Per aggiornare Outlook alla versione più recente, seguire questa guida del supporto Microsoft o contattare l'amministratore:

[Installare gli aggiornamenti di Office](https://support.microsoft.com/office/install-office-updates-2ab296f3-7f03-43a2-8e50-46de917611c5)

## <a name="install-microsoft-edge-webview2"></a>Installare Microsoft Edge WebView2

Assicurarsi che Microsoft Edge WebView2 sia installato sul tuo dispositivo.

### <a name="how-to-check-if-microsoft-edge-webview2-is-installed"></a>Come verificare se Microsoft Edge WebView2 è installato

Per verificare se Microsoft Edge WebView2 è installato su un computer, effettuare le seguenti operazioni:

Dal menu Start:

1. Scegli **Start**![Menu Start di Windows.](media/windows-start-icon.png "Icona Start di Windows") > **Impostazioni** ![Impostazioni di Windows](media/windows-settings-icon.png "Icona Impostazioni di Windows") > **App e funzionalità**.
2. Nella casella di ricerca, digitare **WebView2**. Se Microsoft Edge WebView2 è installato, viene visualizzata la voce **Microsoft Edge Webview2 Runtime**.

Dal pannello di controllo:

1. Nella casella di ricerca accanto a **Start** ![Start di Windows](media/windows-start-icon.png "Icona Start di Windows"), digitare **Pannello di controllo**, quindi selezionare il risultato.
2. Scegliere **Programmi** > **Programmi e funzionalità**.
3. Nella casella di ricerca, digitare **WebView2**. Se Microsoft Edge WebView2 è installato, viene visualizzata la voce **Microsoft Edge Webview2 Runtime**.

### <a name="how-to-install-microsoft-edge-webview2"></a>Come installare Microsoft Edge WebView2

1. Con il tuo browser, vai a [https://developer.microsoft.com/microsoft-edge/webview2/](https://developer.microsoft.com/microsoft-edge/webview2/).
2. Scegliere **Scarica**.
3. Impostare **Seleziona architettura** in base al proprio sistema.
4. Scegliere **Scarica**.

> [!NOTE]
> La tua organizzazione potrebbe avere restrizioni sui componenti che possono essere installati sul tuo dispositivo. Contattare l'amministratore per l'assistenza.

## <a name="use-a-supported-browser"></a>Utilizzare un browser supportato

Prendere in considerazione la possibilità di utilizzare Outlook per il Web in uno dei browser supportati da Business Central. Per un elenco di browser supportati, vedere [Requisiti minimi per l'utilizzo di Business Central](product-requirements.md#browsers).

## <a name="see-also"></a>Vedere anche

[Preparazione al business](ui-get-ready-business.md)  
[Scaricare Business Central sul dispositivo mobile](install-mobile-app.md)  
[Inviare documenti tramite e-mail](ui-how-send-documents-email.md)  
[Finanze](finance.md)  
[Vendite](sales-manage-sales.md)  
[Acquisti](purchasing-manage-purchasing.md)  
[Requisiti minimi per Outlook](product-requirements.md#outlook)  
[Utilizzare i componenti aggiuntivi in Outlook sul Web](https://support.office.com/article/Using-Add-ins-in-Outlook-on-the-web-8f2ce816-5df4-44a5-958c-f7f9d6dabdce?appver=OWB150)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
