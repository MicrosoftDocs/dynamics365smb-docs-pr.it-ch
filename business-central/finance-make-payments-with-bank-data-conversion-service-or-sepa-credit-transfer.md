---
title: Eseguire i pagamenti con il servizio di conversione dati bancari o bonifico SEPA | Microsoft Docs
description: Elaborare i pagamenti ai fornitori esportando un file con le informazioni di pagamento dalle righe registrazioni.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 99277cb2daf37fbce4548cf637e8967fa6688dbc
ms.contentlocale: it-ch
ms.lasthandoff: 03/22/2018

---
# <a name="making-payments-with-bank-data-conversion-service-or-sepa-credit-transfer"></a>Effettuare i pagamenti con servizio di conversione dati bancari o bonifico SEPA
Nella finestra **Registraz. pagamenti** è possibile elaborare i pagamenti ai fornitori esportando un file con le informazioni di pagamento dalle righe registrazioni. È quindi possibile caricare il file sul sito elettronico della banca dove vengono elaborati i trasferimenti di denaro correlati. [!INCLUDE[d365fin](includes/d365fin_md.md)] supporta il formato di bonifico SEPA, ma nel proprio paese potrebbero essere disponibili anche altri formati di pagamento elettronico.   

 Per abilitare i bonifici SEPA, è necessario innanzitutto impostare un conto corrente bancario, un fornitore e il batch registrazioni COGE su cui si basano le registrazioni pagamenti. Successivamente si preparano i pagamenti dei fornitori compilando automaticamente la finestra **Registraz. pagamenti** con i pagamenti in scadenza insieme alle date di registrazione specificate.  

> [!NOTE]  
>  Una volta verificato che i pagamenti sono stati elaborati correttamente dalla banca, è possibile passare alla registrazione delle righe di registrazione pagamenti.  

 Nella tabella seguente viene descritta una sequenza di task, con collegamenti agli argomenti che li descrivono.   

|**Per**|**Vedere**|  
|------------|-------------|  
|Attivare la funzionalità In modo inverso, è possibile utilizzare la funzionalità Servizio di conversione di dati bancari per convertire tutti i file di rendiconto bancario in un formato che è possibile importare o per convertire i file di pagamento esportati nel formato richiesto dalla banca.|[Impostare il servizio di conversione di dati bancari](bank-how-setup-bank-statement-service.md)|  
|Impostare un conto corrente bancario, un fornitore e le registrazioni pagamenti per bonifici SEPA.|[Impostare un bonifico SEPA](finance-how-to-set-up-sepa-credit-transfer.md)|  
|Compilare le registrazioni di pagamento con le righe per i pagamenti dovuti ai fornitori, con l'opzione di inserire le date di registrazione in base alla data di scadenza dei reltivi documenti di acquisto.|[Gestione della contabilità fornitori](payables-manage-payables.md)|  
|Esportare le righe registrazione pagamenti in un file in formato di bonifico SEPA.|[Esportare pagamenti in un file della banca](payables-how-export-payments-bank-file.md)|  
|Quando il pagamento elettronico viene elaborato correttamente dalla banca, registrare i pagamenti.|[Utilizzo delle registrazioni COGE](ui-work-general-journals.md)|  

## <a name="see-also"></a>Vedi anche  
[Impostare il servizio di conversione di dati bancari](bank-how-setup-bank-statement-service.md)  
[Impostare un bonifico SEPA](finance-how-to-set-up-sepa-credit-transfer.md)  
[Gestione della contabilità fornitori](payables-manage-payables.md)   
[Utilizzo delle registrazioni COGE](ui-work-general-journals.md)  
[Riscuotere pagamenti con addebito diretto SEPA](finance-collect-payments-with-sepa-direct-debit.md)   
