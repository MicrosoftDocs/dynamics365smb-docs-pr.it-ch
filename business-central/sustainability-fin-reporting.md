---
title: Sostenibilità Creazione di report finanziari
description: Descrive come utilizzare i report finanziari per creare diverse visualizzazioni e report per l'analisi dei dati sulle prestazioni di sostenibilità.
author: altotovi
ms.topic: conceptual
ms.search.keywords: reporting
ms.search.form: '104, 108, 490'
ms.date: 08/22/2024
ms.author: altotovi
ms.service: dynamics-365-business-central
---

# <a name="analyzing-sustainability-entries-with-financial-reports"></a>Analisi delle voci di sostenibilità con i report finanziari

La funzionalità *Report finanziari*  fornisce informazioni dettagliate sui dati finanziari visualizzati nel piano dei conti (COA). Puoi configurare i report finanziari per analizzare le cifre nei conti di contabilità generale (C/G) e confrontare i movimenti di contabilità generale con i movimenti di budget. Ma è anche possibile analizzare dati statistici e di sostenibilità con la stessa funzione e persino combinare tutti e tre i tipi di dati.  

## <a name="prerequisites-for-financial-reporting"></a>Prerequisiti per il reporting finanziario

Per impostare report finanziari è necessario comprendere la struttura dei dati che si desidera analizzare. Ci sono alcuni concetti chiave a cui probabilmente dovresti prestare attenzione prima di progettare i tuoi report finanziari: 

1. Relativo al piano dei conti: 
   1. Mappare i conti registrazione C/G alle categorie di conti C/G. 
   2. Progettare il modo in cui utilizzi le dimensioni.
   3. Impostare i budget budget C/G.  
2. Relativo alla Sostenibilità:   
   1. Imposta i tuoi account di sostenibilità. 
   2. Imposta le tue tariffe sul carbonio e sulla CO2e nella sezione Tariffe sulle emissioni **.**
   3. Progettare il modo in cui utilizzi le dimensioni.  
3. Relativamente ai Conti statistici: 
   1. Imposta i tuoi account statistici. 
   2. Progettare il modo in cui utilizzi le dimensioni.  

> [!NOTE]
> I report finanziari non tengono conto direttamente delle emissioni di CO2, CH4 o N2O. Invece, utilizza il modello di CO2 equivalente e ciò significa che devi prima configurare **CO2e** (anidride carbonica equivalente) nella pagina **Commissioni sulle emissioni** .  

> [!NOTE]
> Per maggiori dettagli sull'utilizzo dei report finanziari con dati finanziari e piano dei conti, clicca qui [Creazione di report finanziari utilizzando dati finanziari e categorie di conti](bi-how-work-account-schedule.md).   

## <a name="create-a-new-financial-report"></a>Creare un nuovo report finanziario

Per creare rapidamente i propri report finanziari, è possibile iniziare copiando un report finanziario esistente, come descritto al passaggio 3 di seguito. 

1. Scegli l'icona ![lampadina che apre la funzione Dimmi 1.](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immetti **Report finanziari**, quindi scegli il collegamento correlato.  
2. Sulla pagina **Report finanziari** scegli l'azione **Nuovo** per creare un nuovo nome per il report finanziario.  
3. Inserisci il nome breve del report nel campo  **Nome** (non potrai più modificare il nome in seguito) e inserisci  **Descrizione**.  
4. Scegli una definizione di riga e una definizione di colonna.   
5. Selezionare l'azione **Modifica definizione di report** per accedere ad altre proprietà nel report finanziario.  
6. Nella Scheda dettaglio **Opzioni** puoi modificare la descrizione del report, modificare le definizioni di riga e di colonna e definire come visualizzare le date. Le date possono essere una gerarchia Giorno/Settimana/Mese/Trimestre/Anno oppure utilizzare periodi contabili. Per saperne di più, vedi [Confronto dei periodi contabili con le formule periodo](bi-column-definitions.md#comparing-accounting-periods-using-period-formulas) 
7. Nella Scheda dettaglio **Dimensioni** puoi definire i filtri dimensioni per il report.  
8. Puoi visualizzare l'anteprima del report nell'area sotto la Scheda dettaglio **Dimensioni**.   

Se vuoi analizzare i tuoi dati statistici o di sostenibilità, puoi farlo impostando  **definizione di riga**.  

Per creare o modificare un definizione di riga, seguire procedere come segue:

1. Nella pagina **Report finanziari** seleziona il report finanziario pertinente e quindi scegli l'azione **Modifica definizione riga**. 
2. Impostare le righe come nei passaggi seguenti.  

> [!NOTE]
> Il campo **Nr. riga** mostra i primi 10 caratteri di un identificatore, ad esempio un numero di conto. Se aggiungi elementi con identificatori che iniziano con gli stessi 10 caratteri, avrai duplicati nel campo **Nr. riga** . Se necessario, puoi modificare manualmente gli identificatori dopo aver inserito gli elementi. Gli identificatori completi vengono visualizzati nel campo **Totale**.

> [!NOTE]
> È possibile combinare tutti i **tipi di totale**, ovvero conti di registrazione, conti di sostegno. Conti, Conto Statistico.

> [!NOTE]
> Le definizioni di riga non hanno una versione. Quando modifichi un definizione di riga, la vecchia versione viene sostituita e le modifiche vengono salvate nel database. 

### <a name="analyzing-sustainability-data"></a>Analisi dei dati sulla sostenibilità

1. Inserisci il numero di riga. **·** Per identificare i dati grezzi e aggiungere **Descrizione** come testo che apparirà sulla riga del report finanziario. 
2. Nella colonna Tipo di totale, seleziona l'opzione  **Conti di mantenimento** .   
3. Nel campo Totale, seleziona uno o più account di sostenibilità utilizzando tutti i filtri applicabili. 
4. Nel **Tipo di importo** scegli una delle opzioni:   
   1. **CO2e** se si desidera segnalare il valore equivalente di CO2 dal campo **Emissioni di CO2e** nelle **Voci del registro sostenibilità**. 
   2. **Commissione sul carbonio** se si desidera segnalare l'equivalente finanziario (commissione sul carbonio) dal campo **Commissione sul carbonio** nelle **Voci del registro di sostenibilità**. 
5. Se si sceglie **Formula** come **Tipo di totale**, è possibile utilizzare formule matematiche nella colonna **Totale** .  

### <a name="analyzing-statistical-data"></a>Analisi dei dati statistici

1. Inserisci il numero di riga. **·** Per identificare la riga e aggiungere **Descrizione** come testo che apparirà sulla riga del report finanziario. 
2. Nella colonna **Tipo di totale**, seleziona l'opzione **Conti statistici** .   
3. Nel campo  **Totale**, seleziona uno o più account di sostenibilità utilizzando tutti i filtri applicabili. 
4. Se si sceglie **Formula** come **Tipo di totale**, è possibile utilizzare formule matematiche nella colonna **Totale** .  

## <a name="see-also"></a>Vedere anche

[Panoramica sulla gestione della sostenibilità](finance-manage-sustainability.md)    
[Analisi e report per la sostenibilità in Business Central](sustainability-reports.md)   
[API per la sostenibilità](/dynamics365/business-central/dev-itpro/api-sustainability/sustainability-api?toc=/dynamics365/business-central/toc.json)    
[Preparare Creazione di report finanziari](bi-how-work-account-schedule.md)    
[definizione di riga in Creazione di report finanziari](bi-row-definitions.md)    
[definizione di colonna nel Creazione di report finanziari](bi-column-definitions.md)    
[Finanze](finance.md)    
[Utilizzare [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)    

[!INCLUDE[footer-include](includes/footer-banner.md)]
