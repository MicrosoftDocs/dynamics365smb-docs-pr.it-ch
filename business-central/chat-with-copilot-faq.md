---
title: Domande frequenti su Chat con Copilot
description: 'Scopri come chattare con Copilot, un assistente virtuale che ti aiuta a utilizzare Business Central. Trova le risposte alle domande più comuni su funzionalità, impostazioni e limitazioni della chat.'
author: jswymer
ms.author: jswymer
ms.reviewer: jswymer
ms.topic: conceptual
ms.collection:
  - bap-ai-copilot
ms.date: 06/13/2024
ms.custom: bap-template jswymer
---
# <a name="chat-with-copilot-faq"></a>Domande frequenti su Chat con Copilot

[!INCLUDE [preview-banner](~/../shared-content/shared/preview-includes/preview-banner.md)]

Questo articolo fornisce le risposte ad alcune domande comuni sulla chat con Copilot in [!INCLUDE[prod_short](includes/prod_short.md)]. Per domande relative all'intelligenza artificiale e alla chat, consulta [Domande frequenti sull'intelligenza artificiale responsabile per Chat con Copilot](faqs-chat-with-copilot.md).

[!INCLUDE [preview-note](~/../shared-content/shared/preview-includes/production-ready-preview-dynamics365.md)]

## <a name="can-admins-grant-or-deny-permission-to-individual-users-to-get-access-to-chat"></a>Gli amministratori possono concedere o negare l'autorizzazione a singoli utenti per accedere alla chat?

No, non esiste alcuna autorizzazione o set di autorizzazioni per la chat. Se la chat è attivata nella pagina [Funzionalità di Copilot e IA](enable-ai.md), ogni utente in un ambiente ha accesso alla chat.
 
## <a name="is-chat-available-on-tablet-phone-or-other-form-factors"></a>La chat è disponibile su tablet, telefono o altri fattori di forma?

No, il riquadro della chat è disponibile solo nel client Web [!INCLUDE[web_client](includes/web_client.md)].

## <a name="i-dont-use-business-central-in-english-what-are-my-options"></a>Non utilizzo Business Central in inglese. Quali sono le opzioni disponibili?

Al momento la chat è disponibile solo in inglese. Puoi impostare l'inglese come lingua utente in [Impostazioni personali](ui-change-basic-settings.md#language).

## <a name="what-version-of-business-central-do-i-need-for-chat"></a>Quale versione di Business Central è necessaria per la chat?

La chat è disponibile in anteprima pubblica dalla versione 24.0 (ciclo di rilascio 1 del 2024).

## <a name="does-chat-work-with-my-customizations"></a>La chat funziona con le mie personalizzazioni?

Dipende dal tipo di domanda che poni a Copilot. Ad esempio:

- Se poni domande per trovare i record, puoi trovare i record nelle tue tabelle personalizzate che utilizzano campi personalizzati.
- Se chiedi spiegazioni o indicazioni a Copilot, non ha accesso ad alcuna informazione sulle tue personalizzazioni o sulla documentazione per i tuoi componenti aggiuntivi.

## <a name="how-do-i-open-a-record-or-page-with-chat"></a>Come posso aprire un record o una pagina con chat?

Quando chiedi a Copilot di trovare record in [!INCLUDE[prod_short](includes/prod_short.md)], visualizza tutti i record trovati come riquadri o collegamenti selezionabili nel riquadro della chat. Durante l'anteprima, Copilot non passa automaticamente ad alcuna pagina.

## <a name="why-do-i-get-different-answers-from-copilot-for-the-same-question"></a>Perché Copilot fornisce risposte diverse per la stessa domanda?

Copilot potrebbe occasionalmente rispondere in modi diversi. Le risposte non sono sempre identiche.

## <a name="how-do-i-use-the-copy-function-on-chat-messages"></a>Como posso utilizzare la funzione Copia nei messaggi di chat?

Puoi utilizzare il pulsante Copia per copiare un messaggio precedente nella conversazione con Copilot, incollarlo nella casella di input per provare o riprovare una variante del tuo messaggio a Copilot.

## <a name="can-i-customize-or-extend-chat"></a>Posso personalizzare o estendere la chat?

Durante l'anteprima, il riquadro della chat e le risposte di Copilot non possono essere modificati in alcun modo tramite personalizzazione, componenti aggiuntivi o individualizzazione.

## <a name="does-copilot-search-for-data-in-other-companies-or-environments"></a>Copilot cerca i dati in altre società o ambienti?

Copilot cerca solo i record nella società a cui hai effettuato l'accesso. Non cerca dati in più ambienti o società.

## <a name="what-can-i-do-if-the-chat-pane-doesnt-show"></a>Cosa posso fare se il riquadro della chat non viene visualizzato?

Verifica che la lingua utente in **Impostazioni personali** sia impostata su Inglese e che la versione del tuo ambiente sia 24.0 o successiva. Nella pagina Funzionalità di Copilot e IA, assicurati che l'amministratore abbia attivato il consenso per i dati in tutte le aree geografiche e abbia attivato la chat. Inoltre, assicurati che la localizzazione del tuo ambiente non sia il Canada.

Se ancora non vedi la funzionalità Chat con Copilot, è possibile che Microsoft ne stia ancora eseguendo la distribuzone nella tua area geografica. Copilot è stato implementato per i clienti statunitensi nell'aprile 2024 e nelle settimane successive lo sarà nelle localizzazioni di altri paesi/aree.

## <a name="why-does-copilot-only-show-three-records-in-the-chat-pane"></a>Perché Copilot mostra solo tre record nel riquadro della chat?

Quando chiedi a Copilot di trovare record, il modo in cui formuli la domanda determina il modo in cui Copilot identifica e applica i filtri sulle pagine per trovare ciò che stai cercando. Per mantenere le risposte concise, il riquadro della chat visualizza un massimo di tre riquadri di record, anche quando Copilot trova record più pertinenti.

## <a name="why-does-copilot-give-incorrect-answers-to-calculations"></a>Perché Copilot fornisce risposte errate ai calcoli?

Durante l'anteprima, Chat con Copilot può aiutarti a trovare record, spiegare concetti e guidarti su come completare attività in Business Central. Non sono supportati altri casi d'uso, come la somma di un campo tra record o il calcolo dell'importo mensile medio. Ci auguriamo di aggiungere competenze matematiche di base a Copilot in futuro.

## <a name="can-i-use-speech-instead-of-typing-my-prompts"></a>Posso usare il riconoscimento vocale anziché digitare i miei messaggi?

Puoi chattare con Copilot utilizzando la digitazione vocale per parlare invece di digitare le parole nel riquadro della chat. La digitazione vocale utilizza il riconoscimento vocale online ed è disponibile con Windows. Per usare il riconoscimento vocale, attiva la finestra dei messaggi di chat, quindi usa la scelta rapida <kbd>Windows</kbd>+<kbd> H</kbd> e inizia a parlare. Per ulteriori informazioni, vedi [Utilizza la digitazione vocale per parlare anziché digitare sul PC](https://support.microsoft.com/windows/use-voice-typing-to-talk-instead-of-type-on-your-pc-fec94565-c4bd-329d-e59a-af033fa5689f).

## <a name="next-steps"></a>Passaggi successivi

- [Chat con Copilot (anteprima)](chat-with-copilot.md)
