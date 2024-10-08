---
title: Chat con Copilot (anteprima)
description: Scopri come utilizzare Chat con Copilot per trovare dati e ottenere assistenza in Business Central.
author: jswymer
ms.author: jswymer
ms.reviewer: jswymer
ms.topic: how-to
ms.date: 06/13/2024
ms.custom: bap-template
ms.collection:
  - bap-ai-copilot
  - get-started
---

# <a name="chat-with-copilot-preview"></a>Chat con Copilot (anteprima)

[!INCLUDE [preview-banner](~/../shared-content/shared/preview-includes/preview-banner.md)]

In questo articolo viene descritto come chattare con Copilot per ottenere risposte sui dati aziendali e assistenza su attività e argomenti correlati a Business Central.

[!INCLUDE [preview-note](~/../shared-content/shared/preview-includes/production-ready-preview-dynamics365.md)]

## <a name="about-chat-with-copilot"></a>Informazioni su Chat con Copilot

Microsoft Copilot è l'assistente basato sull'intelligenza artificiale che aiuta a stimolare la creatività, aumentare la produttività ed eliminare attività noiose. Tramite la chat con Copilot in Business Central, puoi porre domande e trovare dati aziendali utilizzando il linguaggio naturale. Azioni possibili:

- Trovare dati aziendali per la società in Business Central. Utilizza la chat per cercare (e aprire) dati su entità/record relativi a processi aziendali, come clienti, fornitori, ordini vendita, articoli e altro ancora. Ad esempio, chiedi a Copilot: "Mostrami l'ultimo ordine di vendita per Adatum".
- Ottenere spiegazioni o indicazioni dettagliate su varie attività. Ad esempio, chiedi "Aiutami a capire le dimensioni" o "Come posso registrare un ordine di vendita".
- Comprendere lo scopo e l'uso tipico dei singoli campi. Quando scegli **Chiedi a Copilot** in una descrizione comando di un campo, la chat si apre con un prompt Spiegazione per il nome del campo e Copilot fornisce informazioni al riguardo. Copilot si collega agli articoli a cui fa riferimento, quindi è facile verificare la descrizione.

Le risposte di Copilot provengono dalle informazioni ufficiali disponibili in Microsoft Learn nella [documentazione di Dynamics 365 Business Central](/dynamics365/business-central/).
  
L'uso della chat con Copilot semplifica il flusso di lavoro bypassando la navigazione tradizionale e la guida del prodotto.
  
> [Guarda il video](https://go.microsoft.com/fwlink/?linkid=2250609)

## <a name="prerequisites"></a>Prerequisiti

- Assicurati che la funzionalità chat con Copilot sia attivata da un amministratore. [Scopri di più sulla configurazione delle funzionalità di Copilot e IA](enable-ai.md).
- Imposta la lingua di visualizzazione in Business Central su una delle seguenti impostazioni locali inglesi: en-AU, en-CA, en-GB, en-IE, en-IN, en-NZ, en-PH, en-SG, en-US, en-ZA. [Scorpi di più sulla modifica della lingua](ui-change-basic-settings.md#language).
- Assicurati che l'ambiente Business Central si trovi in qualsiasi paese/area ad eccezione del Canada (questa funzionalità non è ancora disponibile in Canada).

## <a name="get-started-using-chat-with-copilot"></a>Iniziare a utilizzare Chat con Copilot

1. Nell'angolo in alto a destra dello schermo, seleziona l'icona ![Mostra l'icona per Chat con Copilot](media/chat-copilot-icon.png) **Copilot** ![Mostra il colore numero 1](media/callout-number-1.svg).

   Il riquadro **Copilot** viene visualizzato come mostrato nell'immagine:
   
    ![Mostra l'icona per il riquadro Chat con Copilot con callout](media/chat-with-copilot-pane.svg)

1. Nella casella **Fai una domanda** in basso ![Mostra il callout numero 2](media/callout-number-2.svg), immetti la domanda, quindi seleziona la freccia o premi <kbd>INVIO</kbd>  per ottenere una risposta.

   Il tuo input, noto come *prompt*, può essere una domanda, un'istruzione o un comando.

   > [!TIP]
   > Copilot include un paio di funzionalità che possono aiutarti a scrivere domande:
   > - Per assistenza su come formulare una domanda, seleziona una delle guide, ovvero **Trovare**, **Spiegare** o **Guida**, disponibile nella parte superiore del riquadro ![Mostra il callout numero 3](media/callout-number-3.svg) o dall'icona ![Mostra l'icona della guida rapida](media/prompt-guide-icon.png) **Visualizza prompt** sopra la casella **Fai una domanda** ![Mostra il callout numero 4](media/callout-number-4.svg). Le guide rapide sono brevi frasi predefinite che iniziano una domanda o un prompt. Ti fanno risparmiare tempo, guidano le risposte di Copilot verso una categoria di risposte e ti aiutano ad apprendere come formulare le domande per ottenere le risposte migliori.
   > - Seleziona i suggerimenti per i prompt sopra il pulsante **Visualizza prompt** ![Mostra il callout numero 5](media/callout-number-5.svg) per porre automaticamente una domanda predefinita per vedere come funzionano le domande e le risposte. I suggerimenti per prompt sono disponibili solo quando utilizzi la società demo CRONUS.

1. Esaminare le risposte visualizzate nel riquadro Copilot ![Mostra il callout numero 6](media/callout-number-6.svg).

   A seconda della domanda, la risposta può contenere testo, collegamenti a record o pagine in Business Central e collegamenti ad articoli della guida di Business Central in Microsoft Learn.

1. Fai un'altra domanda per affinare la risposta.

   La chat ricorda il contesto, il che significa che non devi ripetere i punti chiave della domanda originale.

## <a name="clear-chat-to-start-over"></a>Cancellare la chat per ricominciare

Se desideri passare a un argomento di conversazione diverso con Copilot, seleziona l'icona ![Mostra l'icona di cancellazione della chat](media/clear-chat-icon.png) **Avvia una nuova sessione chat di Copilot** nella parte inferiore del riquadro Copilot sopra la casella delle domande. Questa azione cancella i tuoi ultimi messaggi dalla memoria di Copilot. Ricominciare da capo è spesso utile dopo una lunga conversazione con molti messaggi e può aiutare Copilot a fornire risposte più precise.

La chat viene cancellata anche quando si chiude o si esce da Business Central.

## <a name="tips-for-better-questions"></a>Suggerimenti per domande migliori

Di seguito sono riportati alcuni modi per migliorare le risposte ottenute da Copilot:

- Fai domande chiare e specifiche.
- Sii conciso ed evita frasi lunghe o multiple.
- Fai una domanda alla volta. <!--Avoid asking about multiple questions in one message.-->
- Utilizza il linguaggio naturale, esprimendo le domande in modo amichevole e colloquiale.
- Utilizza parole chiave, frasi e termini che sai che vengono utilizzati in Business Central, nell'app o nella documentazione.
- Se la risposta iniziale non risponde completamente alle tue domande, fai domande di follow-up o riformula l'ultima domanda.
- Se stai facendo una domanda su un argomento diverso rispetto alla domanda precedente, cancella la sessione di chat corrente per ricominciare.

## <a name="example-prompts"></a>Prompt di esempio

Le tue domande a Copilot variano a seconda del tuo ruolo, dell'attività attuale, dei processi seguiti dalla tua organizzazione e di come ti esprimi a parole. Di seguito sono riportati esempi che mostrano diversi modi di porre domande nel riquadro chat che possono ispirarti a scrivere le tue domande in base alla tua situazione.

Prompt: `Find the Item with Description 'ATHENS Desk'`

In questo esempio, fornisci istruzioni chiare a Copilot per individuare un singolo record. Ad esempio, suggerisci che il record si trova nell'elenco degli articoli. Indichi che il campo "Descrizione" deve essere un testo specifico che hai digitato utilizzando virgolette e con le maiuscole corrette. Copilot di solito risponde in modo accurato quando vengono forniti alcuni suggerimenti precisi, ma è anche possibile utilizzare un linguaggio più informale come nel prossimo esempio.

Prompt: `Give me the latest invoice for adatum`

In questo esempio, chiedi a Copilot di individuare un record, ma la domanda è meno precisa e potrebbe comportare una risposta meno accurata. Copilot può spesso capire, o indovinare, che la fattura che stai cercando non è una fattura di acquisto ma una fattura di vendita dell'elenco Fattura di vendita registrata. Copilot dovrebbe anche abbinare `adatum` a `Adatum Corporation`, ovvero il nome completo e preciso del nome del cliente di vendita associato alla fattura.

Prompt: `Show me customer ledger entries for Adatum from about three weeks ago`

In questo esempio, chiedi al copilota di risolvere un enigma di date comune che in genere richiede l'apertura di un calendario come riferimento o l'utilizzo di filtri avanzati per intervalli di date. Copilot solitamente è in grado di comprendere espressioni comuni e termini commerciali.

Prompt: `How does I save my filterrings for later?`

In questo esempio chiedi a Copilot indicazioni su come eseguire alcune attività in Business Central. Di solito Copilot riesce a comprendere l'intento della tua domanda, anche se sono presenti alcuni errori grammaticali, di ortografia o abbreviazioni.

## <a name="provide-feedback-on-answers"></a>Fornire feedback sulle risposte

Puoi valutare le risposte che ricevi da Copilot utilizzando il pulsante Mi piace (pollice su) per una valutazione buona o il pulsante Non mi piace (pollice giù) per una valutazione scarsa. Quando selezioni il pulsante Non mi piace, puoi scegliere un motivo, tra cui impreciso, inappropriato o altro. Queste informazioni possono aiutarci a migliorare i suggerimenti.

<!--
1. If you want help getting you're question started, select the prompts either from the **Find**, **Explain**, or **Guide** buttons at the top of the Coplit pane or use the **View Prompts** menu above **Ask a question** box at the bottom.

   Prompts are predefined short phrases that start a question. Apart from saving you time, they're designed to target responses to specific categories. They also help you undestand how you can phrase questions to get the responses.-->
   
## <a name="see-also"></a>Vedere anche

- [Risolvere i problemi relativi alle funzionalità di Copilot e IA](ai-copilot-troubleshooting.md)  
- [Configurare le funzionalità di Copilot e IA](enable-ai.md)  
- [Domande frequenti sull'intelligenza artificiale responsabile per Chat con Copilot](faqs-chat-with-copilot.md)  
- [Risorse per la guida in Business Central](product-help-and-support.md)  
