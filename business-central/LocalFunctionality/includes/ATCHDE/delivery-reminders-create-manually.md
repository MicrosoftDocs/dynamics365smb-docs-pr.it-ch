---
author: brentholtorf
ms.topic: include
ms.date: 11/21/2023
ms.author: bholtorf
---

In [!INCLUDE[prod_short](../../../includes/prod_short.md)] è possibile creare solleciti di consegna quando un acquisto non viene consegnato come previsto. È possibile creare un singolo sollecito di consegna manualmente o generare solleciti di consegna per tutte le consegne scadute.  

> [!NOTE]
> Per creare solleciti di consegna, è necessario impostare i testi, i livelli e i termini del sollecito di consegna.

## <a name="to-create-a-delivery-reminder-manually"></a>Per creare un sollecito di consegna manualmente

1. Scegliere l'icona della ![lampadina che apre la funzionalità delle informazioni.](../../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immettere **Sollecito Consegna**, quindi selezionare il collegamento correlato.  
2. Scegliere l'azione **Nuovo**.  
3. Nella pagina **Sollecito di consegna**, compilare i campi come indicato nella tabella riportata di seguito.  

    |Campo|Descrizione|  
    |---------------------------------|---------------------------------------|  
    |**Nr.**|Numero di identificazione univoco del sollecito di consegna.|  
    |**N. fornitore**|Numero del fornitore per cui si desidera registrare il sollecito di consegna.<br /><br /> Quando si seleziona il numero fornitore, i campi **Nome**, **Indirizzo**, **NPA/Città** e **Contatto** vengono compilati automaticamente.|  
    |**Data di Registrazione**|Data di registrazione per il sollecito di consegna. Tale data viene copiata in tutti i movimenti contabili relativi al sollecito di consegna.|  
    |**Data Documento**|Data del documento per il sollecito di consegna. Questa data è utilizzata anche per calcolare la data di scadenza per il sollecito di consegna. Se necessario, è possibile modificare la data di registrazione.|  
    |**Livello di sollecito**|Livello del sollecito di consegna. Questo valore si basa sul numero di solleciti di consegna inviati.|  
    |**Codice termini di sollecito**|Specifica il codice dei termini del sollecito di consegna impostato per il fornitore.|  
    |**Data scad.**|Data di scadenza per il sollecito di consegna.|  

4. Scegliere l'azione selezionare **Suggerisci riga sollecito**.  

    Se per il fornitore specificato sono presenti consegne scadute, queste vengono aggiunte al sollecito di consegna.  

5. Scegliere il pulsante **OK**.  

    Il sollecito di consegna viene creato. È ora possibile emettere e stampare il sollecito di consegna.  
