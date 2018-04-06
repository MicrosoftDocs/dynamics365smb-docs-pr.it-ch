---
title: Pagamenti elettronici svizzeri tramite LSV+
description: "Il metodo di pagamento elettronico svizzero, ovvero Lastschrift Verfahren (LSV+) o addebito diretto, versione migliorata del metodo LSV, consente alle aziende di recuperare i pagamenti direttamente dai conti correnti dei clienti. Per recuperare i pagamenti dei clienti, è necessario inviare un file LSV alla banca, che raccoglierà i pagamenti richiesti nel file."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 03/06/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 6dd44e11baa7a834081e215f21a53db089f47c4b
ms.contentlocale: it-ch
ms.lasthandoff: 03/22/2018

---
# <a name="swiss-electronic-payments-using-lsv"></a>Pagamenti elettronici svizzeri tramite LSV+
Il metodo di pagamento elettronico svizzero, ovvero Lastschrift Verfahren (LSV+) o addebito diretto, versione migliorata del metodo LSV, consente alle aziende di recuperare i pagamenti direttamente dai conti correnti dei clienti. Per recuperare i pagamenti dei clienti, è necessario inviare un file LSV alla banca, che raccoglierà i pagamenti richiesti nel file.  

Il metodo LSV+ è un principio di addebito diretto con facoltà di opporsi. Il metodo BDD (Business Direct Debit) è invece un sistema di addebito diretto senza facoltà di opporsi. Il formato di file da inviare alla banca è lo stesso per i sistemi LSV+ e BDD.  

Prima di usare il modulo LSV, è necessario definire le impostazioni nella finestra **Setup LSV**.

## <a name="automatic-esr-processing"></a>Elaborazione ESR automatica  
È possibile scaricare transazioni creditizie di pagamento nel formato di file ESR (polizza di versamento con numero di riferimento, in tedesco ESR, Einzahlungsschein mit Referenznummer) dalla banca. È possibile ricevere pagamenti LSV nel file ESR se il numero di riferimento ESR è integrato nel sistema LSV+. Se nei file LSV importati sono inclusi pagamenti LSV+, le righe di registrazione LSV correlate vengono chiuse automaticamente. L'elaborazione ESR automatica viene eseguita solo per i pagamenti che utilizzano franchi svizzeri (CHF) e richiede che vengano effettuate queste operazioni:  

- Dopo aver inviato il file LSV+ alla banca, inviare un report di pagamenti entro tre giorni lavorativi dalla data di elaborazione LSV richiesta.  

- Importare i file ESR, quindi inserire le registrazioni ESR. Se una transazione ESR importata è correlata alla riga di pagamento LSV+, la riga di registrazione LSV appropriata viene chiusa automaticamente da ESR.  

    > [!NOTE]  
    >  Quando si importa un file ESR, la riga di registrazione LSV viene chiusa da ESR se viene trovata la registrazione LSV appropriata, indipendentemente dal tipo di transazione ESR.  

- Dopo la data di elaborazione LSV, è possibile controllare le righe di registrazione LSV. Se tutte le righe di registrazione LSV sono chiuse, lo stato del campo **Stato LSV** viene aggiornato sul valore **Completato**.  

## <a name="see-also"></a>Vedi anche  
 [Elaborare una riscossione LSV](how-to-process-an-lsv-collection.md)   
 [Chiudere una riscossione LSV](how-to-close-an-lsv-collection.md)   
 [Registrare pagamenti LSV+](how-to-post-lsv-payments.md)   
 [Esportare pagamenti tramite LSV](how-to-export-payments-using-lsv.md)   
 [Pagamenti elettronici svizzeri](swiss-electronic-payments.md)   
 [Pagamenti elettronici svizzeri tramite ESR](swiss-electronic-payments-using-esr.md)   
 [Effettuare i pagamenti](../../payables-make-payments.md)

