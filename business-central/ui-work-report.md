---
title: Eseguire e stampare report in Business Central
description: Informazioni su come inserire un report in una coda processi e programmarlo per l'elaborazione in una data e un'ora specifiche.
author: jswymer
ms.author: jswymer
ms.reviewer: jswymer
ms.topic: conceptual
ms.search.keywords: 'task, process, report, print, schedule, save, Excel, PDF, Word, dataset'
ms.search.form: null
ms.date: 06/13/2024
ms.custom: bap-template
ms.service: dynamics-365-business-central
---

# <a name="run-and-print-reports-in-business-central"></a>Eseguire e stampare report in Business Central

I report ti aiutano a raccogliere e visualizzare dati in base a criteri specifici. Organizza e presenta le informazioni in un formato di facile lettura che puoi stampare o salvare come file. Sono disponibili molti report a cui è possibile accedere dall'applicazione. I report in genere forniscono informazioni relative al contesto della pagina visualizzata. Ad esempio, la pagina **Cliente** include i report per i principali 10 clienti, statistiche di vendita e altro ancora.

> [!NOTE]
> I processi batch e XMLport eseguono più o meno gli stessi report ma sono usati più per elaborare o esportare dati. Ad esempio, il processo batch **Crea solleciti** crea documenti di sollecito da inviare ai clienti con pagamenti scaduti. Questo articolo fa essenzialmente riferimento ai "report" ma informazioni simili si applicano ai processi batch e a XMLport.

## <a name="get-started"></a>Introduzione

Puoi trovare i report nel menu **Report** in pagine, elenchi e schede selezionati. Puoi anche usare la ricerca ![lampadina che apre la funzione Dimmi](media/ui-search/search_small.png "Dimmi cosa vuoi fare"). per individuare i report per nome. Per una panoramica dei report integrati che puoi utilizzare in [!INCLUDE[prod_short](includes/prod_short.md)], ordinati per categorie, vedi [Report disponibili in [!INCLUDE[prod_short](includes/prod_short.md)]](reports-available-reports.md).

Quando scegli un report, viene visualizzata una pagina di richiesta a cui è assegnato il nome del report, in cui imposti varie opzioni e filtri che determinano quali dati sono inclusi. Le sezioni seguenti spiegano come utilizzare la pagina di richiesta per creare, visualizzare in anteprima e stampare un report.

## <a name="use-default-valuesmdashpredefined-settings"></a><a name="SavedSettings"></a>Utilizzare valori predefiniti: impostazioni predefinite

La maggior parte delle pagine di richiesta report include il campo **Utilizza valori predefiniti di**. Questo campo ti consente di selezionare le impostazioni predefinite per il report, che impostano automaticamente opzioni e filtri. Selezionare una voce dall'elenco a discesa per vedere che le opzioni e i filtri nella pagina della richiesta report cambiano di conseguenza.

La voce **Filtri e opzioni utilizzati di recente** è sempre disponibile. Questa voce imposta il report per utilizzare le opzioni e i filtri che hai utilizzato l'ultima volta che è stato eseguito il report.

Il campo **Utilizza valori predefiniti di** fornisce un modo rapido e affidabile per generare costantemente report che contengono i dati corretti. Dopo aver selezionato una voce, è possibile modificare qualsiasi opzione e filtro prima di visualizzare in anteprima o stampare il report. Le modifiche effettuate non verranno salvate nella voce di impostazione predefinita selezionata, ma verranno salvate in **Filtri e opzioni utilizzati più di recente**.

> [!NOTE]
> Le impostazioni predefinite vengono generalmente configurate e gestite da un amministratore. Per ulteriori informazioni, vedi [Gestire impostazioni salvate per report e processi batch](reports-saving-reusing-settings.md).

## <a name="specify-the-data-to-include-in-a-report"></a>Specificare la data da includere in un report

Usa i campi in **Opzioni** e **Filtri** per cambiare o limitare le informazioni che vuoi nel report. È possibile impostare i filtri in un report più o meno nello stesso modo in cui si impostano i filtri negli elenchi. Ulteriori informazioni nella sezione [Filtro](ui-enter-criteria-filters.md#filtering).

> [!CAUTION]
> La scheda dettaglio **Filtro** in una pagina di richiesta report fornisce una generica capacità di filtro per i report. Tali filtri sono facoltativi.
>
> Alcuni report ignorano tali filtri, nel senso che qualsiasi filtro venga impostato nella scheda dettaglio **Filtro**, l'output del report è lo stesso. Non è possibile fornire un elenco dei campi che vengono ignorati in quali report, quindi sarà necessario sperimentare con i filtri quando utilizzati.
>
> **Esempio**: quando si utilizza il processo batch **Crea solleciti**, un filtro per il campo **Movimenti contabili clienti** di **Livello ultimo sollecito emesso** viene ignorato perché i filtri sono fissi per tale processo batch.

## <a name="preview-a-report"></a>Visualizzare in anteprima un report

L'anteprima di un report ti consente di vedere come apparirà il report prima di stamparlo. L'anteprima non è basata sulla stampante selezionata nel campo **Stampante** nella pagina della richiesta. È controllato dal browser. Dopo l'anteprima, puoi tornare alla pagina della richiesta e modificare le opzioni e i filtri come necessario.

Le scelte di anteprima nella pagina **Richiesta report** dipendono dal report. Quindi per alcuni report puoi selezionare **Anteprima**, mentre per altri la scelta è **Anteprima e chiudi**. Entrambe le scelte aprono un'anteprima del report. La differenza è che **Anteprima** mantiene la pagina della richiesta aperta, in modo da potervi tornare, apportare modifiche, visualizzare di nuovo l'anteprima o stampare. Con **Anteprima e chiudi** invece, la pagina di richiesta si chiude e quindi è necessario aprire nuovamente il report per apportare modifiche o stamparlo.

> [!NOTE]
> Se si utilizza il primo ciclo di rilascio di Business Central 2020 o una versione precedente, l'unica scelta disponibile è **Anteprima** che chiude la pagina di richiesta in anteprima, come descritto sopra per **Anteprima e chiudi**.

### <a name="work-with-the-preview"></a>Utilizzare l'anteprima

Nell'anteprima, utilizzare la barra dei menu nell'anteprima del report per:

- Spostarsi tra le pagine
- Ingrandire o ridurre
- Ridimensionare per adattare alla pagina
- Seleziona testo
  
  È possibile copiare il testo di un report e incollarlo altrove, come ad esempio una pagina in [!INCLUDE[prod_short](includes/prod_short.md)] o Microsoft Word. Usando un mouse, ad esempio, tieni premuto il pulsante sinistro del mouse sul punto in cui vuoi iniziare. Quindi sposta il mouse per selezionare una o più parole, frasi o paragrafi. Premi il pulsante destro del mouse e seleziona **Copia**. Ora puoi incollare il testo selezionato nella posizione desiderata.

- Panoramica del documento
  
  È possibile spostare l'area visibile del report in qualsiasi direzione in modo da poter visualizzare altre aree del report. La panoramica risulta utile quando hai eseguito l'ingrandimento per visualizzare i dettagli. Ad esempio, tieni premuto il pulsante sinistro del mouse su un punto dell'anteprima del report, quindi sposta il mouse per selezionare una sezione del report.

- Scaricare in un file PDF sul computer o in rete.
- Stampa

## <a name="save-a-report-to-a-file"></a>Salvare un report in un file

Puoi salvare un report in un documento PDF, un documento di Microsoft Word, una cartella di lavoro di Microsoft Excel o un documento XML scegliendo **Invia a** ed effettuando la scelta desiderata. Il file viene scaricato nel computer.

Se la tua organizzazione ha configurato OneDrive per le funzionalità di sistema, invece di essere scaricati, le cartelle di lavoro di Excel e i documenti di Word vengono aperti nel browser utilizzando Excel o Word per il Web.

> [!TIP]
> Le opzioni **Documento Microsoft Excel (solo dati)** e **Documento XML** sono principalmente per scopi avanzati. In genere utilizzi queste opzioni per eseguire analisi dettagliate dei dati. Per informazioni vedi [Analisi dei dati del report con Excel e XML](report-analyze-excel.md).
>
> Puoi anche usare l'opzione **Documento Microsoft Excel (solo dati)** per creare nuovi layout di Excel per un determinato report. Per ulteriori informazioni, vedi [Utilizzare i layout di Excel](ui-excel-report-layouts.md).  

## <a name="schedule-a-report-to-run-later-or-periodically"></a><a name="ScheduleReport"></a>Pianificare un report da eseguire in seguito o periodicamente

È possibile pianificare l'esecuzione singola o ricorrente di un report a una data e un'ora specifiche. I report previsti vengono inseriti nella coda commesse e vengono elaborati all'orario pianificato, in maniera analoga alle altre commesse. Seleziona l'opzione **Programmazione** dopo aver scelto il pulsante **Invia a**, quindi immetti le informazioni quali stampante, ora e data. Il report viene aggiunto alla coda processi e viene eseguito alla data specificata. Quando il report viene elaborato, l'elemento viene rimosso dalla coda processi. Per ulteriori informazioni, vedi [Utilizzare le code processi per pianificare le attività](admin-job-queues-schedule-tasks.md).  

Quando pianifichi l'esecuzione di un report, puoi specificare ad esempio che deve essere eseguito ogni giovedì impostando il campo **Prossima esecuzione formula della data** su *D4*. Per ulteriori informazioni, vedi la sezione [Utilizzare le formule per le date](ui-enter-date-ranges.md#use-date-formulas).  

Puoi salvare il report in un file, ad esempio un file Excel, Word, PDF, o stamparlo, o solo generare il report. Se salvi il report in un file, il report elaborato viene inviato nella pagina **Report elaborati** della Gestione ruolo utente, dove puoi visualizzarlo. Per ulteriori informazioni, vedi [Condividere ed esportare report con Report elaborati](ui-work-report-inbox.md)

### <a name="manage-scheduled-recurring-reports"></a>Gestire i report ricorrenti programmati

I processi batch generano report programmati gestiti nella pagina **Movimenti coda processi**. Puoi visualizzare lo stato e altre informazioni per ciascun report nella pagina, sospendere/riprendere il processo batch del report e generare il report su richiesta.

Dalla pagina **Movimenti coda processi** puoi anche modificare alcuni parametri del report, come il tipo di file di output, la ricorrenza, la data di esecuzione e gli orari di inizio e fine. Prima di modificare un report programmato esistente, tuttavia, è necessario mettere in attesa la coda processi del report:

1. Seleziona l'icona ![lampadina che apre la funzionalità Dimmi 1.](media/ui-search/search_small.png "Dimmi cosa vuoi fare") immetti **Movimenti coda processi**, quindi seleziona il collegamento correlato.  
2. Nella pagina **Movimenti coda processi**, seleziona il report desiderato.
3. Seleziona l'azione **Imposta in sospeso**.
4. Apri e modifica il report pianificato selezionando il suo stato (*In attesa*).

Dopo aver modificato le opzioni del report, ripeti i primi due passaggi e seleziona l'azione **Imposta stato su Pronto** per riprendere la generazione del report.

Ulteriori informazioni sulla gestione della coda processi in [Usare le code processi per pianificare le attività](admin-job-queues-schedule-tasks.md).  

## <a name="print-a-report"></a><a name="PrintReport"></a>Stampare un report

Per stampare un report seleziona **Stampa** nella pagina di richiesta report o nella barra dei menu della pagina **Anteprima**.

Quando un report utilizza un layout di Excel, non vedrai il campo **Stampante**, il pulsante **Stampa** o **Anteprima**. C'è invece un'opzione **Scarica**. Per stampare, seleziona **Scarica**, quindi apri il file scaricato in Excel e stampa da lì.

### <a name="printer"></a><a name="Printer"></a>Stampante

Il campo **Stampante** nella pagina di richiesta del report mostra il nome della stampante a cui viene inviato il report. Per cambiare una stampante, seleziona semplicemente la stampante dall'elenco.

> [!NOTE]
> L'opzione **(Gestito dal browser)** indica che non esiste una stampante designata per il report. In questo caso, il browser gestisce la stampa e visualizza i passaggi di stampa standard, in cui è possibile scegliere una stampante locale collegata al computer. L'opzione **(Gestito dal browser)** non è disponibile nell'app per dispositivi mobili [!INCLUDE[prod_short](includes/prod_short.md)] o nell'app per Microsoft Teams.

> [!TIP]
> La stampante selezionata per impostazione predefinita è configurata nella pagina **Selezioni della stampante**. Per ulteriori informazioni su come modificare la stampante predefinita, vedi la sezione [Configurare le stampanti predefinite](ui-specify-printer-selection-reports.md#default).

### <a name="print-reports-in-thai"></a>Stampare report in tailandese

Nella versione tailandese di [!INCLUDE[prod_short](includes/prod_short.md)], non è possibile stampare correttamente i report con il pulsante **Stampa** a causa delle limitazioni nel servizio che genera il file PDF stampabile. In alternativa, è possibile aprire il report in Word e quindi salvare il report come PDF stampabile.  

Oppure è possibile richiedere all'amministratore di creare un layout report Word per i report più utilizzati. Per ulteriori informazioni, vedi [Gestione dei layout di report e documento](ui-manage-report-layouts.md).  

## <a name="switch-the-report-layout"></a>Cambiare il layout di report

Un layout di report determina le informazioni che verranno visualizzate nel report, nonché la disposizione e l'aspetto delle stesse. La modifica del layout può essere effettuata in vari modi:

- Quando stai configurando per eseguire un report, vedrai il layout corrente nel campo **Layout report** nella pagina della richiesta. Per passare temporaneamente a un layout diverso, seleziona il campo **Layout report**, quindi seleziona da un elenco di layout disponibili per il report.
- Per modificare il layout predefinito utilizzato da un report, vai nelle pagine **Layout report** o **Selezione layout report**.

Per ulteriori informazioni, vedi [Impostare il layout utilizzato da un report](ui-set-report-layout.md). Oppure per personalizzare un layout di report, vedi [Iniziare a creare layout](ui-get-started-layouts.md).

## <a name="change-language-and-format-of-numbers-dates-and-times"></a>Cambiare la lingua e il formato di numeri, date e orari

Per impostazione predefinita, la lingua del testo e il formato di numeri, date e orari in un report si basano sulla lingua di lavoro e sulle impostazioni della regione, definite nella pagina **Impostazioni personali**. È tuttavia possibile modificare caso per caso la lingua e la regione del formato durante l'anteprima, la stampa o l'invio di un report. Nella pagina della richiesta, imposta le opzioni **Lingua** e **Formato area geografica** come necessario. Puoi anche specificare la lingua e il formato dell'area geografica da utilizzare per impostazione predefinita per clienti e fornitori nelle pagine schede.

A seconda di dove hai specificato le impostazioni relative a lingua e formato, [!INCLUDE [prod_short](includes/prod_short.md)] determina le impostazioni da utilizzare nel seguente ordine:

1. Le impostazioni che specifichi quando generi un report.
2. Le impostazioni che hai specificato nel documento, che provengono dalle impostazioni relative al cliente o al fornitore.
3. Le impostazioni specificate nell'oggetto Report AL.
4. Le impostazioni definite in Impostazioni personali.

Per ulteriori informazioni sulla pagina **Impostazioni personali** vedi [Modificare le impostazioni di base](ui-change-basic-settings.md#region).

## <a name="advanced-options"></a>Opzioni avanzate

I campi nella scheda dettaglio **Avanzate** impostano le limitazioni sul report generato per controllare le risorse della stampante. In genere non è necessario modificare queste impostazioni, a meno che il report non sia di grandi dimensioni. Se un report supera questi limiti quando si tenta di visualizzarlo in anteprima o stamparlo, viene indicato quale limite è stato superato. È quindi possibile modificare le impostazioni per adattarle al report. Ogni campo, tuttavia, ha un valore massimo che è necessario conoscere:

|Campo|Valore massimo|
|-----|-------------|
|Tempo massimo di rendering|12:00:00|
|Numero massimo di righe|1000000|
|Numero massimo documenti|500|

> [!NOTE]
> I valori massimi possono essere diversi per [!INCLUDE[prod_short](includes/prod_short.md)] in locale e un amministratore può modificarli. Per ulteriori informazioni, vedi [Configurazione di Business Central Server - Report](/dynamics365/business-central/dev-itpro/administration/configure-server-instance#Reports). Per una panoramica dei limiti dei report in [!INCLUDE[prod_short](includes/prod_short.md)] online, vedi [Limiti operativi](/dynamics365/business-central/dev-itpro/administration/operational-limits-online).

## <a name="see-also"></a>Vedere anche

- [Report disponibili in [!INCLUDE[prod_short](includes/prod_short.md)]](reports-available-reports.md)  
- [Usare i report nel lavoro quotidiano](reports-use-reports.md)  
- [Panoramica di Business Intelligence e creazione di report](reports-bi-reporting.md)  
- [Configurare le stampanti](ui-specify-printer-selection-reports.md)  
- [Eseguire processi batch e XMLports](ui-how-run-batch-jobs.md)  
- [Utilizzare date e orari del calendario](ui-enter-date-ranges.md)  
- [Gestione dei layout di report e documenti](ui-manage-report-layouts.md)  
- [Business Intelligence finanziario](bi.md)  
- [Utilizzare [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
