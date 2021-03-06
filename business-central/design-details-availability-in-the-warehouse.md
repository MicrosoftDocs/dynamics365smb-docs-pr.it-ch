---
title: 'Dettagli di progettazione: Disponibilità nella warehouse | Microsoft Docs'
description: Il sistema deve mantenere un controllo costante sulla disponibilità degli articoli nella warehouse, in modo che gli ordini in uscita possano fluire senza problemi e le spedizioni possano essere ottimizzate.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 06/08/2021
ms.author: edupont
ms.openlocfilehash: 184591134706432ed1ea04afa86e1274b748cfe0
ms.sourcegitcommit: 0953171d39e1232a7c126142d68cac858234a20e
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 06/09/2021
ms.locfileid: "6215521"
---
# <a name="design-details-availability-in-the-warehouse"></a>Dettagli di progettazione: Disponibilità nella warehouse
Il sistema deve mantenere un controllo costante sulla disponibilità degli articoli nella warehouse, in modo che gli ordini in uscita possano fluire senza problemi e le spedizioni possano essere ottimizzate.  

La disponibilità varia in base alle allocazioni a livello di collocazione quando si verificano le attività di warehouse ad esempio i prelievi e i movimenti e quando il sistema di impegno magazzino impone limitazioni da soddisfare. Un algoritmo piuttosto complesso verifica che tutte le condizioni siano soddisfatte prima di assegnare le quantità ai prelievi per i flussi in uscita.

Se una o più condizioni non sono soddisfatte, è possibile che vengano visualizzati differenti messaggi di errore, compreso il messaggio generico "Niente da gestire". da gestire". Il messaggio "Niente da gestire" può essere visualizzato per varie ragioni, nei flussi in uscita e in entrata, dove una riga di documento inclusa direttamente o indirettamente contiene il campo **Qtà da gestire**.

> [!NOTE]
> Informazioni sulle possibili ragioni e sulle soluzioni per "Niente da gestire" saranno pubblicate presto qui. da gestire".

## <a name="bin-content-and-reservations"></a>Collocazione e impegno collocazione  
 In qualsiasi installazione della gestione della warehouse, le quantità articolo esistono sia come movimenti warehouse, nell'area dell'applicazione Warehouse, sia come movimenti contabili articoli, nell'area dell'applicazione Magazzino. Questi due tipi di movimento contengono informazioni differenti sulla posizione degli articolo e sulla loro disponibilità. I movimenti warehouse definiscono la disponibilità di un articolo per collocazione e per tipo di collocazione, che è denominato anche contenuto collocazione. I movimenti contabili articoli definiscono la disponibilità di un articolo in base al relativo impegno verso i documenti in uscita.  

 La funzionalità speciale nell'algoritmo di prelievo consente di calcolare la quantità disponibile per il prelievo quando il contenuto collocazione viene associato a degli impegni.  

## <a name="quantity-available-to-pick"></a>Quantità disponibile per il prelievo  
 Se, ad esempio, l'algoritmo di prelievo non considera le quantità di articoli che sono impegnate per una spedizione di ordine di vendita in attesa, tali articoli potrebbero essere prelevati per un altro ordine di vendita che viene spedito prima, impedendo così il completamento della prima vendita. Per evitare questa situazione, l'algoritmo di prelievo sottrae le quantità impegnate per altri documenti in uscita, le quantità nei documenti di prelievo esistenti e le quantità che sono prelevate ma non ancora spedite o consumate.  

 Il risultato viene visualizzato nel campo **Qtà disponibile da prelevare** della pagina **Prospetto prelievi**, dove il campo viene calcolato dinamicamente. Il valore viene calcolato anche quando gli utenti creano prelievi warehouse direttamente per i documenti in uscita. Tali documenti in uscita potrebbero essere ordini di vendita, consumo di produzione o trasferimenti in uscita, dove il risultato viene riflesso nei campi quantità correlati, ad esempio **Qtà da gestire**.  

> [!NOTE]  
>  Per quanto riguarda la priorità degli impegni, la quantità da impegnare viene sottratta dalla quantità disponibile per il prelievo. Ad esempio, se la quantità disponibile nelle collocazioni di prelievo è 5 unità, ma 100 unità si trovano nelle collocazioni di stoccaggio, quando si tenta di impegnare più di 5 unità per un altro ordine, verrà visualizzato un messaggio di errore perché la quantità supplementare deve essere disponibile nelle collocazioni di prelievo.  

### <a name="calculating-the-quantity-available-to-pick"></a>Calcolo della quantità disponibile da prelevare  
 La quantità disponibile da prelevare viene calcolata come segue:  

 quantità disponibile per il prelievo = quantità in collocazioni prelievo - quantità in prelievi e movimenti - (quantità impegnata in collocazioni prelievo + quantità impegnata in prelievi e movimenti)  

 Nel seguente diagramma vengono mostrati i differenti elementi del calcolo.  

 ![Disponibile per il prelievo, con sovrapposizione di impegno](media/design_details_warehouse_management_availability_2.png "Disponibile per il prelievo, con sovrapposizione di impegno")  

## <a name="quantity-available-to-reserve"></a>Quantità disponibile da impegnare  
 Poiché i concetti del contenuto delle condizioni e dell'impegno coesistono, la quantità di articoli disponibili per l'impegno deve essere allineata alle allocazioni ai documenti di warehouse in uscita.  

 Deve essere possibile impegnare tutti gli articoli in magazzino, tranne quelli per cui è stata avviata l'elaborazione in uscita. Di conseguenza, la quantità disponibile per l'impegno è definita come quantità su tutti i documenti e in tutti i tipi di collocazione, ad eccezione delle seguenti quantità in uscita:  

-   Quantità nei documenti di prelievo non registrati  
-   Quantità in collocazioni di spedizione  
-   Quantità nelle collocazioni articoli per produzione  
-   Quantità nelle collocazioni produzione aperte  
-   Quantità nelle collocazioni di assemblaggio  
-   Quantità nelle collocazioni di rettifica  

 Il risultato viene visualizzato nel campo **Quantità totale disponibile** della pagina **Impegni**.  

 In una riga di impegno, la quantità che non può essere impegnata, in quanto è allocata nella warehouse, viene visualizzata nel campo **Qtà. allocata in warehouse** della pagina **Impegni**.  

### <a name="calculating-the-quantity-available-to-reserve"></a>Calcolo della quantità disponibile da impegnare  
 La quantità disponibile da impegnare viene calcolata come segue:  

 quantità disponibile per l'impegno = quantità totale a magazzino - quantità in prelievi e movimenti per i documenti di origine - quantità impegnata - quantità in collocazioni in uscita  

 Nel seguente diagramma vengono mostrati i differenti elementi del calcolo.  

 ![Disponibile per la prenotazione, per allocazioni warehouse](media/design_details_warehouse_management_availability_3.png "Disponibile per la prenotazione, per allocazioni warehouse")  

## <a name="see-also"></a>Vedere anche  
 [Dettagli di progettazione: Gestione warehouse](design-details-warehouse-management.md)  
 [Visualizzare la disponibilità di articoli](inventory-how-availability-overview.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]