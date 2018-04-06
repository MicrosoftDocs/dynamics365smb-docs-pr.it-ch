---
title: Pagamenti elettronici svizzeri
description: I miglioramenti svizzeri consentono di inviare le fatture ai clienti elettronicamente. Le fatture vengono presentate e pagate direttamente utilizzando il software bancario online del cliente.
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
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 5cbcf1172d29ccbfebd1045c0eb7798f1aef2f24
ms.contentlocale: it-ch
ms.lasthandoff: 03/22/2018

---
# <a name="swiss-electronic-payments"></a>Pagamenti elettronici svizzeri
[!INCLUDE[d365fin](../../includes/d365fin_md.md)] consente di inviare le fatture ai clienti elettronicamente. Le fatture vengono presentate e pagate direttamente utilizzando il software bancario online del cliente.  

## <a name="electronic-payment-methods"></a>Metodi di pagamento elettronico  
È possibile effettuare pagamenti elettronici utilizzando i seguenti metodi:  

- Einzahlungsschein mit Referenznummer (ESR)  
- Lastschrift Verfahren (LSV+)  
- Bonifici SEPA  

## <a name="esr"></a>ESR  
ESR è un servizio debitore elettronico che utilizza distinte di pagamento per riscuotere fondi. È il sistema di pagamento elettronico standard creato da Swiss Post. È possibile stampare le distinte di pagamento ESR come allegati a fattura, calcolare i numeri di riferimento ESR e importare file ESR che hanno informazioni di pagamento delle banche. Per ulteriori informazioni, vedere [Pagamenti elettronici svizzeri tramite ESR](how-to-print-esr-invoices.md). Inoltre, è possibile effettuare pagamenti ESR e ESR+ utilizzando la versione della banca di questo metodo di pagamento denominato Bank-ESR (BESR).  

## <a name="lsv"></a>LSV+  
LSV+ è un servizio di addebito diretto che viene utilizzato per l'elaborazione dei pagamenti. Le aziende possono rilasciare i pagamenti dei clienti direttamente dalla banca del cliente utilizzando l'addebito diretto. È possibile richiedere e riscuotere i pagamenti dei clienti utilizzando l'addebito diretto nel formato bancario LSV+ o nel formato DebitDirect PostFinance. Per ulteriori informazioni, vedere [Pagamenti elettronici svizzeri tramite LSV+](swiss-electronic-payments-using-lsv-.md).  

## <a name="sepa-credit-transfers"></a>Bonifici SEPA  
Per esportare i pagamenti secondo lo standard SEPA, è necessario utilizzare un conto bancario. Per assicurarsi che i movimenti contabili corrispondenti siano coerenti con quelli generati per i metodi di pagamento svizzeri locali (vedere sopra), il valore nel campo **Cat. reg. C/C bancario** della finestra **Scheda conto corrente bancario** deve indicare il relativo conto C/G. Per ulteriori informazioni su come esportare i pagamenti SEPA, vedere [Creare movimenti riscossione addebiti diretti SEPA ed esportarli in un file della banca](../../finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md).  

## <a name="see-also"></a>Vedi anche  
 [Importare numeri di clearing svizzeri](how-to-import-swiss-bank-clearing-numbers.md)   
 [Pagamenti elettronici svizzeri tramite ESR](swiss-electronic-payments-using-esr.md)   
 [Stampare fatture ESR](how-to-print-esr-invoices.md)   
 [Pagamenti elettronici svizzeri tramite LSV+](swiss-electronic-payments-using-lsv-.md)   
 [Funzionalità locale per la Svizzera](switzerland-local-functionality.md)  ' [Creare movimenti riscossione addebiti diretti SEPA ed esportarli in un file della banca](../../finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md)  
 [Effettuare i pagamenti](../../payables-make-payments.md)

