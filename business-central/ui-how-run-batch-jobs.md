---
title: Creare ed eseguire un processo batch | Documenti Microsoft
description: "È possibile eseguire i processi batch per elaborare i dati e aggiornare le informazioni, ad esempio, per attività contabili periodiche oppure per effettuare dei calcoli."
services: project-madeira
documentationcenter: 
author: SusanneWindfeldPedersen
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: task, process
ms.date: 10/01/2018
ms.author: solsen
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 9a6435120d122db894bcd6c953da5ab8ea78420b
ms.contentlocale: it-ch
ms.lasthandoff: 09/28/2018

---
# <a name="run-batch-jobs"></a>Eseguire i processi batch
Un processo batch è una routine che elabora i dati in batch, come, ad esempio, il processo **Rettifica tassi di cambio**. Alcuni processi batch eseguono attività contabili periodiche, ad esempio la chiusura del conto economico alla fine di un anno fiscale. Molti processi batch eseguono attività di calcolo, ad esempio il calcolo degli interessi finanziari, la rettifica dei tassi di cambio e il calcolo dei prezzi unitari.

Un processo batch è simile a un report, con la differenza che il processo batch utilizza il risultato delle attività che esegue per aggiornare direttamente le informazioni, anziché stampare i risultati.

## <a name="to-run-a-batch-job"></a>Per eseguire un processo batch
1. Per aprire la finestra di richiesta del processo batch pertinente, scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere il nome del processo batch e quindi scegliere il collegamento correlato.
2. Se per il processo batch è disponibile una Scheda dettaglio **Opzioni**, completarne i campi per determinare l'operazione che sarà eseguita dal processo batch.
3. È possibile che la finestra contenga una o più Schede dettaglio con filtri, che è possibile utilizzare per limitare i dati inclusi nel processo batch. È possibile immettere criteri nei filtri consigliati o aggiungere altri filtri.
4. Scegliere **OK** per avviare il processo batch.

## <a name="see-also"></a>Vedi anche
[Ricerca, filtro e ordinamento di dati](ui-enter-criteria-filters.md)  
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
