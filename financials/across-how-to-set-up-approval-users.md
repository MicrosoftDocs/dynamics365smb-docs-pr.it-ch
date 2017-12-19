---
title: Come impostare gli utenti per l'approvazione | Microsoft Docs
description: "Prima di creare flussi di lavoro che coinvolgono passaggi di approvazione, è necessario impostare gli utenti del flusso di lavoro coinvolti nei processi di approvazione. Nella finestra Setup utente approvazione è possibile anche impostare i limiti quantitativi per specifici tipi di richiesta e definire i responsabili di approvazione sostitutivi ai quali vengono delegate le richieste di approvazione in assenza del responsabile originale."
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
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 49ffa181e653377f3684d138b6ee7df3775a87f6
ms.contentlocale: it-ch
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-set-up-approval-users"></a>Procedura: Impostare gli utenti per l'approvazione
Prima di creare workflow che coinvolgono passaggi di approvazione, è necessario impostare gli utenti del workflow coinvolti nei processi di approvazione. Nella finestra **Setup utente approvazione** è possibile anche impostare i limiti quantitativi per specifici tipi di richiesta e definire i responsabili di approvazione sostitutivi ai quali vengono delegate le richieste di approvazione in assenza del responsabile originale.  

> [!NOTE]  
>  Gli utenti dell'approvazione, sia i richiedenti sia i responsabili dell'approvazione, devono innanzitutto essere impostati come utenti del workflow nella finestra **Gruppo di utenti del workflow**. Per ulteriori informazioni, vedere [Procedura: Impostare gli utenti del workflow](across-how-to-set-up-workflow-users.md).  

 Una volta impostati questi utenti, è possibile utilizzare l'impostazione per creare le risposte del flusso di lavoro per i flussi di lavoro di approvazione. Per ulteriori informazioni, vedere il passaggio 9 in [Procedura: Creare workflow](across-how-to-create-workflows.md).  

> [!NOTE]  
>  Per definire che una richiesta di approvazione non venga approvata fino a che non venga approvata da più responsabili di una catena di approvazione, impostare i responsabili di approvazione in una gerarchia. Per il tipo **Responsabile approvazione**, impostare i responsabili approvazione nella finestra **Setup utente approvazione**. Per il tipo **Gruppo di utenti del workflow**, impostare i responsabili di approvazione nella finestra **Gruppi di utenti del workflow** e definire la gerarchia assegnando numeri incrementali a ogni responsabile nel campo **Nr. sequenza** . Per ulteriori informazioni, vedere questo argomento e [Procedura: Impostare gli utenti del workflow](across-how-to-set-up-workflow-users.md).  
>   
>  Per definire che una richiesta di approvazione non venga approvata fino a che non venga approvata da più responsabili uguali, indipendentemente da una gerarchia, impostare un normale gruppo di utenti del flusso di lavoro. Per il tipo **Gruppo di utenti del workflow**, impostare i responsabili di approvazione nella finestra **Gruppi di utenti del workflow** e assegnare lo stesso numero a ogni responsabile nel campo **Nr. sequenza** . Per ulteriori informazioni, vedere [Procedura: Impostare gli utenti del workflow](across-how-to-set-up-workflow-users.md).  

## <a name="to-set-up-an-approval-user"></a>Per impostare un utente per l'approvazione  
1. Scegliere l'icona ![Cerca pagina o report](media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Setup utente approvazione**, quindi scegliere il collegamento correlato.  
2. Nella finestra **Setup utente approvazione** creare una nuova riga e compilare i campi come descritto nella tabella seguente.  

    |Campo|Description|  
    |---------------------------------|---------------------------------------|  
    |**ID utente**|Selezionare l'ID utente dell'utente coinvolto nel processo di approvazione.|  
    |**Codice agente/addetto acquisti**|Specificare il codice dell'agente o dell'addetto acquisti valido per l'utente nel campo **Codice agente/addetto acquisti**.<br /><br /> In genere si compila il campo **Codice agente/addetto acquisti** se l'agente o l'addetto acquisti che è responsabile del cliente o de fornitore è anche la persone che deve approvare la richiesta di vendite o di acquisto in questione.|  
    |**ID resp. approvazione**|Selezionare l'ID dell'utente che deve approvare le richieste effettuate dall'utente nel campo **ID utente** .|  
    |**Limite importo approvazione ordine**|Specificare l'importo di vendita massimo in valuta locale che l'utente nel campo  **ID utente** può approvare.|  
    |**Approvazione vendite illimitate**|Specificare che l'utente nel campo **ID utente** può approvare tutte le richieste di vendita indipendentemente dall'importo.<br /><br /> Se si seleziona questa casella di controllo, non è possibile compilare il campo **Limite importo approvazione ordine**.|  
    |**Limite approvazione importo acquisto**|Specificare l'importo di acquisto massimo in valuta locale che l'utente nel campo  **ID utente** può approvare.|  
    |**Approvazione acquisti illimitati**|Specificare che l'utente nel campo **ID utente** può approvare tutte le richieste di acquisto indipendentemente dall'importo.<br /><br /> Se si seleziona questa casella di controllo, non è possibile compilare il campo **Limite importo approvazione ordine**.|  
    |**Limite importo approvazione richiesta**|Specificare l'importo massimo in valuta locale che l'utente nel campo **ID utente**  può approvare per le offerte di acquisto.<br /><br /> Per utilizzare questo campo, è necessario selezionare l'opzione **Catena responsabili approvazione** nel campo **Tipo di limite responsabile approvazione** della finestra **Risposta workflow**.|  
    |**Approvazione richieste illimitate**|Specificare che l'utente nel campo **ID utente** può approvare tutte le offerte di acquisto indipendentemente dall'importo.<br /><br /> Se si seleziona questa casella di controllo, non è possibile compilare il campo **Limite importo approvazione richiesta**.|  
    |**Sostituto**|Selezionare l'ID dell'utente che deve approvare le richieste effettuate dall'utente nel campo **ID utente** se l'utente nel campo **ID resp. approvazione** non è disponibile. **Nota:** Il sostituto può essere l'utente nel campo **Sostituto**, il responsabile approvazione diretto o l'amministratore approvazioni, in tale ordine di priorità. Per ulteriori informazioni, vedere [Procedura: Utilizzo dei workflow di approvazione](across-how-use-approval-workflows.md).|  
    |**Indirizzo e-mail**|Specificare l'indirizzo e-mail dell'utente nel campo **ID utente**.|  
    |**Amministratore approvazioni**|Specificare l'utente che dispone dei diritti per sbloccare i flussi di lavoro di approvazione, ad esempio, delegando le richieste di approvazione a nuovi responsabili sostitutivi ed eliminando le richieste di approvazione scadute.|  

    > [!NOTE]  
    >  Il comportamento del campo **Tipo di limite responsabile approvazione** si applica solo alle aree di applicazione dove i limiti possono essere definiti, ossia approvazioni di vendita e di acquisto. Qualunque altro tipo di approvazione in cui i limiti non si applicano si comporterà sempre come descritto per l'opzione **Responsabile approvazione diretto**.  

3. Per testare l'impostazione degli utenti per l'approvazione, scegliere l'azione **Test Setup utente approvazione**.  
4. Ripetere i passaggi 2 e 3 per ogni utente che si desidera impostare come utente di approvazione.  

## <a name="see-also"></a>Vedi anche  
[Procedura: Impostare gli utenti del workflow](across-how-to-set-up-workflow-users.md)   
[Impostazione delle notifiche del workflow](across-setting-up-workflow-notifications.md)   
[Procedura: Creare workflow](across-how-to-create-workflows.md)   
[Impostazione dei workflow](across-set-up-workflows.md)   
[Procedura dettagliata: Impostazione e utilizzo di un workflow di approvazione di acquisto](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md)   
[Workflow](across-workflow.md)   
