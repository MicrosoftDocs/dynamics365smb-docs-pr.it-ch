---
title: Creare una fattura di vendita per fatturare una commessa| Documenti Microsoft
description: Viene descritto come fatturare ai clienti le spese commessa durante lo svolgimento di un progetto.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project invoice
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 873135d2fa6053b7101a999981fb3117ee8689ab
ms.sourcegitcommit: 93c8681054b059cec38cb29b86de20be37980676
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 04/23/2021
ms.locfileid: "5938164"
---
# <a name="invoice-jobs"></a>Fatturazione di commesse
Durante il progetto, è possibile che si accumulino i costi di commessa derivanti dall'utilizzo delle risorse, dai materiali e dagli acquisti correlati alla commessa. A seconda dello stato di avanzamento della commessa, tali transazioni vengono inserite nelle registrazioni commesse. È importante registrare tutti i costi prima di fatturare al cliente.

> [!NOTE]
> Puoi inoltre acquistare risorse esterne non correlate a un processo, ad esempio, per fatturare a un fornitore per il lavoro eseguito. Per ulteriori informazioni, vedere [Registrare gli acquisti](purchasing-how-record-purchases.md).

È possibile fatturare l'intera commessa dalla pagina **Righe task commessa** oppure fatturare solo le righe fatturabili selezionate dalla pagina **Righe pianificazione**. La fatturazione può essere effettuata dopo la chiusura della commessa oppure durante lo svolgimento delle operazioni correlate alla commessa, a determinati intervalli basati su un'apposita programmazione.

> [!NOTE]  
> Se si seleziona **Fatturabile** nel campo **Tipo riga commessa** dei documenti di acquisto per gli acquisti correlati alla commessa, vengono create le righe di pianificazione commessa che sono pronte per la fatturazione al cliente. Per ulteriori informazioni, vedere [Gestire gli approvvigionamenti per un progetto](projects-how-manage-project-supplies.md).

## <a name="to-create-multiple-job-sales-invoices"></a>Per creare più fatture di vendita commesse
È possibile creare una fattura per una commessa o per uno o più task commessa per un cliente al completamento del lavoro da fatturare o al raggiungimento della data per la fatturazione in base a una programmazione di fatturazione.

Nella procedura che segue viene mostrato come utilizzare un processo batch per fatturare più commesse.  

1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Commessa - Crea fattura vendita** e quindi scegliere il collegamento correlato.  
2. Compilare i campi, se necessario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. Impostare i filtri se si desidera limitare le commesse che devono essere elaborate nel processo batch.
4. Scegliere il pulsante **OK** per creare le fatture di assistenza.  

È possibile rivedere e pubblicare le fatture create nella finestra **Fatture vendita**.

> [!NOTE]
> In alternativa, fatturare a un cliente selezionando la commessa, quindi scegliendo l'azione **Crea fattura vendita per commessa**. 

## <a name="to-create-and-post-job-sales-invoice-from-job-planning-lines"></a>Per creare e registrare una fattura di vendita commessa dalle righe di pianificazione commessa
È possibile creare una fattura da righe di pianificazione commessa e indicare in quella occasione la quantità dell'articolo, la risorsa o il conto di contabilità generale che si desidera fatturare.

1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Commesse** e quindi scegliere il collegamento correlato.
2. Aprire una commessa appropriata.
3. Selezionare un task commessa per il quale il campo **Tipo task commessa** contiene **Registrazione**, quindi scegliere l'azione **Righe pianificazione commessa**.  
4. In una riga di pianificazione commessa, nel campo **Qtà da trasferire in fattura** , immettere la quantità dell'articolo, la risorsa, il tipo del conto di contabilità generale che si desidera fatturare.  
5. Scegliere l'azione **Crea fattura di vendita**.
6. Nella pagina **Commessa - Crea fattura vendita**, immettere la data di registrazione e se si desidera creare una nuova fattura o aggiungere questa fattura a una esistente.
7. Scegliere il pulsante **OK**.  
8. Nella pagina **Righe pianificazione commessa** scegliere l'azione **Fatture/Note credito vendite**.

    Verrà visualizzata la pagina **Fatture di vendita** nella quale sarà mostrata la quantità che è stata trasferita in fattura.
9. Apportare tutte le modifiche aggiuntive, quindi scegliere l'azione **Registra**.

> [!NOTE]  
>   La procedura sopra riportata è simile per la creazione, la revisione e la registrazione di una nota di credito di vendita correlata a una commessa.


## <a name="see-also"></a>Vedere anche
[Gestione di progetti](projects-manage-projects.md)  
[Finanze](finance.md)  
[Acquisti](purchasing-manage-purchasing.md)         
[Vendite](sales-manage-sales.md)      
[Utilizzo di [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
