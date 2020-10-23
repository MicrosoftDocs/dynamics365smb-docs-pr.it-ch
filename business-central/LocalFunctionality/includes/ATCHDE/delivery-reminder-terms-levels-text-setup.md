---
author: edupont04
ms.service: dynamics365-business-central
ms.topic: include
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 5ca2eb6fd5972f2494864b61c23bcf6c3ee26a7f
ms.sourcegitcommit: 428f180604e5afcf94fa0e92a0615f58c88e13cd
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 10/02/2020
ms.locfileid: "3959659"
---
Per creare i solleciti di consegna è necessario impostare quanto segue:  

- Termini di sollecito di consegna  
- Livelli del sollecito di consegna  
- Messaggi di testo di sollecito di consegna  

Ogni termine di sollecito di consegna ha due o più livelli di sollecito di consegna e per ogni livello di sollecito di consegna è possibile specificare il testo che fa parte del sollecito di consegna.  

## <a name="to-set-up-delivery-reminder-terms"></a>Per impostare i termini di sollecito di consegna  

1. Scegliere l'![icona a forma di lampadina che consente di aprire la funzionalità delle informazioni](../../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Termini di sollecito consegna** e quindi scegliere il collegamento correlato.  
2. Scegliere l'azione **Nuovo**.  
3. Compilare i campi come indicato nella tabella seguente.  

    |Campo|Descrizione|  
    |---------------------------------|---------------------------------------|  
    |**Codice**|Codice per i termini di sollecito di consegna. È possibile immettere un massimo di 10 caratteri alfanumerici.|  
    |**Descrizione**|Descrizione per i termini di sollecito di consegna. È possibile immettere un massimo di 30 caratteri alfanumerici.|  
    |**Nr. Max di Solleciti Consegna**|Numero massimo di solleciti di consegna che è possibile creare per un ordine.<br /><br /> **NOTA:** questo è il numero massimo per tutti i livelli di sollecito per questo termine di sollecito. Ad esempio, se si impostano tre livelli e si imposta **Numero massimo di solleciti di consegna** su 5, il primo sollecito viene creato al livello 1, il secondo al livello 2 e gli ultimi tre al livello 3.|  

4. Scegliere il pulsante **OK**.  

## <a name="to-add-delivery-reminder-levels-to-a-delivery-reminder-term"></a>Per aggiungere livelli di sollecito di consegna a un termine di sollecito di consegna  

1. Nella pagina **Termini di sollecito di consegna** selezionare il termine di sollecito di consegna per cui si desidera impostare i livelli e scegliere l'azione **Livelli**.  
2. Scegliere l'azione **Nuovo**.  
3. Compilare i campi come indicato nella tabella seguente.  

    |Campo|Descrizione|  
    |---------------------------------|---------------------------------------|  
    |**Nr.**|Numero del livello del sollecito di consegna. Questo campo viene compilato automaticamente.|  
    |**Calcolo data di scadenza**|Formula per il calcolo della data di scadenza per il sollecito di consegna. È possibile immettere una combinazione di numeri da 0 a 9999 e codici di data (G per giorno, GS per il giorno della settimana, S per settimana, M per mese, T per trimestre o A per anno). I codici di data indicano il calcolo della data di scadenza per il sollecito di consegna. È possibile inserire un massimo di 20 caratteri per la formula di calcolo della data di scadenza.|  

4. Scegliere il pulsante **OK**.  

Per ciascun livello di sollecito di consegna è possibile definire messaggi di testo che vengono aggiunti al sollecito di consegna. Definire il testo iniziale che viene aggiunto prima della descrizione dell'ordine di acquisto scaduto e il testo finale che viene aggiunto dopo la descrizione dell'ordine di acquisto scaduto.  

La procedura seguente descrive come impostare i messaggi di testo iniziali, ma gli stessi passaggi si applicano per impostare i messaggi di testo finali.  

## <a name="to-set-up-delivery-reminder-text-messages"></a>Per impostare i messaggi di testo di sollecito di consegna  

1. Nella pagina **Livelli del sollecito di consegna** selezionare un livello e scegliere l'azione **Testo iniziale**.  
2. Scegliere l'azione **Nuovo**.  
3. Nel campo **Descrizione** inserire il messaggio di testo iniziale per il sollecito di consegna.  
4. Scegliere il pulsante **OK**.  
