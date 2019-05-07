---
title: 'Procedura: Emettere solleciti di consegna'
description: Dopo aver creato i solleciti di consegna, è necessario rilasciarli e stamparli in modo da poter inviare i solleciti ai fornitori. È possibile stampare un report di test prima di rilasciare i solleciti di consegna.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: d5e4ac7e3762ce6d54aa466e5881dea810dd274a
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 03/31/2019
ms.locfileid: "916753"
---
# <a name="issue-delivery-reminders"></a>Emettere solleciti di consegna
Dopo aver creato i solleciti di consegna, è necessario rilasciarli e stamparli in modo da poter inviare i solleciti ai fornitori. È possibile stampare un report di test prima di rilasciare i solleciti di consegna. Per ulteriori informazioni, vedere [Stampare report di test per i solleciti di consegna](how-to-print-test-reports-for-delivery-reminders.md).  

Quando si rilasciano i solleciti di consegna, vengono creati movimenti contabili sollecito di consegna. È possibile visualizzare i movimenti contabili creati nella pagina **Movimenti contabili sollecito di consegna**.  

## <a name="to-issue-delivery-reminders"></a>Per emettere solleciti di consegna  

1.  Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Sollecito di consegna**, quindi scegliere il collegamento correlato.  
2.  Nella pagina **Sollecito di consegna**, selezionare il sollecito di consegna da rilasciare quindi selezionare l'azione **Modifica**.  
3.  Scegliere l'azione **Emetti**.  
4.  Nella Scheda dettaglio **Opzioni** della pagina **Emettere sollecito di consegna** compilare i campi come descritto nella tabella seguente.  

    |Campo|Descrizione|  
    |---------------------------------|---------------------------------------|  
    |**Stampa**|Selezionare la stampa dei solleciti di consegna quando vengono emessi.|  
    |**Sostituisci data registrazione**|Selezionare la sostituzione della data di registrazione esistente per il sollecito di consegna.|  
    |**Data di Registrazione**|Data di registrazione per il sollecito di consegna.<br /><br /> Questa data di registrazione viene utilizzata per tutti i solleciti di consegna se è stata selezionata la casella di controllo **Sostituisci data registrazione**. Se la casella di controllo **Sostituisci data registrazione** è deselezionata, questa data verrà utilizzata solo per i solleciti di consegna per i quali una data di registrazione non è disponibile.|  

5.  Facoltativamente, nella Scheda dettaglio **Intestazione sollecito di consegna** selezionare i filtri appropriati.  

    > [!NOTE]  
    >  È possibile rimuovere i filtri ed emettere contemporaneamente tutti i solleciti di consegna.  

6.  Scegliere il pulsante **OK**.  

È possibile visualizzare il solleciti di consegna nella pagina **Sollecito di consegna inviato**. Facoltativamente è possibile stampare un sollecito di consegna.  

## <a name="to-view-delivery-reminder-ledger-entries"></a>Per visualizzare i movimenti contabili solleciti di consegna  

1.  Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "Cerca pagina o report"), immettere **Ordini acquisto**, quindi scegliere il collegamento correlato.  
2.  Selezionare l'ordine di acquisto per cui si desidera visualizzare lo stato del sollecito, quindi scegliere l'azione **Modifica**.  
3.  Scegliere l'azione **Movimenti contabili sollecito di consegna**.  

Nella pagina Movimenti contabili sollecito di consegna, è possibile visualizzare i movimenti contabili sollecito di consegna per l'ordine di acquisto selezionato.  

## <a name="see-also"></a>Vedi anche  
 [Solleciti consegna](delivery-reminders.md)   
 [Generare solleciti di consegna](how-to-generate-delivery-reminders.md)   
 [Creare solleciti di consegna manualmente](how-to-create-delivery-reminders-manually.md)
