---
title: Annullare una registrazione con un movimento di pareggio | Microsoft Docs
description: Se è stata eseguita una registrazione errata nelle registrazioni generali, è possibile utilizzare la funzione Storno per annullare la registrazione con un audit trail corretto.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: reimbursement
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: cdbf4b682b4ad99524ea0aace9a123283668fb43
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 03/31/2021
ms.locfileid: "5779115"
---
# <a name="reverse-journal-postings-and-undo-receiptsshipments"></a>Stornare le registrazioni e annullare carichi/spedizioni errati
Per stornare una registrazione errata, selezionare un movimento e creare movimenti di storno, ovvero movimenti identici a quelli originali ma con segno opposto nel campo relativo all'importo, con numero di documento e data di registrazione identici a quelli del movimento originale. Dopo lo storno di un movimento, è necessario creare il movimento corretto.

È possibile stornare solo movimenti immessi da una riga di registrazioni generali. Un movimento può essere stornato solo una volta.

Per annullare la registrazione di un carico o di una spedizione, prima che vengano registrati come fatturati, è possibile utilizzare la funzione **Annulla** nel documento registrato. È possibile annullare le quantità di tipo **Articolo** e **Risorsa**.

Se è stata eseguita una registrazione di quantità negativa non corretta, ad esempio se è stato creato un ordine di acquisto con un numero errato di articoli e lo si è registrato come ricevuto (ma non fatturato), è possibile annullare la registrazione.

Se è stata eseguita una registrazione di quantità positiva, ad esempio se è stata creata una spedizione vendita o una spedizione di reso acquisto con un numero errato di articoli e lo si è registrato come spedito ma non fatturato, è possibile annullare la registrazione.   

## <a name="to-reverse-the-journal-posting-of-a-general-ledger-entry"></a>Per stornare la registrazione di un movimento di contabilità generale
È possibile stornare i movimenti da tutte le pagine **Movimenti contabili**. La seguente procedura è basata sulla pagina **Movimenti C/G**.
1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Movimenti contabilità generale** e quindi scegliere il collegamento correlato.
2. Selezionare il movimento che si desidera stornare quindi scegliere l'azione **Storno**. Si noti che è necessario che il movimento derivi da una registrazione.
3. Nella pagina **Storna movimenti transazioni**, scegliere l'azione **Storna**.
4. Scegliere il pulsante **Sì** nel messaggio di conferma.

> [!NOTE]
> Non è possibile annullare i movimenti registrati con le informazioni di un processo o che hanno realizzato utili e perdite all'interno della stessa transazione.

## <a name="to-post-a-negative-entry"></a>Per registrare un movimento negativo  
È possibile utilizzare il campo **Correzione** per registrare un addebito negativo anziché un credito oppure un accredito negativo anziché un addebito su un conto. Per soddisfare i requisiti legali, questo campo è visibile per impostazione predefinita in tutte le registrazioni. I campi **Dare** e **Avere** includono il movimento originale e il movimento corretto. Questi campi non influiscono sul saldo del conto.  

1.  Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Registrazioni COGE** e quindi scegliere il collegamento correlato  
2.  Nel campo **Nome batch** selezionare il nome di batch necessario.  
3.  Immettere informazioni nei campi rilevanti.  
4.  Nella riga di registrazione che si desidera attivare per i movimenti negativi, selezionare la casella di controllo **Correzione**.  
5.  Per contabilizzare la registrazione, scegliere l'azione **Registra**, quindi scegliere il pulsante **Sì**.

## <a name="to-undo-a-quantity-posting-on-a-posted-purchase-receipt"></a>Per annullare la registrazione di una quantità in una ricezione acquisti registrata  
Di seguito viene descritto come annullare un carico registrato di articoli o risorse. I passaggi sono simili a quelli per le spedizioni registrate.

1.  Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Carichi acquisti registrati** e quindi scegliere il collegamento correlato.  
2.  Aprire il carico registrato che si desidera annullare.  
3.  Selezionare la riga o le righe che si desidera annullare.  
4.  Scegliere l'azione **Annulla carico**.

Una riga di rettifica viene registrata sotto la riga di carico selezionata. Se la quantità è stata ricevuta in un carico warehouse, una riga di rettifica viene inserita nel carico warehouse registrato.  

I campi **Quantità ricevuta** e **Qtà carichi non fatt.** nell'ordine di acquisto collegato verranno impostati su un valore pari a zero.

## <a name="to-undo-and-then-redo-a-quantity-posting-on-a-posted-return-shipment"></a>Per annullare e successivamente ripetere la registrazione di una quantità in una spedizione di reso registrata
Di seguito viene descritto come annullare una spedizione di reso registrata di articoli o risorse e quindi registrare di nuovo il reso di acquisto con una nuova quantità. I passaggi sono simili a quelli per i carichi da reso registrati.

1.  Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Spedizioni reso registrate** e quindi scegliere il collegamento correlato.  
2.  Aprire la spedizione reso registrata che si desidera annullare.
3. Selezionare la riga o le righe che si desidera annullare.  

4.  Scegliere l'azione **Eliminare spedizione reso**.  

    Nel documento registrato viene inserita una riga correttiva e i campi **Qtà reso spedita** e **Reso spedito non fatt.** nell'ordine di reso vengono impostati su un valore pari a zero.  

    Ora tornare all'ordine di reso di acquisto per ripetere la registrazione.  

5.  Nella pagina **Spedizione reso registrata** prendere nota del numero nel campo **Nr. ordine di reso**. .  
6.  Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Ordini di reso acquisto** e quindi scegliere il collegamento correlato.  
7.  Aprire l'ordine di reso in questione quindi scegliere l'azione **Riapri**.  
8.  Correggere la voce nel campo **Quantità** e registrare nuovamente l'ordine di reso acquisto.  

## <a name="see-also"></a>Vedere anche
[Annullare la registrazione di assemblaggi](assembly-how-to-undo-assembly-posting.md)  
[Registrare le transazioni direttamente nella contabilità generale](finance-how-post-transactions-directly.md)  
[Utilizzo delle registrazioni COGE](ui-work-general-journals.md)  
[Finanze](finance.md)  
[Utilizzo di [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]