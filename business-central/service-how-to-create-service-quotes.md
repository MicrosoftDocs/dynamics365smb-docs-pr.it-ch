---
title: Come creare offerte di assistenza
description: Scopri come usare un'offerta di assistenza come bozza preliminare di un ordine di assistenza e può essere in seguito convertita in un ordine.
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: null
ms.date: 06/23/2021
ms.author: bholtorf
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---
# <a name="create-service-quotes"></a>Creare offerte di assistenza
Le offerte di assistenza possono essere considerate come ordini di assistenza di base. In effetti, sono quasi identici. Entrambi includono informazioni come l'identità del cliente, il tipo di ordine, l'articolo che necessita di assistenza, nonché informazioni di fatturazione, spedizione e relative al lavoro di assistenza effettivo.
 
Un'offerta di assistenza può essere utilizzata come bozza preliminare di un ordine di assistenza e può essere in seguito convertita in un ordine.  
  
## <a name="to-create-a-service-quote"></a>Per creare un'offerta di assistenza
1. Scegli la ![lampadina che apre la funzione Dimmi.](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immetti **Offerte assistenza**, quindi scegli il collegamento correlato.  
2. Creare una nuova offerta di assistenza.  
3. Nel campo **Nr.** immettere un numero per l'offerta di assistenza. In alternativa, se hai impostato una numerazione per le offerte di assistenza nella pagina **Setup gest. assist.**, puoi selezionare <kbd>INVIO</kbd> per selezionare il successivo numero di offerta di assistenza disponibile.  
4. Nel campo **Nr. cliente**  selezionare il cliente appropriato dalla lista.  

  > [!Note]  
  >  I campi del cliente vengono compilati automaticamente con le informazioni della scheda **Cliente**. Se una scheda **Cliente** non esiste per il cliente in questione ed è stato impostato un modello cliente, è possibile creare il cliente a partire dall'offerta di assistenza. Compilare i campi appropriati e scegliere l'azione **Crea cliente**.  
  
5. In base alle impostazioni nella Scheda dettaglio **Campi obbligatori** della pagina **Setup gest. assist.** potrebbe essere necessario compilare il campo **Tipo ordine assistenza** e il campo **Cod. agente**.  
6. Compilare le righe di articolo in assistenza.  
7. Registrare i costi previsti nelle righe di assistenza.  
  
## <a name="see-also"></a>Vedere anche
[Creare ordini di assistenza](service-how-to-create-service-orders.md)  
[Utilizzare i compiti di assistenza](service-how-to-work-on-service-tasks.md)  

 

[!INCLUDE[footer-include](includes/footer-banner.md)]
