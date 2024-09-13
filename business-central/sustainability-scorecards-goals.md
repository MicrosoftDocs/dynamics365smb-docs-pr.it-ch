---
title: Schede didattiche e obiettivi di sostenibilità
description: Scopri come impostare e utilizzare scorecard e obiettivi di sostenibilità.
author: altotovi
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'Sustainability, ESG, emission, GHG, CSRD, scorecard, goal, forecast, budget'
ms.search.form: null
ms.date: 08/19/2024
ms.author: altotovi
ms.service: dynamics-365-business-central
ms.reviewer: solsen
---

# Panoramica delle scorecard e degli obiettivi di sostenibilità

Questo articolo fornisce indicazioni su come creare scorecard e obiettivi e su come aggiornare lo stato degli obiettivi. Le scorecard e gli obiettivi consentono alle organizzazioni di gestire parametri di sostenibilità e di monitorarli rispetto agli obiettivi aziendali chiave. È possibile creare obiettivi in base ai valori attuali e target, in modo che gli utenti possano tenere traccia dell'andamento delle emissioni attuali rispetto ai periodi precedenti.  

## Crea una scheda di valutazione  

Per creare una nuova  *Scheda di valutazione della sostenibilità*, seguire i passaggi:

1. Seleziona l'icona ![lampadina che apre la funzionalità Dimmi](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), Icona, inserisci **Schede di valutazione della sostenibilità**, quindi Seleziona il relativo collegare. 
2. Nella pagina  **Schede di valutazione della sostenibilità**, Seleziona **Nuovo** per creare una nuova scheda di valutazione.  
3. Specificare il **numero.** E i campi  **Nome** nella scheda dettaglio **Generale**, quindi aggiungere il  **Proprietario**. 

> [NOTA!] Nel campo  **Proprietario**, puoi scegliere solo gli utenti che hanno selezionato il campo  **Responsabile sostenibilità** nella tabella  **Configurazione utente** . 

## Creare obiettivi  

Per creare un nuovo  *Obiettivo di sostenibilità*, seguire i passaggi:

1. Seleziona l'icona ![lampadina che apre la funzionalità Dimmi](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), Icona, inserisci **Schede di valutazione della sostenibilità**, quindi Seleziona il relativo collegare.
2. Selezionare l'azione  **Obiettivi** per creare un nuovo  **Obiettivo di sostenibilità** per la scorecard selezionata.  
3. Seleziona **Nuovo** per iniziare a creare un nuovo obiettivo.
4. La scheda segnapunti n. **·** Viene aggiunto automaticamente in base al valore della  **Sustainability Scorecard** connessa e l'utente non potrà modificare questo campo. Il sistema imposta anche il campo  **Unità di misura** in base al  **Codice unità di misura emissione** nella pagina  **Impostazione sostenibilità** .  
5. È necessario compilare **n.** e **Nome** del nuovo **Obiettivo di sostenibilità**. Il campo  **Proprietario** viene compilato automaticamente in base al valore della  **Scheda di valutazione della sostenibilità** collegata.   
6. Gli utenti possono decidere di creare un  *Obiettivo di sostenibilità* per l'intera azienda, per un paese/regione specifico o per una struttura. Se gli utenti desiderano creare un obiettivo specifico, devono scegliere il paese o la regione nel campo  **Codice paese/regione** oppure la struttura nel campo  **Centro di responsabilità** .  
7. Seleziona i campi  **Data di inizio** e  **Data di fine** per impostare un periodo dedicato al monitoraggio dei valori correnti. Questa configurazione determina i valori nei seguenti campi: **Valore corrente per CO2**, **Valore corrente per CH4** e **Valore corrente per N2O**. 
8. Seleziona i campi  **Data di inizio della linea di base** e  **Data di fine della linea di base** per impostare un periodo di linea di base dedicato per confrontare i valori correnti. Questa configurazione determina i valori nei seguenti campi: **Linea di base per CO2**, **Linea di base per CH4** e **Linea di base per N2O**.
9. Inoltre, gli utenti possono aggiungere valori target nel campo  **Unità di misura** selezionato per il periodo corrente utilizzando i seguenti campi:  **Valore target per CO2**,  **Valore target per CH4** e  **Valore target per N2O**.   
10. Uno di questi obiettivi può essere selezionato come **Obiettivo principale**. I valori dell'obiettivo principale vengono utilizzati nel centro ruoli del  **Responsabile della sostenibilità** .  

Se hai molti obiettivi nella pagina, puoi usare l'azione  **Mostra i miei obiettivi** per visualizzare solo i tuoi obiettivi; se vuoi visualizzarli tutti, devi eseguire l'azione  **Mostra tutti gli obiettivi** .  

> [!NOTE]
> *Gli obiettivi di sostenibilità* possono essere creati solo per una specifica *Scheda di valutazione della sostenibilità* e non è possibile creare obiettivi non correlati alla scheda di valutazione, ma è possibile creare più obiettivi per una scheda di valutazione. È possibile contrassegnare come  **Obiettivo di sostenibilità** Obiettivo principale **un solo obiettivo.**

> [!NOTE]
> Gli utenti possono impostare diverse combinazioni di obiettivi per l'intera azienda, per specifici paesi o regioni e per un centro di responsabilità per una *Sustainability Scorecard*. Gli utenti possono anche utilizzare periodi diversi per lo stesso modello di tracciamento. 

## Vedere anche

[Setup sostenibilità](finance-sustainability-setup.md)    
[Contabilità generale e piano dei conti di sostenibilità](finance-sustainability-accounts-ledger.md)    
[Come registrare le voci di sostenibilità](finance-sustainability-journal.md)    
[Analisi ad hoc dei dati di sostenibilità](ad-hoc-analysis-sustainability.md)    
[Analisi e report per la sostenibilità in Business Central](sustainability-reports.md)   
[API per la sostenibilità](/dynamics365/business-central/dev-itpro/api-sustainability/sustainability-api?toc=/dynamics365/business-central/toc.json)    
[Finanze](finance.md)    
[Utilizzare [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)    

[!INCLUDE[footer-include](includes/footer-banner.md)]
