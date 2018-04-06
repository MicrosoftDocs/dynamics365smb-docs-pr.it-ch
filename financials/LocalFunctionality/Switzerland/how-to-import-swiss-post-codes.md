---
title: 'Procedura: Importare codici postali svizzeri'
description: "È possibile importare l'ultimo file di codice postale e utilizzarlo per aggiornare la tabella **CAP**. Il file di codice postale può essere scaricato dal sito Web dei codici postali svizzeri. Dopo l'importazione del codice postale più recente, è possibile definire i codici postali per i clienti o i fornitori."
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
ms.openlocfilehash: 9f37f4ddf20a0a63237066017af87987ca3b9bd2
ms.contentlocale: it-ch
ms.lasthandoff: 03/22/2018

---
# <a name="import-swiss-post-codes"></a>Importare codici postali svizzeri
È possibile importare l'ultimo file di codice postale e utilizzarlo per aggiornare la tabella **CAP**. Il file di codice postale può essere scaricato dal sito Web dei [codici postali svizzeri](http://go.microsoft.com/fwlink/?LinkId=150292). Dopo l'importazione del codice postale più recente, è possibile definire i codici postali per i clienti o i fornitori. Per ulteriori informazioni, vedere [Registrare nuovi fornitori](../../purchasing-how-register-new-vendors.md).  

## <a name="to-import-post-codes"></a>Per importare i codici postali  

1.  Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "Cerca pagina o report"), immettere **Codici postali** e quindi scegliere il collegamento correlato.  
2.  Selezionare l'azione **Importa codici postali**.  
3.  Nella finestra **Importa codici postali** nel campo **Nome file** immettere il nome del file di codice postale da importare nella tabella **CAP**.  
4.  Scegliere il pulsante **OK**.  

    Le informazioni più recenti sui codici postali vengono importate.  

Di seguito viene descritto come definire i codici postali per i clienti, ma gli stessi passaggi si applicano anche per definire i codici postali per i fornitori.  

## <a name="to-define-post-codes-for-customers"></a>Per definire i codici postali per i clienti  

1.  Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Clienti**, quindi scegliere il collegamento correlato.  
2.  Selezionare il cliente per cui definire un codice postale, quindi scegliere l'azione **Modifica**.  
3.  Nella Scheda dettaglio **Generale** della finestra **Scheda cliente**, nel campo **CAP** selezionare il codice postale per l'indirizzo del cliente.  

    > [!NOTE]  
    >  Una volta selezionato il codice postale, i campi **Città** e **Codice paese** vengono popolati automaticamente con le informazioni della tabella **CAP**. Per ulteriori informazioni, vedere [Registrare nuovi clienti](../../sales-how-register-new-customers.md).  

4.  Scegliere il pulsante **OK**.  

## <a name="see-also"></a>Vedi anche   
 [Documenti di acquisto e di vendita per la Svizzera](swiss-purchase-documents-and-sales-documents.md)   
 [Impostare l'archiviazione automatica dei documenti in Svizzera](how-to-set-up-automatic-archiving-of-documents-in-switzerland.md)   
 [Stampare una lista prelievi magazzino da un ordine di vendita](how-to-print-an-inventory-picking-list-from-a-sales-order.md)   
 [Stampare ordini di vendita e acquisto durante la registrazione batch](how-to-print-sales-and-purchase-orders-during-batch-posting.md)   
 [Registrare nuovi fornitori](../../purchasing-how-register-new-vendors.md)  
