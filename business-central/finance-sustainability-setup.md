---
title: Setup sostenibilità
description: Scopri come impostare funzionalità di sostenibilità.
author: altotovi
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'Sustainability, ESG, emission, GHG, CSRD, equivalent, CO2e, CO2, carbon, role center, fees'
ms.search.form: '6221, 6235, 6245'
ms.date: 08/22/2024
ms.author: altotovi
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---

# Impostazione del modulo di sostenibilità 

Prima che il modulo Sostenibilità possa funzionare correttamente, devi impostare alcuni controlli di base e seguire istruzioni di base che sono correlati all'intera funzionalità.

Per impostare un modulo Sostenibilità, segui questi passaggi:

## Centro di ruolo  

Per le persone le cui responsabilità principali riguardano i processi di sostenibilità, si consiglia di utilizzare il centro ruoli  *Responsabile della sostenibilità* . Per configurare questo centro ruoli, seguire seguire i passaggi:  

1. Seleziona l'icona ![lampadina che apre la funzionalità Dimmi](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), Icona, inserisci **Le mie impostazioni**, quindi Seleziona il relativo collegare.
2. Nel campo **Ruolo**, Seleziona la pagina **Ruoli disponibili** .
3. Selezionare la riga  **Responsabile sostenibilità** .
4. Seleziona **OK**.

Il centro di ruolo del  *responsabile della sostenibilità* facilita la gestione efficiente di tutte le aree chiave legate alla sostenibilità. Comprende le principali caratteristiche di sostenibilità, nonché i processi finanziari e di approvvigionamento. Inoltre, fornisce visibilità sui KPI più critici relativi alla sostenibilità.

## Setup sostenibilità  

1. Seleziona l'icona ![lampadina che apre la funzionalità Dimmi](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), e immetti **Setup sostenibilità**, quindi seleziona il collegamento correlato.
2. Nella Scheda dettaglio **Generale**, configura i campi obbligatori che sono correlati al modulo Sostenibilità.

    | Campo | Descrizione |
    |-------|-------------|
    | **Codice unità di misura emissioni** | Specifica il codice dell'unità di misura utilizzato per registrare le emissioni. |
    | **Posizioni decimali emissioni** | Specifica il numero di posizioni decimali che vengono mostrate per gli importi delle emissioni. L'impostazione predefinita, *2:5*, indica che per tutti gli importi vengono mostrati un minimo di due posizioni decimali e un massimo di cinque posizioni decimali. Puoi anche immettere un numero fisso. Ad esempio, se immetti *2*, per tutti gli importi vengono mostrate due posizioni decimali. |
    | **Paese/area geografica obbligatorio** | Specifica se è obbligatorio indicare il paese o l'area geografica. Gli utenti possono impostare il campo Paese/area geografica nei giornali di registrazione anche se non selezioni questo campo. Tuttavia, se lo selezioni, gli utenti dovranno impostare il campo Paese/area geografica prima della registrazione. |
    | **Centro di responsabilità obbligatorio** | Specifica se è obbligatorio indicare il centro di responsabilità. Il centro di responsabilità può essere utilizzato come struttura, cosicché si possa misurare le emissioni basate sulla struttura. Gli utenti possono impostare il campo Centro di responsabilità nei giornali di registrazione anche se non selezioni questo campo. Tuttavia, se lo selezioni, gli utenti dovranno impostare il campo Centro di responsabilità prima della registrazione. |
    | **Modifica della base di calcolo dei blocchi se esistono movimenti contabili** | Specifica se le modifiche alla base di calcolo (formula) a livello di categoria di conto sono bloccate o meno al momento dell'immissione del movimento di sostenibilità, quando la formula è già stata applicata. |
    | **Abilita verifica errori in background** | Specifica se la verifica degli errori in background delle righe di registrazione della sostenibilità è abilitata o meno. |

    > [!NOTE]
    > Dopo che abiliti o disattivi la verifica degli errori in background nelle registrazioni, devi accedere di nuovo prima di avviare la nuova impostazione.

3. Nella scheda dettaglio  **Approvvigionamento**, configura i campi obbligatori relativi all'utilizzo delle funzionalità di sostenibilità nel processo di acquisto.  

    | Campo | Descrizione |
    |-------|-------------|
    | **Utilizzare le emissioni nei documenti di acquisto** | Se si abilita questo campo, nei documenti di acquisto verranno visualizzati campi e funzionalità relativi alla sostenibilità, come ad esempio  **Conto sostenibilità** o emissioni diverse. |

4. Nella Scheda dettaglio **Calcoli**, configura i campi obbligatori che sono correlati alle formule utilizzate per calcolare le emissioni.

    | Campo | Descrizione |
    |-------|-------------|
    | **Posizioni decimali combustibile/elettricità** | Specifica il numero di posizioni decimali che vengono mostrate per gli importi di combustibile/elettricità. L'impostazione predefinita, *2:5*, indica che per tutti gli importi vengono mostrati un minimo di due posizioni decimali e un massimo di cinque posizioni decimali. Puoi anche immettere un numero fisso. Ad esempio, se immetti *2*, per tutti gli importi vengono mostrate due posizioni decimali. |
    | **Posizioni decimali distanza** | Specifica il numero di posizioni decimali che vengono mostrate per le misurazioni della distanza. L'impostazione predefinita, *2:5*, indica che per tutti gli importi vengono mostrati un minimo di due posizioni decimali e un massimo di cinque posizioni decimali. Puoi anche immettere un numero fisso. Ad esempio, se immetti *2*, per tutti gli importi vengono mostrate due posizioni decimali. |
    | **Posizioni decimali importo personalizzato** | Specifica il numero di posizioni decimali che vengono mostrate per gli importi personalizzati. L'impostazione predefinita, *2:5*, indica che per tutti gli importi vengono mostrati un minimo di due posizioni decimali e un massimo di cinque posizioni decimali. Puoi anche immettere un numero fisso. Ad esempio, se immetti *2*, per tutti gli importi vengono mostrate due posizioni decimali. |

5. Nella Scheda dettaglio **Creazione di report**, completa l'impostazione configurando i campi che sono correlati alla creazione di report per le autorità.

    > [!NOTE]
    > Nella versione 24.0, [!INCLUDE[prod_short](includes/prod_short.md)] non supporta la creazione di report per alcuna autorità. Pertanto, i campi che sono correlati alla configurazione di questa funzionalità nella Scheda dettaglio **Creazione di report** sono destinati a funzionalità di reporting future. I partner possono comunque utilizzare questi campi anche nelle versioni localizzate.

    | Campo | Descrizione |
    |-------|-------------|
    | **Codice unità gerarchica di misura delle emissioni** | Specifica il codice dell'unità di misura utilizzato per creare report sulle emissioni, poiché puoi utilizzare un'unità di misura diversa quando crei i report per le autorità. Questo campo non è applicabile ai report standard. |
    | **Creazione report fattore UOM** | Specifica il fattore di unità di misura utilizzato per registrare le emissioni, se utilizzi un'unità di misura diversa quando crei i report per le autorità. |
    | **Approssimazione di arrotondamento delle emissioni** | Specifica le dimensioni dell'intervallo che viene utilizzato nell'arrotondamento degli importi delle emissioni quando crei i report per le autorità. |
    | **Tipo di arrotondamento delle emissioni** | Specifica in che modo il programma arrotonda gli importi delle emissioni quando crei i report per le autorità. Sono disponibili le opzioni seguenti: **Al più vicino**, **Per eccesso** e **Per difetto**. |

## Imposte sulle emissioni   

Per monitorare le tariffe interne sulle emissioni di carbonio o calcolare le emissioni utilizzando gli equivalenti di anidride carbonica (CO2), è necessario configurare la pagina  **Tariffe sulle emissioni** . Per impostare queste informazioni, seguire segui questi passaggi:  

1. Seleziona l'icona ![lampadina che apre la funzionalità Dimmi](media/ui-search/search_small.png "Dimmi cosa vuoi fare"), Icona, inserisci **Commissioni di emissione**, quindi Seleziona il relativo collegare. 
2. Nel campo  **Tipo di emissione**, seleziona l'emissione di gas serra che vuoi configurare: **CO2**, **CH4** o **N2O**. Questa opzione è obbligatoria.   
3. È possibile specificare ulteriormente il **Tipo di ambito**. Se si lascia vuoto questo campo, verrà applicato a tutti gli ambiti, ma è possibile configurarlo per ciascun ambito.  
4. È possibile configurare **Data di inizio** e **Data di fine**. Ciò significa in particolare che è possibile utilizzare configurazioni diverse per periodi diversi. 
5. Il **Codice Paese/Regione** e il **Codice di responsabilità** sono campi facoltativi e puoi scegliere se utilizzarli. Questi campi possono essere utili in quanto è possibile avere tariffe diverse per le emissioni di carbonio a seconda del Paese o utilizzare conversioni diverse della CO2e a seconda del Paese o della struttura (centro di responsabilità).  
6. Il campo  **onere per emissioni di carbonio** rappresenta l'onere per emissioni di carbonio interno che un'azienda addebita a se stessa per ogni unità di CO2 equivalente emessa. Può essere utilizzato in base ad alcune normative locali o regionali, ma anche per calcoli interni. **onere per emissioni di carbonio** verrà calcolato ogni volta che si registrano le emissioni e questa informazione sarà visibile nelle **Voci del registro di sostenibilità**, senza alcuna registrazione aggiuntiva nel **registro contabile**. Puoi impostare  **onere per emissioni di carbonio** per unità di misura presente in  **Configurazione sostenibilità** e può essere compilato solo per la riga in cui il  **Tipo di emissione** è **CO2**. 
7. Il  **fattore di carbonio equivalente** specifica il coefficiente che converte l'impatto di vari gas serra nella quantità equivalente di anidride carbonica in base al loro potenziale di riscaldamento globale. Se il **tipo di emissione** è CO2, il **fattore di carbonio equivalente** sarà sempre *1* e non è possibile modificare questo valore, perché la CO2 è il gas di riferimento utilizzato per calcolare il potenziale di riscaldamento globale (GWP) degli altri gas serra; poiché la CO2 è la base di riferimento, il suo GWP è impostato su *1*. Per altri gas serra, gli utenti devono configurare i valori manualmente. Per effettuare un calcolo corretto, puoi usare il seguente esempio: se assumiamo che 1 chilogrammo di N2O equivale a 298 chilogrammi di CO2, devi calcolare 1/298 e il risultato da popolare sarà 0.00336.  

> [!NOTE]
> **Il campo onere per emissioni di carbonio** nelle **voci del registro di sostenibilità** non verrà calcolato in base ai valori delle **emissioni di CO2** . Invece, come base per questa formula, [!INCLUDE[prod_short](includes/prod_short.md)] utilizzeremo il campo **Emissioni di CO2e** . **Il campo Emissioni di CO2e** verrà calcolato in base a tutte le emissioni registrate all'ingresso e al  **Fattore di carbonio equivalente** configurato per ciascuno dei gas nella pagina  **Commissioni sulle emissioni** .  

Se non hai configurato le  **Commissioni sulle emissioni** prima di pubblicare le voci di sostenibilità e desideri calcolare retroattivamente le tue tariffe sul carbonio e la CO2e, devi eseguire l'azione  **Calcola tariffe sulle emissioni** per aggiornare i valori nelle  **Voci del registro sostenibilità**.  

## Vedere anche

[Finanze](finance.md)    
[Panoramica della gestione della sostenibilità](finance-manage-sustainability.md)    
[Contabilità generale e piano dei conti di sostenibilità](finance-sustainability-accounts-ledger.md)    
[Registrare movimenti di sostenibilità](finance-sustainability-journal.md)    
[Utilizzare [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)    

[!INCLUDE[footer-include](includes/footer-banner.md)]
