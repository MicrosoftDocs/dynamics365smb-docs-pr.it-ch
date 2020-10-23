---
title: Come importare numeri di clearing bancari svizzeri
description: I numeri di clearing bancari sono numeri univoci usati per identificare ogni agenzia o filiale nella directory delle banche. Questa informazioni è necessaria per effettuare un pagamento elettronico. Il file può essere scaricato dal sito Web SIX Interbank Clearing.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 55b3993f30484af990b1500f18490ed70b00bc0a
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 10/01/2020
ms.locfileid: "3914638"
---
# <a name="import-swiss-bank-clearing-numbers"></a>Importare numeri di clearing svizzeri
I numeri di clearing bancari sono numeri univoci usati per identificare ogni agenzia o filiale nella directory delle banche. Questa informazioni è necessaria per effettuare un pagamento elettronico. Il file può essere scaricato dal sito Web [SIX Interbank Clearing](https://go.microsoft.com/fwlink/?LinkId=145121).  

È possibile importare il file Bank Master di numeri di clearing, ovvero il file ufficiale dei numeri di clearing bancari, per aggiornare le informazioni sui numeri di clearing nella directory delle banche. Quando si importa il file dei numeri di clearing bancari, i dati vengono inseriti nella tabella **Directory banche** e i dati esistenti vengono sovrascritti. Dopo aver importato il file dei numeri di clearing bancari, è possibile definire il numero di filiale aggiornato per clienti e fornitori. Per ulteriori informazioni, vedere le tabelle Conti correnti clienti e Conti correnti fornitori.  

## <a name="to-import-swiss-bank-clearing-numbers"></a>Per importare numeri di clearing svizzeri  

1.  Scegliere l'![icona a forma di lampadina che consente di aprire la funzionalità delle informazioni](../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Elenco banche** e quindi scegliere il collegamento correlato.  
2.  Scegliere l'azione **Importa directory banche**.  
3.  Nella pagina **Importa directory banche**, nella Scheda dettaglio **Opzioni** selezionare il campo **Aggiorna automaticamente numeri di clearing** per aggiornare i numeri di clearing bancari in modo automatico.  
4.  Scegliere il pulsante **Stampa** o il pulsante **Anteprima** per importare i numeri di clearing bancari, quindi nella pagina **Apri** individuare il file scaricato dal sito Web SIX Interbank Clearing.
5. Scegliere il pulsante **Apri**.  

    Se si sceglie il pulsante **Stampa**, il contenuto del file verrà stampato. Se si sceglie il pulsante **Anteprima**, la tabella **Directory banche** verrà aggiornata e verrà visualizzato un report con i numeri di clearing modificati.  

La procedura seguente descrive come definire i numeri di filiale bancaria per i conti correnti dei clienti, ma gli stessi passaggi si applicano anche per definire i numeri di filiale per i conti correnti dei fornitori.  

## <a name="to-define-bank-branch-numbers-for-customer-bank-accounts"></a>Per definire i numeri di filiale bancaria per i conti correnti dei clienti  

1.  Scegliere l'![icona a forma di lampadina che consente di aprire la funzionalità delle informazioni](../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Clienti** e quindi scegliere il collegamento correlato.  
2.  Selezionare il cliente per cui creare informazioni di conto corrente, quindi scegliere l'azione **C/C bancari**.  
3.  Nella pagina **Lista C/C bancari clienti**, selezionare il conto corrente bancario richiesto e scegliere l'azione **Modifica**.  
4.  Nella scheda dettaglio **Generale**, nel campo **Nr. filiale banca** selezionare il numero dell'agenza o filiale bancaria.  
5.  Scegliere il pulsante **OK**.  

## <a name="see-also"></a>Vedere anche  
 [Pagamenti elettronici svizzeri](swiss-electronic-payments.md)   
 [Impostare i conti correnti bancari](../../bank-how-setup-bank-accounts.md)
