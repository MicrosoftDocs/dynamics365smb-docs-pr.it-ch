---
title: 'Pagamenti elettronici svizzeri tramite ESR [CH]'
description: Questo argomento spiega le diverse attività che è possibile eseguire con il servizio debitore del metodo di pagamento elettronico Einzahlungsschein mit Referenznummer (ESR).
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: null
ms.search.form: '3010531, 3010532'
ms.date: 06/21/2021
ms.author: bholtorf
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---
# Pagamenti elettronici svizzeri tramite ESR nella versione per la Svizzera
Il metodo di pagamento elettronico ESR (polizza di versamento con numero di riferimento, in tedesco ESR, Einzahlungsschein mit Referenznummer) è un servizio debitori elettronico che consente al cliente di fatturare fatture aperte in franchi svizzeri (CHF) ed euro (EUR) e di registrare pagamenti in entrata in modo efficiente. Il numero di riferimento, o riga di codice, contiene tutti i dati contabili rilevanti.  

Con i pagamenti elettronici ESR è possibile effettuare le seguenti operazioni:  

- Inviare distinte di pagamento ESR con numeri di riferimento univoci sulle fatture. Poiché i numeri di riferimento ESR sono univoci, i pagamenti per la liquidazione vengono applicati automaticamente alle fatture correlate. Per ulteriori informazioni, vedere [Stampare fatture ESR](how-to-print-esr-invoices.md).  

- Scaricare giornalmente i file ESR dalla banca. I file contengono informazioni su tutte le fatture pagate.  

- Importare i file ESR e creare righe di pagamento in modo automatico per ogni pagamento. Per ulteriori informazioni, vedere [Importare pagamenti ESR](how-to-import-esr-payments.md).  

> [!NOTE]  
>  Prima di usare il modulo ESR, è necessario impostare la banca, il conto corrente bancario e il nome del file. È inoltre necessario specificare se deve essere usato il metodo ESR o ESR+.

Dopo aver valutato le informazioni di setup, è possibile modificare il modulo di fatturazione e creare una serie di test che la banca o il servizio postale può convalidare.  

Quando si impostano le numerazioni per le fatture, è necessario seguire queste linee guida:  

- Usa un massimo di otto cifre.  
- Usare solo caratteri numerici.  
- Non anteporre zero ai numeri.  

## Vedi anche  
 [Pagamenti elettronici svizzeri](swiss-electronic-payments.md)   
 [Stampare fatture ESR](how-to-print-esr-invoices.md)   
 [Importare i pagamenti ESR](how-to-import-esr-payments.md)   
 [Pagamenti elettronici svizzeri tramite LSV+](swiss-electronic-payments-using-lsv-.md)   
 [Effettuare i pagamenti](../../payables-make-payments.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]