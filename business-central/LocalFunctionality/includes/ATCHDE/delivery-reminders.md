---
author: edupont04
ms.service: dynamics365-business-central
ms.topic: include
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 1e7cb126ea06d96bd130d644948d08fd7e2e1a11
ms.sourcegitcommit: 428f180604e5afcf94fa0e92a0615f58c88e13cd
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 10/02/2020
ms.locfileid: "3959661"
---
I solleciti di consegna sono usati per tracciare le consegne scadute dei fornitori e per segnalare ai fornitori le consegne scadute. Per creare i solleciti di consegna è necessario impostare quanto segue:

- Termini di sollecito di consegna  

    I termini di sollecito di consegna sono identificati da un codice che deve essere assegnato ai fornitori. Per utilizzare più di una combinazione delle impostazioni, è necessario impostare un codice per ciascuna di esse separatamente. È possibile impostare un numero qualsiasi di termini di sollecito di consegna.  

- Livelli del sollecito di consegna  

    Per ogni termine di sollecito di consegna, è necessario impostare i livelli di sollecito di consegna. Questi livelli determinano la frequenza di creazione dei promemoria di consegna per un determinato termine. Il livello 1 è il primo sollecito di consegna creato per una consegna scaduta. Il livello 2 è il secondo sollecito di consegna e così via. Quando vengono creati i solleciti di consegna, viene considerato il numero di solleciti creati in precedenza e il numero corrente viene utilizzato per applicare i termini.  

- Messaggi di testo di sollecito di consegna  

    Per ogni livello di sollecito di consegna, è necessario impostare i messaggi di testo di sollecito di consegna. Sono disponibili due tipi di messaggi di testo di sollecito di consegna: iniziale e finale. Il messaggio di testo iniziale viene stampato sotto la sezione intestazione, prima dell'elenco delle voci contrassegnate per il sollecito. Il messaggio di testo finale viene stampato dopo questo elenco.  

Dopo aver impostato i testi, i livelli e i termini di consegna, è necessario assegnare ai fornitori i codici del sollecito di consegna.  

È possibile creare i solleciti di consegna manualmente o automaticamente. È possibile usare il processo batch **Crea sollecito di consegna** per creare automaticamente i solleciti di consegna in modo da poter selezionare gli ordini di acquisto per i quali è necessario creare i solleciti di consegna.  

È possibile anche tracciare i documenti in relazione alle righe degli ordini di vendita e di acquisto.  

[!INCLUDE[d365fin](../../../includes/d365fin_md.md)] fornisce i seguenti report:  

- **Sollecito di consegna inviato** - Per visualizzare i solleciti di consegna per i fornitori.  
- **Sollecito di consegna - Test** - Per verificare i solleciti di consegna prima dell'invio.  
