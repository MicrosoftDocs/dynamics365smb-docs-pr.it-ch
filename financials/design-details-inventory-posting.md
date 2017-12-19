---
title: 'Dettagli di progettazione: Registrazione di magazzino | Microsoft Docs'
description: Ogni transazione di magazzino, ad esempio un carico di acquisto o una spedizione di vendita, registra due movimenti dei tipi diversi.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 9bc177d45efa1e6e772ed70cc66de393e6250def
ms.contentlocale: it-ch
ms.lasthandoff: 09/22/2017

---
# <a name="design-details-inventory-posting"></a>Dettagli di progettazione: Registrazione di magazzino
Ogni transazione di magazzino, ad esempio un carico di acquisto o una spedizione di vendita, registra due movimenti dei tipi diversi.  

|Tipo movimento|Description|  
|----------------|---------------------------------------|  
|Quantità|Riflette la modifica della quantità a magazzino. Queste informazioni vengono archiviate nei movimenti contabili articoli.<br /><br /> Accompagnato da movimenti di collegamento articolo.|  
|Valore|Riflette la modifica del valore di magazzino. Queste informazioni vengono archiviate nei movimenti di valorizzazione.<br /><br /> È possibile associare a ciascun movimento contabile articolo o a ciascun movimento contabile capacità uno o più movimenti valorizzazione.<br /><br /> Per informazioni sui movimenti di valorizzazione di capacità correlati all'utilizzo delle risorse di assemblaggio o di produzione, vedere [Dettagli di progettazione: Registrazione dell'ordine di produzione](design-details-production-order-posting.md).|  

 In relazione alle registrazioni della quantità, i movimenti di collegamento articoli sono disponibili per collegare l'aumento di magazzino con una riduzione di magazzino. Ciò consente al motore di costing di inoltrare i costi dagli aumenti alle diminuzioni correlate e viceversa. Per ulteriori informazioni, vedere [Dettagli di progettazione: Collegamento articoli](design-details-item-application.md).  

 I movimenti contabili articoli, i movimenti di valorizzazione e i movimenti di collegamento articoli vengono creati come risultato della registrazione di una riga di registrazioni magazzino, indirettamente tramite la registrazione di una riga ordine o direttamente nella finestra Registrazioni magazzino.  

 A intervalli regolari, i movimenti di valorizzazione creati nei movimenti di magazzino vengono registrati nella contabilità generale per riconciliare i due registri per i motivi di controllo finanziario. Per ulteriori informazioni, vedere [Dettagli di progettazione: Riconciliazione con la contabilità generale](design-details-reconciliation-with-the-general-ledger.md).  

 ![Flusso di movimento tra l'inventario e C/G](media/design_details_inventory_costing_1_entry_flow.png "design_details_inventory_costing_1_entry_flow")  

## <a name="example"></a>Esempio  
 Nell'esempio seguente viene illustrato come i movimenti contabili articoli, i movimenti di valorizzazione e i movimenti di collegamento articoli risultano nei movimenti di contabilità generale.  

 È possibile registrare un ordine di acquisto come ricevuto e fatturato per 10 articoli con un costo unitario diretto di VL 7 e un coefficiente costi generali di VL 1. La data di registrazione è 01-01-20. Vengono creati i seguenti movimenti.  

 **Mov. contabili articoli**  

|Data di registrazione:|Tipo movimento|Importo costo (effettivo)|Quantità|Nr. movimento|  
|------------------|----------------|----------------------------|--------------|---------------|  
|01-01-20|Acquisti|80,00|10|1|  

 **Movimenti di valorizzazione**  

|Data di registrazione:|Tipo movimento|Importo costo (effettivo)|Nr. movimento cont. articolo|Nr. movimento|  
|------------------|----------------|----------------------------|---------------------------|---------------|  
|01-01-20|Costo Diretto|70.00|1|1|  
|01-01-20|Costo Indiretto|10,00|1|2|  

 **Movimenti di collegamento articoli**  

|Nr. movimento|Nr. movimento cont. articolo|Nr. movimento articolo in entrata|Nr. movimento articolo in uscita|Quantità|  
|---------------|---------------------------|----------------------------|-----------------------------|--------------|  
|1|1|1|0|10|  

 Successivamente, registrare una vendita di 10 unità dell'articolo con una data di registrazione di 01-15-20.  

 **Mov. contabili articoli**  

|Data di registrazione:|Tipo movimento|Importo costo (effettivo)||Quantità|Nr. movimento|  
|------------------|----------------|----------------------------|-|--------------|---------------|  
|01-15-20|Vendite|-80,00||-10|2|  

 **Movimenti di valorizzazione**  

|Data di registrazione:|Tipo movimento|Importo costo (effettivo)|Nr. movimento cont. articolo|Nr. movimento|  
|------------------|----------------|----------------------------|---------------------------|---------------|  
|01-15-20|Costo Diretto|-80,00|2|3|  

 **Movimenti di collegamento articoli**  

|Nr. movimento|Nr. movimento cont. articolo|Nr. movimento articolo in entrata|Nr. movimento articolo in uscita|Quantità|  
|---------------|---------------------------|----------------------------|-----------------------------|--------------|  
|2|2|1|2|-10|  

 Alla fine del periodo contabile, viene eseguito il processo batch **Registra costo magazzino in CG** per riconciliare le transazioni di magazzino con la contabilità generale.  

 Per ulteriori informazioni, vedere [Dettagli di progettazione: Conti nella contabilità generale](design-details-accounts-in-the-general-ledger.md).  

 Nelle seguenti tabelle viene mostrano il risultato della riconciliazione delle transazioni di magazzino in questo esempio con la contabilità generale.  

 **Movimenti di valorizzazione**  

|Data di registrazione:|Tipo movimento|Importo costo (effettivo)|Costo registrato in C/G|Nr. movimento cont. articolo|Nr. movimento|  
|------------------|----------------|----------------------------|-------------------------|---------------------------|---------------|  
|01-01-20|Costo Diretto|70.00|70.00|1|1|  
|01-01-20|Costo Indiretto|10,00|10,00|1|2|  
|01-15-20|Costo Diretto|-80,00|-80,00|2|3|  

 **Movimenti C/G**  

|Data di registrazione:|Conti C/G|Numero di conto (demo en-US)||Importo|Nr. movimento|  
|------------------|------------------|---------------------------------|-|------------|---------------|  
|01-01-20|[Conto giac. magazzino]|2130||70.00|1|  
|01-01-20|[Conto costi diretti coll.]|7291||-70,00|2|  
|01-01-20|[Conto giac. magazzino]|2130||10,00|3|  
|01/01/07|[Conto costi generali coll.]|7292||-10,00|4|  
|01-15-20|[Conto giac. magazzino]|2130||-80,00|5|  
|01-15-20|[Conto COGS]|7290||80,00|6|  

> [!NOTE]  
>  La data di registrazione dei movimenti di contabilità generale è la stessa dei movimenti di valorizzazione correlati.  
>   
>  Il campo **Costo registrato in C/G** nella tabella **Movimenti valorizzazione** viene compilato.  

 La relazione tra i movimenti di valorizzazione e i movimenti di contabilità generale viene archiviata nella tabella **Relazione C/G - Mov. contabili art.**.  

 **Movimenti di relazione nella C/G – Relazione Movimento Articolo**  

|Nr. movimento C/G|Nr. movimento valorizzazione|Nr. registro C/G|  
|--------------------|---------------------|-----------------------|  
|1|1|1|  
|2|1|1|  
|3|2|1|  
|4|2|1|  
|5|3|1|  
|6|3|1|  

## <a name="assembly-and-production-posting"></a>Registrazione assemblaggio e produzione  
I movimenti contabili risorse e capacità rappresentano il tempo registrato come consumato nella produzione o nell'assemblaggio. Questi costi di processo vengono registrati come movimenti di valorizzazione nella contabilità generale insieme ai costi di materiale interessati in una struttura simile a quella descritta per i movimenti contabili articoli in questo argomento.  

Per ulteriori informazioni, vedere [Dettagli di progettazione: Metodi di costing](design-details-assembly-order-posting.md).  

## <a name="see-also"></a>Vedi anche  
 [Dettagli di progettazione: Costing di magazzino](design-details-inventory-costing.md)   
 [Dettagli di progettazione: Conti nella contabilità generale](design-details-accounts-in-the-general-ledger.md)   
 [Dettagli di progettazione: Componenti costo](design-details-cost-components.md) [Gestione dei costi di magazzino](finance-manage-inventory-costs.md)  
 [Finanze](finance.md)  
 [Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
