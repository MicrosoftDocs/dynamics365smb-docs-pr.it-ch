---
title: Impostare l'assegnazione delle risorse | Documenti Microsoft
description: "Informazioni su come il sistema può aiutare a garantire che l'assegnazione venga fatta a chi ha le competenze necessarie per fornire a un servizio di assistenza."
services: project-madeira
documentationcenter: 
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: resource, skill, service, zones
ms.date: 10/01/2018
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 7ce128aa32d650cf756117ab46987167d9a3781a
ms.contentlocale: it-ch
ms.lasthandoff: 09/28/2018

---

# <a name="set-up-resource-allocation"></a>Impostare l'assegnazione delle risorse
Per assicurarsi che un compito di assistenza sia eseguito correttamente, è importante trovare una risorsa qualificata per il lavoro. È possibile configurare [!INCLUDE[d365fin](includes/d365fin_md.md)] di modo che sia semplice assegnare una risorsa che disponga delle competenze necessarie per il compito. In [!INCLUDE[d365fin](includes/d365fin_md.md)] questa funzionalità è detta _assegnazione delle risorse_. È possibile assegnare le risorse in base alla loro competenza, disponibilità o se si trovano nella stessa zona di assistenza del cliente. 

Per utilizzare l'assegnazione delle risorse, è necessario impostare:  
  
* Le competenze necessarie per riparare e gestire gli articoli in assistenza. Queste devono essere assegnate agli articoli in assistenza e alle risorse.  
* Le aree geografiche, chiamate zone, definite per il proprio mercato. Ad esempio, Est, Ovest, Centro e così via. Queste devono essere assegnate ai clienti e alle risorse.  
* Scegliere se visualizzare le zone e le competenze delle risorse e se visualizzare un avviso quando qualcuno sceglie una risorsa non qualificata o che non si trova nella zona cliente.  

## <a name="to-set-up-skills"></a>Per impostare le competenze
1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Competenze** e quindi scegliere il collegamento correlato.  
2. Compilare i campi come necessario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

## <a name="to-assign-skills-to-service-items-and-resources"></a>Per assegnare le competenze agli articoli in assistenza e alle risorse
1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Articoli** o **Risorse**e quindi scegliere il collegamento correlato.  
2. Aprire la scheda relativa all'articolo in assistenza o alla risorsa, quindi scegliere una delle seguenti opzioni:  
  
    * Per gli articoli in assistenza, scegliere **Competenze risorse**.  
    * Per le risorse, scegliere **Competenze**.  

## <a name="to-set-up-zones"></a>Per impostare le zone
1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Zone** e quindi scegliere il collegamento correlato.  
2. Compilare i campi come necessario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

## <a name="to-assign-zones-to-customers-and-resources"></a>Per assegnare le zone ai clienti e alle risorse 
1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Clienti** o **Risorse**e quindi scegliere il collegamento correlato.  
2. Aprire la scheda relativa all'articolo in assistenza o alla risorsa, quindi scegliere una delle seguenti opzioni:  
  
    * Per i clienti, scegliere una zona nel campo **Codice zona di assistenza**.  
    * Per le risorse, scegliere l'azione **Zone assistenza**.  

## <a name="to-specify-what-to-show-when-a-resource-is-chosen"></a>Per specificare il contenuto da visualizzare quando si sceglie una risorsa
1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Setup assistenza** e quindi scegliere il collegamento correlato. 
2. Nel campo **Opzione competenze risorse** scegliere una delle opzioni descritte nella seguente tabella.  
  
    |**Opzione**|**Description**|  
    |------------|-------------|  
    |Mostra codice | Viene visualizzato solo il codice.|  
    |Warning visualizzato | Le informazioni vengono visualizzate e appare un avviso se si sceglie una risorsa che non è qualificata.|  
    |Non usato | Le informazioni non vengono visualizzate.|  

## <a name="to-update-resource-capacity"></a>Per aggiornare la capacità della risorsa  
Potrebbe essere necessario modificare la capacità delle risorse.  
  
1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Capacità** e quindi scegliere il collegamento correlato.  
2. Scegliere la risorsa, quindi scegliere l'azione **Imposta capacità**.  
3. Apportare le modifiche, quindi scegliere **Aggiorna capacità**.  

## <a name="to-update-skills-for-items-service-items-or-service-item-groups"></a>Per aggiornare le competenze per gli articoli, gli articoli in assistenza o i gruppi di articoli in assistenza
Se si desidera modificare i codici competenza assegnati agli articoli, ad esempio da **PC** a **PCS**, è possibile effettuare questa operazione per un articolo, un articolo in assistenza o per tutti gli articoli in un gruppo di articoli in assistenza.  
  
1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Articoli**, **Articolo assistenza** o **Gruppo articoli in assistenza** e quindi scegliere il collegamento correlato.  
2. Scegliere l'entità da aggiornare, quindi scegliere l'azione **Competenze risorse**.  
3. Sulla riga contenente il codice da modificare, nel campo **Codice competenza**, scegliere il codice competenza appropriato.  
4.  Se all'articolo sono associati articoli in assistenza, verrà visualizzata una finestra di dialogo con le due opzioni seguenti:  
  
    * Modificare i codici competenze nel valore selezionato: selezionare questa opzione per sostituire il vecchio codice con il nuovo in tutti gli articoli in assistenza correlati.  
    * Eliminare i codici competenze o aggiornarne la relazione: selezionare questa opzione se si desidera modificare il codice competenza solo per l'articolo selezionato. Il codice competenza degli articoli in assistenza correlati verrà riassegnato, ovvero, il campo **Assegnato da** verrà aggiornato.  
  
## <a name="see-also"></a>Vedi anche
[Assegnare risorse](service-how-to-allocate-resources.md)  
[Impostare le ore di lavoro e le ore di assistenza](service-how-setup-work-service-hours.md)  
[Impostare il reporting dei guasti](service-how-setup-fault-reporting.md)  
[Impostare codici per servizi standard](service-how-setup-service-coding.md)  
 

