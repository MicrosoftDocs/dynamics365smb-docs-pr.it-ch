---
title: Pagamenti elettronici svizzeri
description: I miglioramenti svizzeri consentono di inviare le fatture ai clienti elettronicamente. Le fatture vengono presentate e pagate direttamente utilizzando il software bancario online del cliente.
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: null
ms.date: 03/22/2022
ms.author: bholtorf
ms.service: dynamics-365-business-central
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

Per esportare i pagamenti secondo lo standard SEPA, è necessario utilizzare un conto bancario. Nei conti bancari, il campo **Categoria registrazione C/C bancario** deve specificare il conto di contabilità generale pertinente. In questo modo, i relativi movimenti di contabilità generale saranno coerenti con i movimenti generati per i metodi di pagamento svizzeri. Per ulteriori informazioni su come esportare i pagamenti SEPA, vedere [Creare movimenti riscossione addebiti diretti SEPA ed esportarli in un file della banca](../../finance-collect-payments-with-sepa-direct-debit.md#creating-sepa-direct-debit-collection-entries-and-export-to-a-bank-file).  

### <a name="iban-and-qr-iban"></a><a name="iban-qr"></a>IBAN e QR-IBAN

In Svizzera, le richieste di pagamento basate su bonifici SEPA possono includere un normale codice IBAN per il conto bancario o un codice QR-IBAN. Per ulteriori informazioni, vedi [Gestione fatture QR](ui-extensions-qr-bill-management.md).  

Il tipo di IBAN del conto bancario del destinatario deve corrispondere al tipo di riferimento di pagamento nel movimento quando tenti di pagare un fornitore. Se il riferimento di pagamento è un riferimento QR, [!INCLUDE [prod_short](../../includes/prod_short.md)] verificherà che l'IBAN sul conto bancario del fornitore sia un codice QR-IBAN. Se il riferimento di pagamento è un riferimento creditore, l'IBAN deve essere un normale IBAN.  

> [!TIP]
> Se un fornitore utilizza regolarmente entrambi i tipi di conto, crea più conti bancari del fornitore e utilizzali di conseguenza. Per ulteriori informazioni, vedi [Utilizzo di più conti bancari per emettere fatture QR](ui-extensions-qr-bill-management.md#multiplebankaccounts).

## <a name="see-also"></a>Vedere anche

[Gestione fatture QR nella versione svizzera](ui-extensions-qr-bill-management.md)  
[Importare numeri di clearing svizzeri](how-to-import-swiss-bank-clearing-numbers.md)  
[Pagamenti elettronici svizzeri tramite ESR](swiss-electronic-payments-using-esr.md)  
[Stampare fatture ESR](how-to-print-esr-invoices.md)  
[Pagamenti elettronici svizzeri tramite LSV+](swiss-electronic-payments-using-lsv-.md)  
[Funzionalità locale per la Svizzera](switzerland-local-functionality.md)  
[Effettuare i pagamenti](../../payables-make-payments.md)
[Creare movimenti riscossione addebiti diretti SEPA ed esportarli in un file della banca](../../finance-collect-payments-with-sepa-direct-debit.md#creating-sepa-direct-debit-collection-entries-and-export-to-a-bank-file)  

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
