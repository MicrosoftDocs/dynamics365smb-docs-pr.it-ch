---
title: Data di registrazione dei movimenti di valorizzazione
description: Informazioni su come il processo batch Rettifica costo - Movimenti articoli identifica e assegna una data di registrazione ai movimenti di valorizzazione che il processo batch crea.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 06/08/2021
ms.author: edupont
ms.openlocfilehash: 918a450ea40676447f872ba95eb489c7cc210211
ms.sourcegitcommit: 0953171d39e1232a7c126142d68cac858234a20e
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 06/09/2021
ms.locfileid: "6215121"
---
# <a name="design-details-posting-date-on-adjustment-value-entry"></a>Dettagli di progettazione: Data di registrazione del movimento di valorizzazione della rettifica
In questo articolo vengono fornite informazioni per gli utenti della funzionalità Magazzino e costing di [!INCLUDE[prod_short](includes/prod_short.md)]. L'articolo fornisce informazioni su come il processo batch **Rettifica costo - Movimenti articoli** identifica e assegna una data di registrazione ai movimenti di valorizzazione che il processo batch crea.  

Innanzitutto viene esaminato il concetto del processo, il modo in cui il processo batch identifica e assegna la data di registrazione al movimento di valorizzazione da creare. Vengono descritti alcuni scenari in cui il team di supporto si è a volte imbattuto e infine viene mostrato un riepilogo dei concetti utilizzati.  

## <a name="the-concept"></a>Concetto  
Il processo batch **Rettifica costo - Movimenti articoli** assegna una data di registrazione al movimento valorizzazione da creare mediante la seguente procedura:  

1.  Inizialmente la data di registrazione del movimento da creare è la stessa data del movimento che viene rettificato.  

2.  La data di registrazione viene convalidata in base ai periodi di magazzino e/o al setup di contabilità generale.  

3.  Assegnazione della data di registrazione; se la data di registrazione iniziale non rientra nell'intervallo di date di registrazione consentite, il processo batch assegnerà una data di registrazione consentita in base al periodo di magazzino o al setup di contabilità generale. Se i periodi di magazzino e le date di registrazione consentite nel setup di contabilità generale sono definiti, la data più lontana delle due verrà assegnata al movimento di valorizzazione della rettifica.  

 Esaminiamo questo processo con un esempio pratico. Supponiamo di avere un movimento contabile articolo di vendita. L'articolo è stato spedito il 5 settembre 2013 ed è stato fatturato il giorno dopo.  

![Stato dei movimenti contabili articolo nello scenario](media/helene/TechArticleAdjustcost1.png "Stato dei movimenti contabili articolo nello scenario")  

Nell'illustrazione seguente, il primo movimento di valorizzazione (379) indica la spedizione e ha la stessa data di registrazione del movimento contabile articolo padre.  

Il secondo movimento di valorizzazione (381) rappresenta la fattura.  

 Il terzo movimento di valorizzazione (391) è una rettifica del movimento di valorizzazione di fatturazione (381).  

 ![Stato dei movimenti valorizzazione nello scenario](media/helene/TechArticleAdjustcost2.png "Stato dei movimenti valorizzazione nello scenario")  

 Passaggio 1: al movimento di valorizzazione della rettifica da creare è assegnata la stessa data di registrazione del movimento che viene rettificato, illustrato sopra dal movimento di valorizzazione 391.  

 Passaggio 2: convalida della data di registrazione assegnata iniziale.  

Il processo batch **Rettifica costo - Movimenti articoli** determina se la data di registrazione iniziale del movimento di valorizzazione della rettifica rientra nell'intervallo di date consentite basato sui periodi di magazzino e/o sul setup di contabilità generale.  

 Esaminiamo la vendita menzionata in precedenza aggiungendo il setup dell'intervallo di date di registrazione consentite.  

 Periodi di magazzino:  

![Periodi di magazzino nello scenario](media/helene/TechArticleAdjustcost3.png "Periodi di magazzino nello scenario")

 La prima data di registrazione consentita è il primo giorno del primo periodo aperto. 1 settembre 2013.  

 Setup contabilità generale:  

![Configurazione C/G nello scenario](media/helene/TechArticleAdjustcost4.png "Configurazione C/G nello scenario")

 La prima data di registrazione consentita è la data indicata nel campo Consenti registraz. da: 10 settembre 2013.  

 Se i periodi di magazzino e le date di registrazione consentite nel setup di contabilità generale sono definiti, la data più lontana delle due definirà l'intervallo di date di registrazione consentite.  

 Passaggio 3: assegnazione di una data di registrazione consentita;  

 La data di registrazione assegnata iniziale era il 6 settembre come illustrato nel passaggio 1. Tuttavia, nel secondo passaggio il processo batch Rettifica costo - Movimenti articoli identifica che la data di registrazione consentita più vicina è il 10 settembre e pertanto assegna il 10 settembre al movimento di valorizzazione della rettifica, come illustrato di seguito.  

 ![Stato dei movimenti valorizzazione nello scenario 2](media/helene/TechArticleAdjustcost5.png "Stato dei movimenti valorizzazione nello scenario 2")

 Qui termina la descrizione del concetto per l'assegnazione di date di registrazione a movimenti di valorizzazione creati mediante il processo batch Rettifica costo - Movimenti articoli.  

 Esaminiamo ora alcuni scenari in cui il team di supporto si è a volte imbattuto riguardanti le date di registrazione assegnate nel processo batch Rettifica Costo – Movimenti articoli e i relativi setup .  

## <a name="scenarios"></a>Scenari  

### <a name="scenario-i-posting-date-is-not-within-your-range-of-allowed-posting-dates"></a>Scenario I: "la data di registrazione non è compresa nell'intervallo di date di registrazione consentite....".  
 Questo è uno scenario in cui un utente riceve il suddetto messaggio di errore durante il processo batch Rettifica costo - Movimenti articoli.  

 Nella descrizione del concetto di assegnazione di date di registrazione vista nella sezione precedente, lo scopo del processo batch Rettifica costo – Movimenti articoli è creare un movimento di valorizzazione con il 10 settembre come data di registrazione.  

![Messaggio di errore sulla data di registrazione](media/helene/TechArticleAdjustcost6.png "Messaggio di errore sulla data di registrazione")

 Continuiamo con il setup utente:  

![Configurazione delle date di registrazione consentite dell'utente](media/helene/TechArticleAdjustcost7.png "Configurazione delle date di registrazione consentite dell'utente")

 L'utente in questo caso ha un intervallo di date di registrazione consentite dall'11 settembre al 30 settembre e pertanto non gli è consentito registrare il movimento di valorizzazione della rettifica con il 10 settembre come data di registrazione.  

![Panoramica della configurazione della data di registrazione coinvolta](media/helene/TechArticleAdjustcost8.png "Panoramica della configurazione della data di registrazione coinvolta")

 L'articolo della Knowledge Base [952996](https://mbs2.microsoft.com/Knowledgebase/kbdisplay.aspx?WTNTZSMNWUKNTMMYXUPYZQPOUXNXSPSYOQQYYMLUQLOYYMWP) esamina più scenari relativi al messaggio di errore citato.  

### <a name="scenario-ii-posting-date-on-adjustment-value-entry-versus-posting-date-on-entry-causing-the-adjustment-such-as-revaluation-or-item-charge"></a>Scenario II: la data di registrazione del movimento di valorizzazione della rettifica rispetto alla data di registrazione del movimento origina la rettifica come rivalutazione o addebito articolo.  

### <a name="revaluation-scenario"></a>Scenario di rivalutazione:  
 Prerequisiti:  

 Setup magazzino:  

-   Reg. automatica costi = Sì  

-   Rettifica costo automatica=Sempre  

-   Tipo calcolo costo medio=articolo  

-   Costo medio periodo=Giorno  

 Setup contabilità generale:  

-   Consenti registraz. da = 1° gennaio 2014  

-   Consenti registrazioni fino a = vuoto  

 Setup utente:  

-   Consenti registraz. da = 1° dicembre 2013  

-   Consenti registrazioni fino a = vuoto  

##### <a name="to-test-the-scenario"></a>Per verificare lo scenario:  

1.  Creare TEST articolo:  

     Unità di misura base = PZ  

     Metodo di costing = Media  

     Selezionare categorie di registrazione facoltative.  

2.  Aprire le registrazioni magazzino, creare e registrare una riga come segue:  

     Data di registrazione = 15 dicembre 2013  

     Articolo = TEST  

     Tipo movimento = Acquisto  

     Quantità = 100  

     Importo unitario = 10  

3.  Aprire le registrazioni magazzino, creare e registrare una riga come segue:  

     Data = 20 dicembre 2013  

     Articolo = TEST  

     Tipo movimento = Rettifica negativa  

     Quantità = 2  

4.  Aprire le registrazioni magazzino, creare e registrare una riga come segue:  

     Data = 15 gennaio 2014  

     Articolo = TEST  

     Tipo movimento = Rettifica negativa  

     Quantità = 3  

5.  Aprire le registrazioni rivalutazioni, creare e registrare una riga come segue:  

     Articolo = TEST  

     Collega-a movimento = selezionare il movimento di tipo Acquisto registrato nel passaggio 2. La data di registrazione della rivalutazione sarà la stessa del movimento che rettifica.  

     Costo unitario (rivalutato) = 40  

 I seguenti movimenti contabili articoli e di valorizzazione sono stati registrati:  

![Panoramica dei movimenti di valorizzazione e contabili articolo 1](media/helene/TechArticleAdjustcost9.png "Panoramica dei movimenti di valorizzazione e contabili articolo 1")

 ![Panoramica dei movimenti di valorizzazione e contabili articolo 2](media/helene/TechArticleAdjustcost10.png "Panoramica dei movimenti di valorizzazione e contabili articolo 2")

 Il processo batch Rettifica costo - Movimenti articoli ha riconosciuto una variazione nel costo e rettificato le rettifiche negative.  

 **Analisi delle date di registrazione dei movimenti di valorizzazione delle rettifiche creati:** la data di registrazione consentita più vicina a cui il processo batch Rettifica costo - Movimenti articoli deve fare riferimento è il 1° gennaio 2014 come indicato nel setup di contabilità generale.  

 **Rettifica negativa nel passaggio 3:** la data di registrazione assegnata è il 1° gennaio, fornita dal setup di contabilità generale. La data di registrazione del movimento di valorizzazione in relazione alla rettifica è il 20 dicembre 2013. Secondo il setup contabilità generale la data non rientra nell'intervallo di date di registrazione consentite. Di conseguenza, la data di registrazione indicata nel campo Consenti registraz. da nel setup di contabilità generale è assegnata al movimento di valorizzazione della rettifica.  

 **Rettifica negativa nel passaggio 4:** la data di registrazione assegnata è il 15 gennaio. La data di registrazione del movimento di valorizzazione in relazione alla rettifica è il 15 gennaio, che rientra nell'intervallo di date di registrazione consentite secondo il setup di contabilità generale.  

 La rettifica apportata per la rettifica negativa nel passaggio 3 è oggetto di discussione. La data di registrazione favorevole del movimento di valorizzazione della rettifica sarebbe stata il 20 dicembre o almeno in dicembre in quanto la rivalutazione che causa la modifica in COGS è stata registrata in dicembre.  

 Per eseguire la rettifica negativa nel passaggio 3 in dicembre, la data indicata nel campo Consenti registraz. da del setup di contabilità generale deve essere in dicembre.  

 **Conclusione:**  

 Sulla base delle esperienze relative a questo scenario, considerando il setup più appropriato dell'intervallo di date di registrazione consentite per un'azienda, potrebbe essere utile considerare le seguenti informazioni: fino a che è consentito registrare le modifiche apportate al valore di magazzino in un periodo, dicembre in questo caso, il setup utilizzato dall'azienda per gli intervalli di date di registrazione consentite deve essere allineato a questa decisione. Il campo Consenti registraz. da nel setup di contabilità generale, indicante il 1° dicembre, permetterebbe il trasferimento della rivalutazione effettuata a dicembre ai movimenti in uscita interessati nello stesso periodo.  

 Per i gruppi di utenti a cui non è consentito registrare in dicembre ma a gennaio, condizione probabilmente determinata dal setup di contabilità generale in questo scenario, si deve utilizzare il setup utente.  

### <a name="item-charge-scenario"></a>Scenario con addebito articolo:  
 Prerequisiti:  

 Setup magazzino:  

-   Reg. automatica costi = Sì  

-   Rettifica costo automatica=Sempre  

-   Tipo calcolo costo medio=articolo  

-   Costo medio periodo=Giorno  

 Setup contabilità generale:  

-   Consenti registraz. da = 1° dicembre 2013  

-   Consenti registrazioni fino a = vuoto  

 Setup utente:  

-   Consenti registraz. da = 1° dicembre 2013  

-   Consenti registrazioni fino a = vuoto  

##### <a name="to-test-the-scenario"></a>Per verificare lo scenario:  

1.  Creare un addebito articolo:  

     Unità di misura base = PZ  

     Metodo di costing = Media  

     Selezionare categorie di registrazione facoltative.  

2.  Creare un nuovo ordine di acquisto  

     Acquistare da - Nr. for.: 10000  

     Data di registrazione = 15 dicembre 2013  

     Nr. fattura fornitore: 1234  

     Nella riga ordine di acquisto:  

     Articolo = ADDEBITO  

     Quantità = 1  

     Costo unitario diretto = 100  

     Registrare carico e fattura.  

3.  Creare un nuovo ordine di vendita:  

     Vendere a - Nr. cliente: 10000  

     Data di registrazione = 16 dicembre 2013  

     Nella riga dell'ordine di vendita:  

     Articolo = ADDEBITO  

     Quantità = 1  

     Prezzo unitario = 135  

     Registrare spedizione e fattura.  

4.  Setup contabilità generale:  

     Consenti registraz. da = 1° gennaio 2014  

     Consenti registrazioni fino a = vuoto  

5.  Creare un nuovo ordine di acquisto:  

     Acquistare da - Nr. for.: 10000  

     Data di registrazione = 2 gennaio 2014  

     Nr. fattura fornitore: 2345  

     Nella riga ordine di acquisto:  

     Addebito articolo = COM-SPEDIZ  

     Quantità = 1  

     Costo unitario diretto = 3  

     Assegnare l'addebito articolo al carico di acquisto del passaggio 2.  

     Registrare carico e fattura.  

     ![Panoramica dei movimenti di valorizzazione e contabili articolo 3](media/helene/TechArticleAdjustcost11.png "Panoramica dei movimenti di valorizzazione e contabili articolo 3")

6.  In data 3 gennaio arriva una fattura di acquisto contenente un ulteriore addebito articolo per l'acquisto effettuato nel passaggio 2. La data documento di questa fattura è il 30 dicembre e pertanto viene registrata con la data 30 dicembre 2013.  

     Creare un nuovo ordine di acquisto:  

     Acquistare da - Nr. for.: 10000  

     Data di registrazione = 30 dicembre 2013  

     Nr. fattura fornitore: 3456  

     Nella riga ordine di acquisto:  

     Addebito articolo = COM-SPEDIZ  

     Quantità = 1  

     Costo unitario diretto = 2  

     Assegnare l'addebito articolo al carico di acquisto del passaggio 2.  

     Registrare carico e fattura.  

   ![Panoramica dei movimenti di valorizzazione e contabili articolo 4](media/helene/TechArticleAdjustcost12.png "Panoramica dei movimenti di valorizzazione e contabili articolo 4")

 Il report Valutazione magazzino viene stampato in data 31 dicembre 2013  

![Contenuto del report di valutazione magazzino](media/helene/TechArticleAdjustcost13.png "Contenuto del report di valutazione magazzino")

 **Riepilogo dello scenario:**  

 Lo scenario descritto termina con un report Valutazione magazzino che indica Quantità = 0 quando Valore = 2. L'addebito articolo registrato nel passaggio 11 fa parte del valore Aumento di magazzino di dicembre mentre la riduzione di magazzino dello stesso periodo non è influenzata.  

 La data 1° gennaio indicata nel campo Consenti registraz. da del setup di contabilità generale era ideale per il primo addebito articolo. I costi dell'aumento e della riduzione di magazzino sono stati registrati nello stesso periodo. Per il secondo addebito articolo tuttavia, il setup di contabilità generale posiziona la modifica in COGS nel periodo successivo.  

 **Conclusione:**  

 È una sfida dimostrare nel report Valutazione magazzino che Quantità = 0 quando Valore <> 0. In questo caso è anche più difficile indicare le impostazioni ottimali, in quanto le fatture di acquisto arrivano lo stesso giorno ma fanno riferimento a periodi o persino anni fiscali differenti. Il passaggio a un nuovo anno fiscale richiede normalmente una pianificazione e in tale ambito le informazioni relative al processo Rettifica costo - Movimenti articoli, che riconosce COGS, devono essere prese in considerazione.  

 Come alternativa in questo scenario si sarebbe potuto avere una data in dicembre di un paio di giorni in più nel campo Consenti registraz. da del setup di contabilità generale e differire la registrazione del primo addebito articolo per consentire il riconoscimento di tutti i costi relativi al periodo/anno fiscale per il periodo a cui appartengono inizialmente, quindi eseguire il processo batch Rettifica costo - Movimenti articoli e infine spostare la data di registrazione consentita al nuovo periodo\/anno fiscale. Si sarebbe quindi potuto registrare il primo addebito con la data 2 gennaio.  

## <a name="history-of-adjust-cost--item-entries-batch-job"></a>Cronologia del processo batch Rettifica costo - Movimenti articoli  
 Di seguito è riportato un riepilogo del concetto che assegna date di registrazione ai movimenti di valorizzazione delle rettifiche mediante il processo batch Rettifica costo – Movimenti articoli.  

### <a name="about-the-request-form-posting-date"></a>Informazioni sulla data di pubblicazione del form di richiesta:  
 Non è più necessario indicare una data di registrazione nel modulo di richiesta del processo batch Rettifica costo - Movimenti articoli. Il processo batch esamina tutte le modifiche necessarie e crea movimenti di valorizzazione con la data di registrazione del movimento di valorizzazione che rettifica. Se la data di registrazione non rientra nell'intervallo di date di registrazione consentito, viene utilizzata la data di registrazione nel campo Consenti registraz. da del setup di contabilità generale OPPURE, se vengono utilizzati i periodi di magazzino, la data più lontana tra le due. Vedere il concetto descritto in precedenza.  

## <a name="history-of-post-inventory-cost-to-gl-batch-job"></a>Cronologia del processo batch Registra costo magazzino in C/G  
 Il processo batch Registra costo magazzino in C/G è strettamente associato al processo batch Rettifica Costo - Movimenti articoli ed è per questo motivo che la cronologia di questo processo batch è inclusa in questo argomento.  
 
![Costo effettivo rispetto al costo previsto](media/helene/TechArticleAdjustcost14.png "Costo effettivo rispetto al costo previsto")

### <a name="about-the-posting-date"></a>Informazioni sulla data di registrazione
 Non è più necessario indicare una data di registrazione nel modulo di richiesta del processo batch Registra costo magazzino in C/G. Il movimento C/G viene creato con la stessa data di registrazione del movimento di valorizzazione correlato. Per completare il processo batch, l'intervallo di date di registrazione consentite deve permettere la data di registrazione del movimento C/G creato. In caso contrario, l'intervallo di date di registrazione consentite deve essere riaperto temporaneamente modificando o rimuovendo le date nei campi Consenti registraz. da e Consenti registrazioni fino a nel setup di contabilità generale. Per evitare problemi di riconciliazione la data di registrazione del movimento C/G deve corrispondere alla data di registrazione del movimento di valorizzazione.  

 Il processo batch esamina la Tabella 5811 - Registra mov. valorizzazione in C/G per identificare i movimenti di valorizzazione nell'ambito della registrazione nella contabilità generale. Dopo una corretta esecuzione, la tabella viene svuotata.

## <a name="see-also"></a>Vedere anche  
[Dettagli di progettazione: Costing di magazzino](design-details-inventory-costing.md)  
[Dettagli di progettazione: Collegamento articoli](design-details-item-application.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
