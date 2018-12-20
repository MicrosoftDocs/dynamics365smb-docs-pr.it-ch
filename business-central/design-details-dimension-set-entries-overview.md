---
title: Sintesi movimenti set di dimensioni | Microsoft Docs
description: In questo argomento viene descritto il modo in cui i movimenti set di dimensioni vengono memorizzati e registrati in Dynamcis 365.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: dimension
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 0a94a47a2c32fc38792fbfc3285e9d0e4659ccf1
ms.contentlocale: it-ch
ms.lasthandoff: 09/28/2018

---
# <a name="dimension-set-entries-overview"></a>Sintesi movimenti set di dimensioni
In questo argomento viene descritto il modo in cui i movimenti set di dimensioni vengono memorizzati e registrati in [!INCLUDE[d365fin](includes/d365fin_md.md)].  

## <a name="dimension-sets"></a>Set di dimensioni  
Un set di dimensioni è una combinazione univoca di valori dimensioni. Viene archiviato come movimenti set di dimensioni nel database. Ogni movimento set di dimensioni rappresenta un valore dimensioni singolo. Il set di dimensioni è identificato da un ID set di dimensioni comune assegnato a ogni movimento set di dimensioni che appartiene al set di dimensioni.  

Nel seguente esempio viene mostrato un set di dimensioni in cui sono presenti tre relativi movimenti. Il set di dimensioni è identificato da un ID set di dimensioni, vale a dire 108.  

|ID set di dimensioni|Codice Dimensione:|Codice Valore Dimensioni:|Nome valore dimensioni|  
|----------------------|--------------------|--------------------------|--------------------------|  
|108|AREA|70|Nord America|  
|108|GRUPPOBUSINES|HOME|Home|  
|108|REPARTO|VENDITE|Vendite|  

## <a name="dimension-set-entries"></a>Movimenti set di dimensioni  
I set di dimensioni vengono archiviati nella tabella **Movimento set di dimensioni** come movimenti di set di dimensioni con lo stesso ID set di dimensioni.  

![Flusso dei movimenti del set di dimensioni](media/dimensionentrynav7.png "Flusso dei movimenti del set di dimensioni")  

Quando si crea una nuova riga di registrazione, testata del documento o riga documento, è possibile specificare una combinazione di valori dimensioni. Anziché archiviare esplicitamente ogni valore dimensioni nel database, viene assegnato un ID set di dimensioni alla riga di registrazione, alla testata del documento o alla riga del documento per specificare il set di dimensioni.  

Quando si modifica e si chiude la finestra **Modifica movimenti set di dimensioni** , viene eseguito un controllo per verificare se la combinazione dei valori dimensioni esiste come set di dimensioni nella tabella. Se la combinazione si verifica nella tabella, l'ID set di dimensioni corrispondente viene assegnato alla riga di registrazione, alla testata del documento o alla riga del documento. In caso contrario, un nuovo set di dimensioni viene aggiunto alla tabella e il nuovo ID set di dimensioni viene assegnato alla riga di registrazione, alla testata del documento o alla riga del documento.  

## <a name="performance-improvement"></a>Miglioramento delle prestazioni  
Archiviando i set di dimensioni una volta nel database, lo spazio di quest'ultimo viene mantenuto e le prestazioni globali vengono migliorate.  

## <a name="see-also"></a>Vedi anche  
[Dettagli di progettazione: Ricerca delle combinazioni di dimensione](design-details-searching-for-dimension-combinations.md)   
[Dettagli di progettazione: Struttura della tabella](design-details-table-structure.md)   
[Dettagli di progettazione: Gestione dimensioni della codeunit 408](design-details-codeunit-408-dimension-management.md)   
[Dettagli di progettazione: Esempi di codice dei modelli modificati nelle modifiche](design-details-code-examples-of-changed-patterns-in-modifications.md)   
[Dettagli di progettazione: Movimenti set di dimensioni](design-details-dimension-set-entries.md)   
