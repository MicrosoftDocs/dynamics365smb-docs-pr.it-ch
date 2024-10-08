---
title: Domande frequenti sull'assistenza all'analisi (anteprima)
description: 'Queste domande frequenti forniscono informazioni sulla tecnologia di IA utilizzata per analizzare dati nelle pagine in Business Central. Includono considerazioni e dettagli chiave su come viene utilizzata l''intelligenza artificiale, come è stata testata e valutata ed eventuali limitazioni specifiche.'
ms.date: 06/13/2024
ms.custom:
  - responsible-ai-faqs
ms.topic: article
author: jswymer
ms.author: jswymer
ms.reviewer: jswymer
ms.search.keywords: 'copilot, AI'
ms.collection:
  - bap-ai-copilot
---

# <a name="faq-for-analysis-assist-preview"></a>Domande frequenti sull'assistenza all'analisi (anteprima)

[!INCLUDE [preview-banner](~/../shared-content/shared/preview-includes/preview-banner.md)]

Queste domande frequenti descrivono l'impatto sull'intelligenza artificiale della funzionalità di assistenza all'analisi in [!INCLUDE[prod_short](includes/prod_short.md)].

[!INCLUDE [preview-note](~/../shared-content/shared/preview-includes/production-ready-preview-dynamics365.md)]

## <a name="what-is-analysis-assist"></a>Cos'è l'assistenza all'analisi?

L'assistenza all'analisi è un copilota che fornisce assistenza per l'uso della [modalità di analisi dei dati](analysis-mode.md) in Business Central. La modalità di analisi dei dati ti consente di organizzare, aggregare e riepilogare i dati in pagine e query per renderli più adatti all'analisi e all'estrazione di informazioni significative. Con l'assistenza all'analisi, puoi creare automaticamente la visualizzazione dei dati che desideri analizzare esprimendo le tue esigenze in un linguaggio semplice e naturale, come "mostra i venditori per ubicazione ordinati per numero di acquisti". L'assistenza all'analisi semplifica l'utilizzo dei dati senza la necessità di competenze tecniche complesse.

## <a name="what-are-capabilities-of-analysis-assist"></a>Quali sono le funzionalità dell'assistenza all'analisi?

L'assistenza all'analisi è basata sugli strumenti per sviluppatori per Copilot in Business Central. Utilizza il servizio OpenAI di Azure per convertire le istruzioni non strutturate in un progetto strutturato per visualizzare i dati nella modalità di analisi, senza creare, modificare o aggiornare i dati aziendali del cliente.

## <a name="what-is-the-intended-use-of-analysis-assist"></a>Qual è l'uso previsto dell'assistenza all'analisi?

L'assistenza all'analisi consente di creare schede di analisi nella modalità di analisi dei dati per presentare i dati in un modo che rende più facile trarre conclusioni. Tuttavia, è importante notare che l'assistenza all'analisi non fornisce informazioni o conclusioni dirette sui dati. È uno strumento per aiutare gli utenti a organizzare e visualizzare i propri dati. Spetta all'utente estrarre informazioni utili, scoprire tendenze e prendere decisioni informate per generare valore aziendale.

## <a name="how-was-analysis-assist-evaluated-what-metrics-are-used-to-measure-performance"></a>Come è stato valutata l'assistenza all'analisi? Quali metriche vengono utilizzate per misurare le prestazioni?

- La funzionalità è stata sottoposta a test estesi in base ai dati dimostrativi di [!INCLUDE[prod_short](includes/prod_short.md)] e altri cataloghi di prodotti fittizi. A Copilot sono state fornite numerosi prompt nelle versioni locali inglesi supportate. I prompt coprivano un'ampia gamma di istruzioni per l'analisi dei dati e stili di intento di espressione. I risultati sono stati valutati rispetto a accuratezza, pertinenza e sicurezza.

- La funzionalità è stata creata in conformità con lo standard di intelligenza artificiale responsabile di Microsoft. [Scopri di più sull'intelligenza artificiale responsabile di Microsoft](https://aka.ms/RAI).

## <a name="how-does-microsoft-monitor-the-quality-of-generated-content"></a>In che modo Microsoft monitora la qualità del contenuto generato?

Microsoft dispone di vari sistemi per garantire che i contenuti generati da Copilot siano della massima qualità, per rilevare abusi e garantire la sicurezza dei nostri clienti e dei loro dati.

Gli utenti hanno la possibilità di fornire feedback a ogni risposta di Copilot e segnalare contenuti imprecisi o inappropriati per aiutare Microsoft a migliorare questa funzionalità.

- Se riscontri contenuto generato inappropriato, segnalalo a Microsoft utilizzando questo modulo di feedback: [Segnala abuso](https://go.microsoft.com/fwlink/?linkid=2249810)

- Analizziamo il feedback degli utenti sulla funzionalità e lo usiamo per migliorare le risposte.

  Per fornire feedback, utilizza l'icona Mi piace (pollice su) o Non mi piace (pollice giù) nel riquadro **Copilot**in [!INCLUDE[prod_short](includes/prod_short.md)].

- Microsoft potrebbe disattivare le funzionalità basate su Copilot per clienti selezionati se viene rilevato un abuso della funzionalità.

## <a name="what-are-the-limitations-of-analysis-assist-how-can-users-minimize-the-impact-of-the-analysis-assist-limitations-when-using-the-system"></a>Quali sono le limitazioni dell'assistenza all'analisi? In che modo gli utenti possono ridurre al minimo l'impatto delle limitazioni dell'assistenza all'analisi durante l'utilizzo del sistema?

- Limitazioni generali dell'IA:

  I sistemi di intelligenza artificiale sono strumenti preziosi, ma non deterministici. Il contenuto che generano potrebbe non essere accurato. È importante utilizzare il proprio giudizio per esaminare e verificare le risposte prima di prendere decisioni che potrebbero influenzare le parti interessate come clienti e partner.

- Lingue disponibili

   [!INCLUDE[analysis-assist-language-support](includes/analysis-assist-language-support.md)]

   La qualità delle risposte può anche essere inferiore se l'impostazione della lingua per l'utente in Business Central è diversa dalla lingua principale dei dati aziendali nel database [!INCLUDE[prod_short](includes/prod_short.md)].
  
- Limitazione geografica:
  
   La funzionalità è disponibile in tutte le [aree geografiche/paesi di Business Central](/dynamics365/business-central/dev-itpro/compliance/apptest-countries-and-translations) supportati<!-- except for Canada-->. Tuttavia, la funzionalità utilizza il servizio OpenAI di Microsoft Azure, attualmente disponibile per Business Central in alcune aree geografiche. Se il tuo ambiente si trova in un paese/area geografica in cui il servizio OpenAI di Azure non è disponibile, gli amministratori devono consentire lo spostamento dei dati tra aree geografiche. [Ulteriori informazioni sullo spostamento di dati di Copilot tra aree geografiche](/dynamics365/business-central/ai-copilot-data-movement).

- Alcune limitazioni di settore, prodotto e soggetto:

  Le organizzazioni che operano in alcuni settori aziendali, ad esempio quello medico, farmaceutico, legale e delle armi, potrebbero riscontrare una qualità inferiore del servizio.

## <a name="what-data-does-analysis-collect-and-how-is-it-used"></a>Quali dati vengono raccolti dall'analisi e come vengono utilizzati?

La funzionalità di assistenza all'analisi raccoglie i dati minimi necessari a Business Central per offrire il servizio. Microsoft non utilizza i dati della tua società, incluso il testo inviato a Copilot, per addestrare i modelli fondamentali a vantaggio di altri. Per ulteriori informazioni, vedi [Termini di Dynamics 365 per le funzionalità basate sul servizio OpenAI di Azure](https://go.microsoft.com/fwlink/?linkid=2236010).

Raccoglie inoltre i dati dal feedback che gli utenti possono fornire utilizzando le icone Mi piace (pollice su) o Non mi piace (pollice giù) nella pagina **Copilot** dell'assistenza all'analisi. I dati sono anonimi e includono la scelta Mi piace o Non mi piace, il motivo di Non mi piace, se fornito, e la funzionalità Copilot a cui si applica il feedback.

## <a name="see-also"></a>Vedere anche

[Analizzare i dati con Copilot (anteprima)](analysis-assist.md)
