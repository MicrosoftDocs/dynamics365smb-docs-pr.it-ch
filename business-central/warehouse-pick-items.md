---
title: Prelievo degli articoli
description: L'attività di prelievo degli articoli prima della spedizione o dell'utilizzo viene eseguita in modi diversi a seconda della configurazione delle funzionalità di gestione warehouse.
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.form: 5779, 5798, 7343, 7345, 7357, 7359, 7377, 7392, 7395, 7397, 9313, 9316, 9344
ms.date: 06/25/2021
ms.author: edupont
ms.openlocfilehash: 07cb13480146496c7186cef2d845c4a799eb699a
ms.sourcegitcommit: 3acadf94fa34ca57fc137cb2296e644fbabc1a60
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 09/19/2022
ms.locfileid: "9535602"
---
# <a name="pick-items"></a>Prelievo degli articoli

L'attività di warehouse di prelievo degli articoli prima della spedizione o dell'utilizzo viene eseguita in modi diversi a seconda della configurazione delle funzionalità di gestione warehouse. La complessità può andare dall'assenza delle funzionalità di warehouse, alle configurazioni di warehouse di base per la gestione ordine per ordine in una o più attività, fino alle configurazioni avanzate in cui tutte le attività di warehouse devono essere eseguite in un flusso di lavoro guidato. Per ulteriori informazioni, vedere [Impostazione gestione warehouse](warehouse-setup-warehouse.md).

Se si decide di organizzare e di registrare l'attività di prelievo associata a documenti di warehouse, inserire un segno di spunta nel campo **Richiesto prelievo** nella scheda Ubicazione. Ciò indica che, nel caso di articoli che devono essere prelevati per un documento di origine in uscita, il prelievo dovrà essere controllato dal sistema. Un documento di origine in uscita può essere un ordine di vendita, un ordine di reso da acquisto, un ordine di trasferimento in uscita, un ordine di assistenza o un ordine di produzione di cui è richiesto il prelievo dei componenti.

> [!NOTE]
> Anche se l'impostazione è chiamata **Richiesto prelievo**, è possibile registrare carichi e spedizioni direttamente dal documento aziendale di origine nell'ubicazione in cui si seleziona questa casella di controllo.

Se l'ubicazione è impostata per la richiesta dell'elaborazione del prelievo, ma non della spedizione, è necessario utilizzare la pagina **Prelievo magazzino** per organizzare le informazioni relative al prelievo, stamparle, immettere i risultati del prelievo e registrare tali informazioni, operazioni che comportano anche la spedizione degli articoli. Nel caso del prelievo di componenti per un ordine di produzione, la registrazione del prelievo comprende anche il consumo.

Se l'ubicazione è impostata in modo da richiedere l'elaborazione di prelievi e di spedizioni, inserendo un segno di spunta nei campi **Richiesta prelievo** e **Richiesta spedizione** della scheda Ubicazione, occorrerà utilizzare la pagina **Prelievo warehouse** per gestire il prelievo. Il prelievo warehouse presenta un funzionamento analogo a quello di magazzino, ad eccezione del fatto che invece di registrare le informazioni sul prelievo viene registrato il prelievo stesso. Tale processo non include la registrazione della spedizione ma semplicemente rende disponibili gli articoli per la spedizione. Il responsabile di warehouse può utilizzare i prospetti prelievi per organizzare le informazioni di prelievo prima di creare le istruzioni di prelievo dalla singola warehouse.

Nella tabella seguente viene descritta una sequenza di task, con collegamenti agli argomenti che li descrivono.   

|**Per**|**Vedere**|
|------------|-------------|  
|Registrare la spedizione degli articoli direttamente nel documento ordine in uscita in quanto non sono disponibili funzionalità di warehouse. (Funzionamento analogo per ordini di vendita, ordini di trasferimento in uscita e spedizioni di reso.)|[Spedire articoli](warehouse-how-ship-items.md)|  
|Prelevare gli articoli ordine per ordine e registrare la spedizione nella stessa attività, in una configurazione di base della warehouse.|[Prelevare articoli con prelievi magazzino](warehouse-how-to-pick-items-with-inventory-picks.md)|
|Prelevare gli articoli per più ordini in una configurazione avanzata della warehouse.|[Prelevare articoli con prelievi warehouse](warehouse-how-to-pick-items-for-warehouse-shipment.md)|  
|Prelevare i componenti per la produzione o l'assemblaggio in una configurazione di base della warehouse.|[Prelevare per produzione o assemblaggio in configurazioni di warehouse di base](warehouse-how-to-pick-for-production.md)|
|Prelevare i componenti per la produzione o l'assemblaggio in una configurazione avanzata della warehouse.|[Prelevare per produzione o assemblaggio in configurazioni di warehouse avanzate](warehouse-how-to-pick-for-internal-operations-in-advanced-warehousing.md)|  
|Pianificare istruzioni di prelievo ottimizzate per diverse spedizioni anziché lasciare che i lavoratori warehouse agiscano direttamente sulle spedizioni registrate.|[Pianificare prelievi nei prospetti](warehouse-how-to-plan-picks-in-worksheets.md)|  
|Prelevare tecnicamente gli articoli per uno scopo specifico, ad esempio per un'unità di produzione che necessita di componenti aggiuntivi, in modo che gli articoli non escano tecnicamente dalla warehouse.|[Selezionare e stoccare senza un documento di origine](warehouse-how-to-create-put-aways-from-internal-put-aways.md)|
|Comprendere come prelevare automaticamente gli articoli in base alla loro data di scadenza, ad esempio beni deperibili.|[Prelievo in base al metodo FEFO](warehouse-picking-by-fefo.md)|
|Dividere una riga di prelievo in più righe, ad esempio perché non vi sono articoli sufficienti da prelevare nella collocazione designata.|[Suddividere righe attività warehouse](warehouse-how-to-split-warehouse-activity-lines.md)|
|Ottenere accesso immediato ai prelievi che sono stati assegnati a un lavoratore della warehouse.|[Individuare le assegnazioni della warehouse](warehouse-how-to-find-your-warehouse-assignments.md)|  

## <a name="see-related-microsoft-training"></a>Vedi il relativo [training Microsoft](/training/paths/pick-ship-items-business-central/)

## <a name="see-also"></a>Vedere anche

[Warehouse Management](warehouse-manage-warehouse.md)  
[Magazzino](inventory-manage-inventory.md)  
[Impostazione Warehouse Management](warehouse-setup-warehouse.md)  
[Gestione assemblaggio](assembly-assemble-items.md)  
[Dettagli di progettazione: Warehouse Management](design-details-warehouse-management.md)  
[Utilizzare [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
