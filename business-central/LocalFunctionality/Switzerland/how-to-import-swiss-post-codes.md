---
title: 'Procedura: Importare codici postali svizzeri'
description: È possibile importare l'ultimo file di codice postale e utilizzarlo per aggiornare la tabella CAP. Il file di codice postale può essere scaricato dal sito Web dei codici postali svizzeri. Dopo l'importazione del codice postale più recente, è possibile definire i codici postali per i clienti o i fornitori.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 278ed697f3380633d6d35387ed7eeb3ed6b15c6c
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 02/15/2021
ms.locfileid: "5383979"
---
# <a name="import-swiss-post-codes"></a>Importare codici postali svizzeri
È possibile importare l'ultimo file di codice postale e utilizzarlo per aggiornare la tabella **CAP**. Il file di codice postale può essere scaricato dal sito Web dei [codici postali svizzeri](https://go.microsoft.com/fwlink/?LinkId=150292). Dopo l'importazione del codice postale più recente, è possibile definire i codici postali per i clienti o i fornitori. Per ulteriori informazioni, vedere [Registrare nuovi fornitori](../../purchasing-how-register-new-vendors.md).  

## <a name="to-import-post-codes"></a>Per importare i codici postali  

1.  Scegliere l'![icona a forma di lampadina che consente di aprire la funzionalità delle informazioni](../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **NPA** e quindi scegliere il collegamento correlato.  
2.  Selezionare l'azione **Importa codici postali**.  
3.  Nella pagina **Importa codici postali** nel campo **Nome file** immettere il nome del file di codice postale da importare nella tabella **CAP**.  
4.  Scegliere il pulsante **OK**.  

    Le informazioni più recenti sui codici postali vengono importate.  

Di seguito viene descritto come definire i codici postali per i clienti, ma gli stessi passaggi si applicano anche per definire i codici postali per i fornitori.  

## <a name="to-define-post-codes-for-customers"></a>Per definire i codici postali per i clienti  

1.  Scegliere l'![icona a forma di lampadina che consente di aprire la funzionalità delle informazioni](../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Clienti** e quindi scegliere il collegamento correlato.  
2.  Selezionare il cliente per cui definire un codice postale, quindi scegliere l'azione **Modifica**.  
3.  Nella Scheda dettaglio **Generale** della pagina **Scheda cliente**, nel campo **CAP** selezionare il codice postale per l'indirizzo del cliente.  

    > [!NOTE]  
    >  Una volta selezionato il codice postale, i campi **Città** e **Codice paese** vengono popolati automaticamente con le informazioni della tabella **CAP**. Per ulteriori informazioni, vedere [Registrare nuovi clienti](../../sales-how-register-new-customers.md).  

4.  Scegliere il pulsante **OK**.  

## <a name="see-also"></a>Vedi anche   
 [Documenti di acquisto e di vendita per la Svizzera](swiss-purchase-documents-and-sales-documents.md)   
 [Stampare una lista prelievi magazzino da un ordine di vendita](how-to-print-an-inventory-picking-list-from-a-sales-order.md)   
 [Registrare nuovi fornitori](../../purchasing-how-register-new-vendors.md)  


[!INCLUDE[footer-include](../../includes/footer-banner.md)]