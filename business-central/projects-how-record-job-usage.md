---
title: Registrare il consumo o l'utilizzo di articoli e di risorse nella commessa
description: Descrive come registrare il consumo o l'utilizzo degli articoli o di risorse nelle commesse per semplificare la gestione progetti.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project management, consumption
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 65975621fff862b64333c87e70f34b75f8e2cbdb
ms.sourcegitcommit: 93c8681054b059cec38cb29b86de20be37980676
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 04/23/2021
ms.locfileid: "5938114"
---
# <a name="record-consumption-or-usage-for-jobs"></a>Registrare il consumo o l'utilizzo per le commesse

Nella pagina **Righe pianificazione commessa** è possibile esaminare e registrare l'utilizzo nelle diverse parti della commessa, che viene automaticamente aggiornato quando si modificano e si trasferiscono le informazioni tra le commesse e le registrazioni delle commesse o le fatture commessa. Questo richiede che sia stata impostata una commessa in modo da attivare **Applica collegamento utilizzo**. Per ulteriori informazioni, vedere [Impostare le commesse](projects-how-setup-jobs.md).  

Ad esempio, per le righe di pianificazione di tipo **Budget**, è possibile immettere la quantità di una risorsa e indicare la quantità da trasferire nelle registrazioni commesse. Se il tipo di righe di pianificazione è **Fatturabile**, è possibile immettere la quantità della risorsa e indicare la quantità da trasferire in una fattura. Per ulteriori informazioni sulla fatturazione al cliente, vedere [Fatturazione di commesse](projects-how-invoice-jobs.md). Confrontando la quantità originale, la quantità residua o la quantità registrata è possibile rivedere rapidamente le informazioni sull'utilizzo. Per informazioni sulla stima dei valori a budget durante la pianificazione, vedere [Gestire i budget delle commesse](projects-how-manage-budgets.md).  

Di seguito viene descritto come registrare le quantità e i costi (previsti) effettivi con la registrazione delle commesse. In alternativa è possibile utilizzare i documenti di acquisto per registrare l'acquisto di una commessa. Per ulteriori informazioni, vedere [Gestire gli approvvigionamenti delle commesse](projects-how-manage-project-supplies.md).

## <a name="to-record-usage-for-a-job-planning-line-of-type-budget"></a>Per registrare l'utilizzo per una riga di pianificazione commessa di tipo Budget

1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Commesse** e quindi scegliere il collegamento correlato.  
2. Selezionare la relativa commessa, quindi scegliere l'azione **Righe pianificazione commessa**.
3. Selezionare una riga di pianificazione commessa di tipo **Budget** o **Budget e fatturabile** per la quale si desidera registra l'utilizzo.  

    > [!NOTE]
    > È inoltre possibile registrare l'utilizzo per una riga pianificazione commessa di tipo **Fatturabile**. In genere, queste righe vengono utilizzate per creare fatture, ma è anche possibile trasferirle a una registrazione. Per ulteriori informazioni, vedere [Fatturazione di commesse](projects-how-invoice-jobs.md) <!--However, when you do that, a job planning line of type **Budget** is created to match the billable line. For more information, see [Manage Job Budgets](projects-how-manage-budgets.md).-->

4. Nel campo **Qtà da trasferire per registrazione**, immettere il numero che si desidera trasferire. La quantità di default è il valore che si immette nel campo **Quantità**.

    Il campo **Quantità residua** mostra la quantità che rimane per completare la commessa e da trasferire nelle registrazioni.  
5. Scegliere l'azione **Crea righe registrazioni commesse**.

    > [!TIP]
    > Se si aggiungono più righe di pianificazione commessa per questa commessa, attendere fino a quando non sono state aggiunte tutte le righe di pianificazione commessa.
6. Nella pagina **Trasferimento commessa a riga pianificazione** compilare i campi in base alle esigenze, quindi scegliere **OK**. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
7. Scegliere l'azione **Apri registrazioni commesse**.  
8. Nella pagina **Registrazioni commesse**, selezionare la riga pertinente e scegliere l'azione **Registra**.
9. Nella pagina **Righe pianificazione commessa**, esaminare l'utilizzo registrato osservando i campi **Quantità**, **Quantità residua** e **Qtà da trasferire per registrazione**.  
10. Ripetere i passaggi da 3 a 8 per registrare altri utilizzi.  

## <a name="to-create-job-journal-lines-manually"></a>Per creare le righe delle registrazioni delle commesse manualmente

1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Registrazioni commesse** e quindi scegliere il collegamento correlato.  
2. Nel campo **Nome batch** scegliere un nome batch di registrazioni commesse pertinente.  
3. In una nuova riga, immettere il numero di documento, il numero di commessa, il numero di task commessa, il tipo e la quantità del tipo consumata.  
4. Una volta completate le righe di registrazione commessa, scegliere l'azione **Registra**.  

## <a name="to-view-job-usage-estimates-and-post-updates"></a>Per visualizzare le stime di utilizzo della commessa e gli aggiornamenti della registrazione

È possibile visualizzare l'utilizzo della commessa fino al completamento di un progetto in un unico passaggio. A questo scopo, utilizzare il processo batch **Commessa - Calc. utilizzo residuo** per tutti i task fino al termine della commessa incluso.  

In questo modo è possibile tenere traccia e confrontare le stime iniziali rispetto ai risultati effettivi ed apportare modifiche o creare nuovi movimenti in base alle esigenze. Ad esempio, è possibile che si sia stimato che una commessa richieda 10 ore e ad oggi siano state impiegate 15 ore. È possibile aggiungere le cinque ore in più nella riga di registrazione esistente o creare una nuova riga registrazioni per indicare le cinque ore come straordinario, ovvero un altro tipo di lavoro. Vengono calcolati il costo e il prezzo appropriati ed è quindi possibile contabilizzarli nella registrazione.  

> [!NOTE]  
>   I movimenti articoli creano movimenti contabili articoli e riducono la quantità di inventario. Il processo batch **Registra costo magazzino in C/GL** trasferisce il costo dal magazzino alla contabilità generale. I movimenti risorse creano movimenti contabili risorse.  

1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Registrazioni commesse** e scegliere il collegamento correlato.  
2. Selezionare una registrazione commessa corrispondente, quindi scegliere l'azione **Calc. utilizzo residuo**.  
3. Nella pagina **Commessa - Calc. utilizzo residuo**, immettere il numero di documento e la data di registrazione che deve essere inserita nelle registrazioni, quindi scegliere **OK**.  
4. Aggiornare le registrazioni con tutte le necessarie modifiche.  
5. Scegliere **Registra**.



## <a name="to-review-planning-lines-for-a-job-ledger-entry"></a>Per esaminare le righe di pianificazione per un movimento contabile commessa

Dopo avere registrato le righe di registrazione commessa registrate, è possibile visualizzare le righe di pianificazione associate ai movimenti di registrazione commesse che sono stati registrati.

> [!NOTE]  
> Ciò richiede che la casella di controllo **Applica collegamento di utilizzo** sia stata selezionata la commessa. Per ulteriori informazioni, vedere [Impostare le commesse](projects-how-setup-jobs.md).  

1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Registrazioni commesse** e quindi scegliere il collegamento correlato.  
2. Selezionare una registrazione commessa corrispondente, quindi scegliere l'azione **Mov. contabili**.  
3. Nella pagina **Movimenti contabili commesse** scegliere l'azione **Mostra righe pianificazione commessa collegate**.

## <a name="see-also"></a>Vedi anche
[Gestione progetti](projects-manage-projects.md)  
[Finanze](finance.md)  
[Acquisti](purchasing-manage-purchasing.md)         
[Vendite](sales-manage-sales.md)      
[Utilizzo di [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
