---
title: Come impostare solleciti di consegna
description: In Business Central, è possibile usare solleciti di consegna per segnalare ai fornitori le consegne scadute.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: bacb809ae0dddc3989a9150ad40e8d947e7b36a1
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 10/01/2019
ms.locfileid: "2300989"
---
# <a name="set-up-delivery-reminders"></a>Impostare solleciti di consegna
In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], è possibile usare solleciti di consegna per segnalare ai fornitori le consegne scadute. Per creare solleciti di consegna per i fornitori, è necessario impostare dati di base per la creazione di solleciti di consegna e numerazioni per i solleciti di consegna nella pagina **Setup contabilità fornitori e acquisti**.  

## <a name="to-set-up-delivery-reminders"></a>Per impostare solleciti di consegna  

1.  Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Setup contabilità fornitori e acquisti**, quindi scegliere il collegamento correlato.  
2.  Nella Scheda dettaglio **Generale**, nel campo **Data sollecito eliminato di default** specificare una delle opzioni seguenti come descritto in questa tabella.  

    |Opzione|Descrizione|  
    |----------------------------------|---------------------------------------|  
    |**Data di carico richiesta**|Specifica che il valore della data nel campo **Data di carico richiesta** sulla riga ordine di acquisto verrà usato come data di default per la creazione di solleciti di consegna.|  
    |**Data di carico promessa**|Specifica che il valore della data nel campo **Data di carico promessa** sulla riga ordine di acquisto verrà usato come data di default per la creazione di solleciti di consegna.|  
    |**Data carico prevista**|Specifica che il valore della data nel campo **Data carico prevista** sulla riga ordine di acquisto verrà usato come data di default per la creazione di solleciti di consegna.|  

3.  Nella Scheda Dettaglio **Numerazione** compilare i campi come indicato nella tabella seguente.  

    |Campo|Descrizione|  
    |---------------------------------|---------------------------------------|  
    |**Nr. Solleciti Consegna**|Codice numerazione per i solleciti di consegna.|  
    |**Nr. Solleciti Consegna Emessi**|Codice numerazione per i solleciti di consegna inviati.|  

4.  Scegliere il pulsante **OK**.  

## <a name="see-also"></a>Vedi anche  
 [Solleciti consegna](delivery-reminders.md)   
 [Impostare i termini, i livelli e i testi di sollecito di consegna](how-to-set-up-delivery-reminder-terms-levels-and-text.md)   
 [Assegnare codici di solleciti di consegna ai fornitori](how-to-assign-delivery-reminder-codes-to-vendors.md)   
 [Creare solleciti di consegna manualmente](how-to-create-delivery-reminders-manually.md)
