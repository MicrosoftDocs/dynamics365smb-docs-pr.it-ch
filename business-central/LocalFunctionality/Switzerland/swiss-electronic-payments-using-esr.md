---
title: Pagamenti elettronici svizzeri tramite ESR
description: "Il metodo di pagamento elettronico ESR (polizza di versamento con numero di riferimento, in tedesco ESR, Einzahlungsschein mit Referenznummer) è un servizio debitori elettronico che consente al cliente di fatturare fatture aperte in franchi svizzeri (CHF) ed euro (EUR) e di registrare pagamenti in entrata in modo efficiente."
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
ms.openlocfilehash: dbd03106bca19c2b6d19fc92d36b839ea856acd1
ms.contentlocale: it-ch
ms.lasthandoff: 03/22/2018

---
# <a name="swiss-electronic-payments-using-esr"></a>Pagamenti elettronici svizzeri tramite ESR
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

## <a name="see-also"></a>Vedi anche  
 [Pagamenti elettronici svizzeri](swiss-electronic-payments.md)   
 [Stampare fatture ESR](how-to-print-esr-invoices.md)   
 [Importare i pagamenti ESR](how-to-import-esr-payments.md)   
 [Pagamenti elettronici svizzeri tramite LSV+](swiss-electronic-payments-using-lsv-.md)   
 [Effettuare i pagamenti](../../payables-make-payments.md)

