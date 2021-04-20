---
author: edupont04
ms.service: dynamics365-business-central
ms.topic: include
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 7cab5533c038dda6082a0455bf480779f143854e
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 03/31/2021
ms.locfileid: "5777577"
---
Dopo aver creato i solleciti di consegna, è necessario rilasciarli e stamparli in modo da poter inviare i solleciti ai fornitori. È possibile stampare un report di test prima di rilasciare i solleciti di consegna.  

Quando si rilasciano i solleciti di consegna, vengono creati movimenti contabili sollecito di consegna. È possibile visualizzare i movimenti contabili creati nella pagina **Movimenti contabili sollecito di consegna**.  

## <a name="to-issue-delivery-reminders"></a>Per emettere solleciti di consegna  

1. Scegliere l'![icona a forma di lampadina che consente di aprire la funzionalità delle informazioni](../../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Sollecito consegna** e quindi scegliere il collegamento correlato.  
2. Nella pagina **Sollecito di consegna**, selezionare il sollecito di consegna da rilasciare quindi selezionare l'azione **Modifica**.  
3. Scegliere l'azione **Emetti**.  
4. Nella pagina **Emettere sollecito di consegna**, compilare i campi come indicato nella tabella riportata di seguito.  

    |Campo|Descrizione|  
    |---------------------------------|---------------------------------------|  
    |**Stampa**|Selezionare la stampa dei solleciti di consegna quando vengono emessi.|  
    |**Sostituisci data registrazione**|Selezionare la sostituzione della data di registrazione esistente per il sollecito di consegna.|  
    |**Data di Registrazione**|Data di registrazione per il sollecito di consegna.<br /><br /> Questa data di registrazione viene utilizzata per tutti i solleciti di consegna se è stata selezionata la casella di controllo **Sostituisci data registrazione**. Se la casella di controllo **Sostituisci data registrazione** è deselezionata, questa data verrà utilizzata solo per i solleciti di consegna per i quali una data di registrazione non è disponibile.|  

5. Facoltativamente, nella Scheda dettaglio **Intestazione sollecito di consegna** selezionare i filtri appropriati.  

    > [!NOTE]  
    >  È possibile rimuovere i filtri ed emettere contemporaneamente tutti i solleciti di consegna.  

6. Scegliere il pulsante **OK**.  

È possibile visualizzare il solleciti di consegna nella pagina **Sollecito di consegna inviato**. Facoltativamente è possibile stampare un sollecito di consegna.  

## <a name="to-view-delivery-reminder-ledger-entries"></a>Per visualizzare i movimenti contabili solleciti di consegna  

1. Scegliere l'![icona a forma di lampadina che consente di aprire la funzionalità delle informazioni](../../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Ordini acquisto** e quindi scegliere il collegamento correlato.  
2. Selezionare l'ordine di acquisto per cui si desidera visualizzare lo stato del sollecito, quindi scegliere l'azione **Modifica**.  
3. Scegliere l'azione **Movimenti contabili sollecito di consegna**.  

Nella pagina **Movimenti contabili sollecito di consegna**, è possibile visualizzare i movimenti contabili sollecito di consegna per l'ordine di acquisto selezionato.  
