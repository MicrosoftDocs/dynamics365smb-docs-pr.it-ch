---
title: 'Pagamenti elettronici svizzeri tramite LSV+ [CH]'
description: 'Il metodo di pagamento elettronico svizzero, ovvero Lastschrift Verfahren (LSV+) o addebito diretto consente alle aziende di recuperare i pagamenti direttamente dai conti correnti dei clienti.'
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: null
ms.search.form: '3010830, 3010831, 3010832,3010834, 3010835'
ms.date: 12/08/2023
ms.author: bholtorf
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---
# <a name="swiss-electronic-payments-using-lsv-in-the-swiss-version"></a>Pagamenti elettronici svizzeri tramite LSV+ nella versione per la Svizzera
Il metodo di pagamento elettronico svizzero, ovvero Lastschrift Verfahren (LSV+) o addebito diretto, versione migliorata del metodo LSV, consente alle aziende di recuperare i pagamenti direttamente dai conti correnti dei clienti. Per recuperare i pagamenti dei clienti, è necessario inviare un file LSV alla banca, che raccoglierà i pagamenti richiesti nel file.  

Il metodo LSV+ è un principio di addebito diretto con facoltà di opporsi. Il metodo BDD (Business Direct Debit) è invece un sistema di addebito diretto senza facoltà di opporsi. Il formato di file da inviare alla banca è lo stesso per i sistemi LSV+ e BDD.  

Prima di usare il modulo LSV, è necessario definire le impostazioni nella pagina **Setup LSV**.

## <a name="automatic-esr-processing"></a>Elaborazione ESR automatica
È possibile scaricare transazioni creditizie di pagamento nel formato di file ESR (polizza di versamento con numero di riferimento, in tedesco ESR, Einzahlungsschein mit Referenznummer) dalla banca. È possibile ricevere pagamenti LSV nel file ESR se il numero di riferimento ESR è integrato nel sistema LSV+. Se nei file LSV importati sono inclusi pagamenti LSV+, le righe di registrazione LSV correlate vengono chiuse automaticamente. L'elaborazione ESR automatica viene eseguita solo per i pagamenti che utilizzano franchi svizzeri (CHF) e richiede che vengano effettuate queste operazioni:  

- Dopo aver inviato il file LSV+ alla banca, inviare un report di pagamenti entro tre giorni lavorativi dalla data di elaborazione LSV richiesta.  

- Importare i file ESR, quindi inserire le registrazioni ESR. Se una transazione ESR importata è correlata alla riga di pagamento LSV+, la riga di registrazione LSV appropriata viene chiusa automaticamente da ESR.  

    > [!NOTE]  
    >  Quando si importa un file ESR, la riga di registrazione LSV viene chiusa da ESR se viene trovata la registrazione LSV appropriata, indipendentemente dal tipo di transazione ESR.  

- Dopo la data di elaborazione LSV, è possibile controllare le righe di registrazione LSV. Se tutte le righe di registrazione LSV sono chiuse, lo stato del campo **Stato LSV** viene aggiornato sul valore **Completato**.  

## <a name="see-also"></a>Vedere anche
 [Elaborare una riscossione LSV](how-to-process-an-lsv-collection.md)   
 [Chiudere una riscossione LSV](how-to-close-an-lsv-collection.md)   
 [Registrare pagamenti LSV+](how-to-post-lsv-payments.md)   
 [Esportare pagamenti tramite LSV](how-to-export-payments-using-lsv.md)   
 [Pagamenti elettronici svizzeri](swiss-electronic-payments.md)   
 [Pagamenti elettronici svizzeri tramite ESR](swiss-electronic-payments-using-esr.md)   
 [Effettuare i pagamenti](../../payables-make-payments.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
