---
title: Gestione delle transazioni Intercompany
description: Utilizzando la funzionalità intercompany, è possibile semplificare i processi aziendali e le transazioni tra società all'interno della stessa organizzazione.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: IC, group, consolidation, affiliate, subsidiary
ms.date: 06/02/2021
ms.author: edupont
ms.openlocfilehash: 0a69507b32f8782fe876458adb590529bfd64b20
ms.sourcegitcommit: 1aab52477956bf1aa7376fc7fb984644bc398c61
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 06/04/2021
ms.locfileid: "6184442"
---
# <a name="managing-intercompany-transactions"></a>Gestione delle transazioni Intercompany

Un'organizzazione potrebbe essere costituita da più società, ma non disporre di un numero corrispondente di team contabili e amministrativi. La funzionalità intercompany consente di effettuare operazioni con le filiali e le organizzazioni partner interne esattamente come con i fornitori e i clienti esterni. Le informazioni sulle transazioni intercompany devono essere immesse una sola volta nei documenti appropriati. È possibile utilizzare le funzionalità già conosciute, quali quelle di gestione di crediti e debiti. Le funzionalità di mappatura per il piano dei conti e le dimensioni garantiscono che le informazioni vengano visualizzate nelle posizioni appropriate.  

La funzionalità intercompany offre quattro vantaggi principali:  

- Maggiore produttività grazie alla possibilità di risparmiare tempo e a transazioni più semplici.  
- Riduzione al minimo del potenziale di errore grazie alla necessità di immettere le informazioni una sola volta e agli aggiornamenti automatici a livello di sistema.  
- Audit trail e visibilità completi per quanto riguarda le attività aziendali e lo storico delle transazioni.  
- Transazioni efficaci e convenienti con le consociate e le filiali.  

È possibile disporre di controllo completo su tutti i documenti delle transazioni. È ad esempio possibile rifiutare un documento inviato e, in questo modo, stornare le registrazioni e annullare carichi/spedizioni errati. Oppure, quando si effettua un acquisto da un partner o una filiale, è possibile aggiornare l'ordine di acquisto fino a quando la società venditrice non ha spedito le merci.  

Quando si immette una transazione, non è necessario specificare i conti per un singolo gruppo di registri, ma è sufficiente indicare l'identificativo della società partner. Tramite la funzionalità intercompany vengono create righe di registrazioni COGE che comportano il bilancio dei registri di entrambe le società coinvolte in una transazione. Nella contabilità clienti e fornitori è possibile assegnare un codice partner intercompany a qualsiasi cliente o fornitore. Da quel momento, tutte le fatture e gli ordini generati relativi a transazioni con tali società comporteranno la creazione di documenti corrispondenti nella società partner, consentendo un corretto bilancio dei conti.  

Dopo avere impostato nel sistema i partner aziendali come clienti e fornitori e avere assegnato loro codici partner intercompany, è possibile scambiare documenti di acquisto e di vendita intercompany, inclusi articoli e addebiti articoli. [!INCLUDE [prod_short](includes/prod_short.md)] supporta le transazioni intercompany tra più database, ad esempio in paesi/aree geografiche diversi, nonché tra più valute, piani dei conti diversi, dimensioni diverse e numerazioni articoli diverse.  

> [!NOTE]
> Non tutti i tipi di dati possono essere scambiati tra aziende in questo modo. Le fatture acquisto non vengono inviate ai business partner tramite processi intercompany. Tuttavia, le fatture di vendita inviate tramite processi interaziendali verranno create come fatture di acquisto nella società ricevente.

Il consolidamento dei dati finanziari può risultare utile con i processi Intercompany. Per ulteriori informazioni, vedere [Consolidare dati finanziari di molteplici società](finance-consolidated-company-reporting.md).

Nella tabella seguente viene descritta una sequenza di task, con collegamenti agli articoli che li descrivono.

|A |Vedere|
|---|---|
|Creare i fornitori e i clienti intercompany come partner intercompany e impostare un piano dei conti intercompany.|[Impostare la contabilità interaziendale](intercompany-how-setup.md)|
|Utilizzare documenti o registrazioni intercompany per registrare le transazioni con i partner Intercompany.|[Utilizzo di documenti e registrazioni intercompany](intercompany-how-work-documents-journals.md)|
|Organizzare ed elaborare le transazioni in entrata e in uscita che si scambiano con i partner IC.|[Gestire la casella in entrata e in uscita intercompany](intercompany-how-manage-intercompany-inbox.md)|
|Utilizzare le registrazioni IC per distribuire i costi tra società partner.|[Allocare costi a partner IC](intercompany-allocate-costs.md)|

## <a name="see-also"></a>Vedere anche

[Finanze](finance.md)  
[Impostazione di dati finanziari](finance-setup-finance.md)  
[Utilizzo delle registrazioni COGE](ui-work-general-journals.md)  
[Utilizzo di [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  


[!INCLUDE[footer-include](includes/footer-banner.md)]