---
title: Documenti di acquisto e di vendita per la Svizzera
description: I miglioramenti svizzeri includono funzioni speciali di documento di vendita e di acquisto.
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
ms.openlocfilehash: 4b2879f3b913ddc554cbbbe49fedd3bc1434b0ad
ms.contentlocale: it-ch
ms.lasthandoff: 03/22/2018

---
# <a name="swiss-purchase-documents-and-sales-documents"></a>Documenti di acquisto e di vendita per la Svizzera
[!INCLUDE[d365fin](../../includes/d365fin_md.md)] include miglioramenti svizzeri per documenti di vendita e documenti di acquisto. È incluso quanto segue:  

- Descrizioni di registrazione avanzata per i movimenti di contabilità generale, i movimenti contabili clienti e i movimenti contabili fornitori. Per ulteriori informazioni, vedere la tabella Movimenti C/G, Mov. contabili clienti e Mov. contabili fornitori.  
- La capacità di avere sottotitoli, subtotali e totali iniziali e finali nelle offerte di vendita e negli ordini di vendita.  
- La capacità di arrotondare i totali delle fatture nelle righe di registrazione pagamenti se è disponibile uno sconto di pagamento.  
- La possibilità di disattivare la stampa di documenti di spedizione aggiuntivi per fatture di acquisto e le fatture di vendita.  

## <a name="purchase-documents-and-sales-documents"></a>Documenti di acquisto e di vendita  
Le descrizioni di registrazione contabilizzate nei movimenti contabili per ordini di acquisto e ordini di vendita indicano il nome dei fornitori o dei clienti e i numeri delle fatture o delle note di credito. Ad esempio, **Fatt. 103020/ Cannon Group SpA** è una descrizione di registrazione. Questa descrizione di registrazione mostra un numero rilevante per le transazioni finanziarie, che consente di analizzare le transazioni più facilmente.  

### <a name="sales-quotes-and-sales-orders"></a>Offerte di vendita e ordini di vendita  
Quando viene creata una offerta di vendita o un ordine di vendita, se il tipo della riga dell'offerta o dell'ordine di vendita è **Totale iniziale** o **Totale finale**, gli articoli elencati nelle righe sono contrassegnati come articoli fisici o come articoli in assistenza. Gli articoli hanno quindi sottotitoli per ogni gruppo di articoli e viene creato un subtotale per ogni gruppo di articoli.  

Gli articoli vengono suddivisi in base ai valori generati dal sistema visualizzati nel campo **Livello**.  

Specificare un articolo come variante nella riga dell'offerta di vendita. In tal modo è possibile elencare gli articoli alternativi senza includere il prezzo nell'offerta. Inoltre è possibile fare riferimento a parti specifiche di una offerta di vendita o di un ordine di vendita in base al valore visualizzato nel campo **Posizione** della riga dell'offerta di vendita o dell'ordine di vendita. Per ulteriori informazioni, vedere la tabella Righe vendite.  

## <a name="purchase-invoices-and-sales-invoices-with-payment-discounts"></a>Fatture di acquisto e fatture di vendita con sconti di pagamento  
Per le fatture di acquisto e le fatture di vendita, l'importo della fattura viene ridotto per l'importo dello sconto e quindi arrotondato. Anche il totale della fattura viene arrotondato se c'è uno sconto. Per ulteriori informazioni, vedere la tabella Setup contabilità generale.  

## <a name="shipment-documents"></a>Documenti di spedizione  
Nella finestra **Setup contabilità clienti e vendite**, il campo **Spedizione e fattura** viene utilizzato per disattivare la stampa di documenti di spedizione aggiuntivi per fatture di acquisto e le fatture di vendita. Quando si registra un ordine, vengono automaticamente create una spedizione registrata e una fattura registrata. Se la fattura stampata viene anche utilizzata come documento di spedizione, non è necessario stampare la documentazione di spedizione aggiuntiva. È possibile disattivare la stampa dei documenti di spedizione aggiuntivi per le fatture di acquisto e le fatture di vendita deselezionando il campo **Spedizione e fattura** nella finestra **Setup contabilità clienti**. Per ulteriori informazioni, vedere la tabella Setup contabilità clienti.  

## <a name="see-also"></a>Vedi anche  
 [Importare codici postali svizzeri](how-to-import-swiss-post-codes.md)   
 [Stampare una lista prelievi magazzino da un ordine di vendita](how-to-print-an-inventory-picking-list-from-a-sales-order.md)   
 [Stampare ordini di vendita e acquisto durante la registrazione batch](how-to-print-sales-and-purchase-orders-during-batch-posting.md)   
 [Funzionalità locale per la Svizzera](switzerland-local-functionality.md)

