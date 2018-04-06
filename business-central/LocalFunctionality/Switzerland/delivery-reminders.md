---
title: Solleciti consegna
description: I solleciti di consegna sono usati per tracciare le consegne scadute dei fornitori e per segnalare ai fornitori le consegne scadute.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: a4b9e8d032e95327f1457ec9695df855e175b9a0
ms.contentlocale: it-ch
ms.lasthandoff: 03/22/2018

---
# <a name="delivery-reminders"></a>Solleciti consegna
I solleciti di consegna sono usati per tracciare le consegne scadute dei fornitori e per segnalare ai fornitori le consegne scadute. Per creare i solleciti di consegna è necessario impostare quanto segue:  

- Termini di sollecito di consegna  

    I termini di sollecito di consegna sono identificati da un codice che deve essere assegnato ai fornitori. Per utilizzare più di una combinazione delle impostazioni, è necessario impostare un codice per ciascuna di esse separatamente. È possibile impostare un numero qualsiasi di termini di sollecito di consegna.  

- Livelli del sollecito di consegna  

    Per ogni termine di sollecito di consegna, è necessario impostare i livelli di sollecito di consegna. Questi livelli determinano la frequenza di creazione dei promemoria di consegna per un determinato termine. Il livello 1 è il primo sollecito di consegna creato per una consegna scaduta. Il livello 2 è il secondo sollecito di consegna e così via. Quando vengono creati i solleciti di consegna, viene considerato il numero di solleciti creati in precedenza e il numero corrente viene utilizzato per applicare i termini.  

- Messaggi di testo di sollecito di consegna  

    Per ogni livello di sollecito di consegna, è necessario impostare i messaggi di testo di sollecito di consegna. Sono disponibili due tipi di messaggi di testo di sollecito di consegna: iniziale e finale. Il messaggio di testo iniziale viene stampato sotto la sezione intestazione, prima dell'elenco delle voci contrassegnate per il sollecito. Il messaggio di testo finale viene stampato dopo questo elenco.  

Per ulteriori informazioni, vedere [Impostare termini, livelli e testo dei solleciti di consegna](how-to-set-up-delivery-reminder-terms-levels-and-text.md).  

Dopo aver impostato i termini di consegna, è necessario assegnare ai fornitori i codici del termine di sollecito di consegna. Per ulteriori informazioni, vedere [Assegnare codici di solleciti di consegna ai fornitori](how-to-assign-delivery-reminder-codes-to-vendors.md).  

È possibile creare i solleciti di consegna manualmente o automaticamente. È possibile usare il processo batch **Crea sollecito di consegna** per creare automaticamente i solleciti di consegna. Questo processo batch consente di selezionare gli ordini di acquisto per i quali devono essere creati i solleciti di consegna. Per ulteriori informazioni, vedere [Generare solleciti di consegna](how-to-issue-delivery-reminders.md).  

È possibile anche tracciare i documenti in relazione alle righe degli ordini di vendita e di acquisto.  

[!INCLUDE[d365fin](../../includes/d365fin_md.md)] fornisce i seguenti report:  

- **Sollecito di consegna inviato** - Per visualizzare i solleciti di consegna per i fornitori.  
- **Sollecito di consegna - Test** - Per verificare i solleciti di consegna prima dell'invio.  

Per ulteriori informazioni, vedere [Stampare report di test per i solleciti di consegna](how-to-print-test-reports-for-delivery-reminders.md).  

## <a name="see-also"></a>Vedi anche  
 [Impostare solleciti di consegna](how-to-set-up-delivery-reminders.md)   
 [Impostare i termini, i livelli e i testi di sollecito di consegna](how-to-set-up-delivery-reminder-terms-levels-and-text.md)   
 [Assegnare codici di solleciti di consegna ai fornitori](how-to-assign-delivery-reminder-codes-to-vendors.md)   
 [Generare solleciti di consegna](how-to-generate-delivery-reminders.md)   
 [Creare solleciti di consegna manualmente](how-to-create-delivery-reminders-manually.md)   
 [Emettere solleciti di consegna](how-to-issue-delivery-reminders.md)   
 [Stampare report di test per i solleciti di consegna](how-to-print-test-reports-for-delivery-reminders.md)

