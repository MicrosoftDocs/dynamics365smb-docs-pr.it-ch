---
author: edupont04
ms.topic: include
ms.date: 03/01/2022
ms.author: edupont
ms.openlocfilehash: 5a3e15669bfc590d663b7774fba84017ae842521
ms.sourcegitcommit: 865b390b5571b08084bde93b539ec9898e201933
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 03/02/2022
ms.locfileid: "8372070"
---
La tabella seguente descrive alcuni dei report di produzione chiave.

| Report | Descrizione | Id | 
|---------|---------|---------|
| [Esplosione quantità DB](https://businesscentral.dynamics.com?report=99000753)|Mostra una lista della DB con rientri per l'articolo o gli articoli che si specificano nel filtro. La DB di produzione viene completamente esplosa a tutti i livelli.|99000753|
| [Articolo - Produzione possibile (sequenza temporale)](https://businesscentral.dynamics.com?report=5871)|Mostra come cinque diverse cifre sulla disponibilità principali cambiano nel tempo per un articolo della DB. Tali cifre cambiano in base agli eventi previsti di approvvigionamento e domanda e all'approvvigionamento basato sui componenti disponibili che possono essere assemblati o prodotti.<br>È possibile utilizzare il report per verificare se è possibile soddisfare un ordine di vendita per un articolo nella data stabilita osservando la disponibilità corrente insieme alle quantità potenziali che i suoi componenti possono fornire se un ordine di assemblaggio fosse avviato. Questo report mostra quando e quante unità di un articolo di assemblaggio e di produzione è possibile produrre sulla base della disponibilità dei componenti e della disponibilità corrente dell'articolo. Questo valore è indicato come quantità totale.<br>Le informazioni vengono mostrate in un grafico in cui ogni cifra sulla disponibilità è rappresentata da una linea che avanza lungo la sequenza temporale e si sposta verso l'alto e verso il basso al variare delle quantità. Le cifre sulla quantità provengono dallo stesso motore che fornisce informazioni nella finestra **Pagina Disponibilità articolo per livello DB**. |5871|
| [Distribuzione dettaglio costi DB](https://businesscentral.dynamics.com?report=5872)|Visualizza graficamente come il costo di un articolo prodotto o assemblato viene ripartito nella relativa DB.<br>Tali informazioni possono essere utili per decidere, ad esempio, se modificare i fornitori di componenti, sostituire l'utilizzo di capacità interna con manodopera in appalto o viceversa o quando si rivede e si modifica la distinta base di un articolo.<br>Il primo grafico nel report mostra il costo unitario totale dei componenti e delle risorse di manodopera dell'articolo padre suddivisi fino a cinque dettagli di costo diversi e rappresentati graficamente con diversi colori.<br>Il grafico a torta etichettato *Per materiale/manodopera* mostra la distribuzione proporzionale tra il materiale e i costi di manodopera dell'articolo padre nonché i costi generali di produzione. Il dettaglio dei costi del materiale include i costi del materiale dell'articolo. Il dettaglio del costo di manodopera include la capacità, i costi generali capacità e i costi in conto lavoro. Le quote di costo vengono visualizzate in modo diverso a seconda delle tue scelte nel campo **Mostra solo**.<br>Il grafico a torta con la didascalia *Per costo diretto/indiretto* mostra la distribuzione proporzionale i costi diretti e indiretti dell'articolo padre. Il dettaglio dei costi diretti include i costi di materiale, capacità e in conto lavoro. Il dettaglio dei costi indiretti include i costi generali capacità e i costi generali produzione.<br>La tabella nella parte inferiore del report verrà inclusa quando si seleziona la casella di controllo **Includi dettaglio**. Visualizza i valori selezionati nella finestra Dettaglio costi DB per singolo livello o ricalcolati, in base all'opzione scelta nel campo **Mostra dettaglio costi come**.|5872|
| [Calcolo dettagliato](https://businesscentral.dynamics.com?report=99000756)|Mostra una lista dei costi per ogni articolo tenendo in considerazione lo scarto.|99000756|
| [Dove-usato (livello principale)](https://businesscentral.dynamics.com?report=99000757)|Mostra dove e in quali quantità gli articoli vengono utilizzati nella struttura di prodotto.<br>Il report fornisce soltanto l'articolo dove utilizzato, quando l'articolo di base viene utilizzato come articolo di livello superiore. Ad esempio, se l'articolo “A” viene utilizzato per produrre l'articolo “B” e l'articolo “B” viene utilizzato per produrre l'articolo “C”, il report mostrerà l'articolo B se si esegue questo report per l'articolo A. Se si esegue questo report per l'articolo B, allora l'articolo C verrà mostrato dove utilizzato.<br>La pagina **Righe dove-usato** può essere aperta direttamente dall'articolo.|99000757|
| [Lista confronto DB articolo](https://businesscentral.dynamics.com?report=99000758)|Questo report ti dà la possibilità di confrontare prodotti finali simili riguardo ai costi. Vedrai un elenco con tutti i componenti e i loro costi, nonché le quantità necessarie. La data calcolo è normalmente impostata sulla data di lavoro. |99000758|
| [Statistiche ordini di produzione](https://businesscentral.dynamics.com?report=99000791)|Specifica i vari costi che si sono accumulati per l'ordine di produzione selezionato.<br>Il contenuto del report è molto simile alla pagina **Statistiche ordini produzione**.<br>Per gli ordini di produzione che utilizzano la politica di produzione *Produzione su ordine*, la finestra mostra solo i costi di materiale e capacità degli articoli al più alto livello della DB.|99000791|
| [Lista task capacità](https://businesscentral.dynamics.com?report=99000780)|Mostra gli ordini di produzione in attesa di essere elaborati nelle aree di produzione e nei centri di lavoro. Le stampe vengono effettuate per la capacità dell'area di produzione o del centro lavoro. Il report comprende informazioni quali l'ora di inizio e di fine, la data per ordine di produzione e la quantità di input.|99000780|
| [Carico area di produzione](https://businesscentral.dynamics.com?report=99000783)|Fornisce una lista del carico su un'area di produzione. Il carico su un'area di produzione è la somma del numero di esecuzioni richieste di tutti gli ordini pianificati ed effettivi sull'area di lavoro in un periodo specificato.|99000783|
| [Carico centro lavoro](https://businesscentral.dynamics.com?report=99000784)|Fornisce una lista del carico su un centro di lavoro. Il carico su un centro di lavoro è la somma del numero di esecuzioni richieste di tutti gli ordini pianificati ed effettivi sul centro di lavoro in un periodo specificato.|99000784|
| [Ord. prod. - Lista el. mancanti](https://businesscentral.dynamics.com?report=99000788)|Questo report può essere utilizzato per vedere tutti i componenti che non sono disponibili a causa di scorte mancanti. Quindi, questa panoramica può essere utilizzata per vedere in tempo, se la sequenza temporale per un ordine di produzione pianificato o rilasciato se il tempo pianificato può essere mantenuto.|99000788|
|[Ordine di produzione - Calcolo](https://businesscentral.dynamics.com?report=99000767)|Fornisce una lista degli ordini di produzione e i relativi costi. Sono inclusi i costi operazione previsti, i costi componenti previsti e i costi totali.|99000767|