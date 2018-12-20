---
title: Come impostare un servizio di scambio documenti | Microsoft Docs
description: Utilizzare un provider di servizi esterno per scambiare documenti elettronici con i partner commerciali.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: d785dfd1a9c3879fc0ddfc79c7c254adbc2ddb52
ms.contentlocale: it-ch
ms.lasthandoff: 09/28/2018

---
# <a name="set-up-a-document-exchange-service"></a>Impostare un servizio di scambio documenti
Utilizzare un provider di servizi esterno per scambiare documenti elettronici con i partner commerciali. Per ulteriori informazioni, vedere [Scambio di dati in modalità elettronica](across-data-exchange.md).  

## <a name="to-set-up-a-document-exchange-service"></a>Per impostare un servizio di Exchange per documenti  
1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Setup servizio scamb. doc.** e quindi scegliere il collegamento correlato.  
2. Compilare i campi come indicato nella tabella seguente.  

    |Campo|Descrizione|  
    |---------------------------------|---------------------------------------|  
    |**Agente utente**|Immettere un testo che può essere utilizzato per identificare la società nei processi di scambio documenti.|  
    |**ID tenant scamb. doc.**|Immettere il tenant nel servizio di Exchange per documenti che rappresenta la società. Questa chiave viene fornita dal provider di servizi di scambio documenti.|  
    |**Abilitato**|Specificare se il servizio è abilitato. **Nota:** Non appena si abilita il servizio, vengono creati almeno due movimenti della coda processi per elaborare il traffico dei documenti elettronici in entrata e in uscita di [!INCLUDE[d365fin](includes/d365fin_md.md)]. Quando si disabilita il servizio, i movimenti della coda processi vengono eliminati.|  
    |**URL iscrizione**|Specificare la pagina Web a cui viene effettuata l'iscrizione per il servizio di Exchange per documenti.|  
    |**URL servizio**|Specificare l'indirizzo del servizio di Exchange per documenti che verrà chiamato quando si inviano e ricevono documenti elettronici.|  
    |**URL accesso**|Specificare la pagina di accesso del servizio di Exchange per documenti, cioè il punto in cui si immettono il nome utente della società e la password per accedere al servizio.|  
    |**Chiave cliente**|Immettere la chiave OAuth basata su transazioni a tre per la chiave del cliente. Questa chiave viene fornita dal provider di servizi di scambio documenti.|  
    |**Domanda segreta cliente**|Immettere il segreto che protegge la chiave del cliente. Questa chiave viene fornita dal provider di servizi di scambio documenti.|  
    |**Token**|Immettere la chiave OAuth basata su transazioni a tre per il token. Questa chiave viene fornita dal provider di servizi di scambio documenti.|  
    |**Domanda segreta token**|Immettere il segreto che protegge il token. Questa chiave viene fornita dal provider di servizi di scambio documenti.|  

    > [!NOTE]  
    > I dati di accesso vengono automaticamente crittografati.

## <a name="see-also"></a>Vedi anche  
[Impostazione dello scambio di dati](across-set-up-data-exchange.md)  
[Scambio di dati in modalità elettronica](across-data-exchange.md)
