---
title: Pagamenti elettronici svizzeri
description: I miglioramenti svizzeri consentono di inviare le fatture ai clienti elettronicamente. Le fatture vengono presentate e pagate direttamente utilizzando il software bancario online del cliente.
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 570804934f0cd4fae17a797f383048d95b0b5ae5
ms.sourcegitcommit: ef80c461713fff1a75998766e7a4ed3a7c6121d0
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 02/15/2022
ms.locfileid: "8134438"
---
# <a name="swiss-electronic-payments"></a>Pagamenti elettronici svizzeri
[!INCLUDE[prod_short](../../includes/prod_short.md)] consente di inviare le fatture ai clienti elettronicamente. Le fatture vengono presentate e pagate direttamente utilizzando il software bancario online del cliente.  

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
Per esportare i pagamenti secondo lo standard SEPA, è necessario utilizzare un conto bancario. Per assicurarsi che i movimenti contabili corrispondenti siano coerenti con quelli generati per i metodi di pagamento svizzeri locali (vedere sopra), il valore nel campo **Cat. reg. C/C bancario** della pagina **Scheda conto corrente bancario** deve indicare il relativo conto C/G. Per ulteriori informazioni su come esportare i pagamenti SEPA, vedere [Creare movimenti riscossione addebiti diretti SEPA ed esportarli in un file della banca](../../finance-collect-payments-with-sepa-direct-debit.md#creating-sepa-direct-debit-collection-entries-and-export-to-a-bank-file).  

## <a name="see-also"></a>Vedi anche  
 [Importare numeri di clearing svizzeri](how-to-import-swiss-bank-clearing-numbers.md)  
 [Pagamenti elettronici svizzeri tramite ESR](swiss-electronic-payments-using-esr.md)  
 [Stampare fatture ESR](how-to-print-esr-invoices.md)  
 [Pagamenti elettronici svizzeri tramite LSV+](swiss-electronic-payments-using-lsv-.md)  
 [Funzionalità locale per la Svizzera](switzerland-local-functionality.md)  
 [Effettuare i pagamenti](../../payables-make-payments.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]