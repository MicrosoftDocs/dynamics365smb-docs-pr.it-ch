---
title: Come importare numeri di clearing bancari svizzeri
description: "I numeri di clearing bancari sono numeri univoci usati per identificare ogni agenzia o filiale nella directory delle banche. Questa informazioni è necessaria per effettuare un pagamento elettronico. Il file può essere scaricato dal sito Web [SIX Interbank Clearing](http://go.microsoft.com/fwlink/?LinkId=145121)."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b34f276a764f0e828fbc1f015429df9852242a4c
ms.openlocfilehash: 6a9e593c25555a3780f7ec895cd70b34ce4c3170
ms.contentlocale: it-ch
ms.lasthandoff: 03/22/2018

---
# <a name="import-swiss-bank-clearing-numbers"></a>Importare numeri di clearing svizzeri
I numeri di clearing bancari sono numeri univoci usati per identificare ogni agenzia o filiale nella directory delle banche. Questa informazioni è necessaria per effettuare un pagamento elettronico. Il file può essere scaricato dal sito Web [SIX Interbank Clearing](http://go.microsoft.com/fwlink/?LinkId=145121).  

È possibile importare il file Bank Master di numeri di clearing, ovvero il file ufficiale dei numeri di clearing bancari, per aggiornare le informazioni sui numeri di clearing nella directory delle banche. Quando si importa il file dei numeri di clearing bancari, i dati vengono inseriti nella tabella **Directory banche** e i dati esistenti vengono sovrascritti. Dopo aver importato il file dei numeri di clearing bancari, è possibile definire il numero di filiale aggiornato per clienti e fornitori. Per ulteriori informazioni, vedere le tabelle Conti correnti clienti e Conti correnti fornitori.  

## <a name="to-import-swiss-bank-clearing-numbers"></a>Per importare numeri di clearing svizzeri  

1.  Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Directory banche**, quindi scegliere il collegamento correlato.  
2.  Scegliere l'azione **Importa directory banche**.  
3.  Nella finestra **Importa directory banche**, nella Scheda dettaglio **Opzioni** selezionare il campo **Aggiorna automaticamente numeri di clearing** per aggiornare i numeri di clearing bancari in modo automatico.  
4.  Scegliere il pulsante **Stampa** o il pulsante **Anteprima** per importare i numeri di clearing bancari, quindi nella finestra **Apri** individuare il file scaricato dal sito Web SIX Interbank Clearing.
5. Scegliere il pulsante **Apri**.  

    Se si sceglie il pulsante **Stampa**, il contenuto del file verrà stampato. Se si sceglie il pulsante **Anteprima**, la tabella **Directory banche** verrà aggiornata e verrà visualizzato un report con i numeri di clearing modificati.  

La procedura seguente descrive come definire i numeri di filiale bancaria per i conti correnti dei clienti, ma gli stessi passaggi si applicano anche per definire i numeri di filiale per i conti correnti dei fornitori.  

## <a name="to-define-bank-branch-numbers-for-customer-bank-accounts"></a>Per definire i numeri di filiale bancaria per i conti correnti dei clienti  

1.  Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Clienti**, quindi scegliere il collegamento correlato.  
2.  Selezionare il cliente per cui creare informazioni di conto corrente, quindi scegliere l'azione **C/C bancari**.  
3.  In **Lista C/C bancari clienti**, selezionare il conto corrente bancario richiesto e scegliere l'azione **Modifica**.  
4.  Nella scheda dettaglio **Generale**, nel campo **Nr. filiale banca** selezionare il numero dell'agenza o filiale bancaria.  
5.  Scegliere il pulsante **OK**.  

## <a name="see-also"></a>Vedi anche  
 [Pagamenti elettronici svizzeri](swiss-electronic-payments.md)   
 [Impostare i conti correnti bancari](../../bank-how-setup-bank-accounts.md)

