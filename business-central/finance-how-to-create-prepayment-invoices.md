---
title: Come creare fatture di pagamenti anticipati | Microsoft Docs
description: Informazioni su come gestire situazioni in cui un pagamento anticipato viene richiesto ai clienti o dal fornitore.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 72a073fcde9ddf20df7c138ab544afb6719b93ce
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 03/31/2021
ms.locfileid: "5782181"
---
# <a name="create-prepayment-invoices"></a>Creare fatture per i pagamenti anticipati

Se è necessario che i clienti inviino il pagamento prima della spedizione di un ordine, è possibile utilizzare la funzionalità di pagamento anticipato. Lo stesso vale se il fornitore richiede di inviare il pagamento prima di spedire un ordine.  

È possibile creare un processo di pagamento anticipato quando si crea un ordine di vendita o di acquisto. Se è impostata una percentuale di pagamento anticipato predefinita per il cliente o il fornitore, verrà automaticamente inclusa nella fattura di pagamento anticipato risultante. È inoltre possibile specificare una percentuale di pagamento anticipato per l'intero documento.

Dopo avere creato un ordine di vendita o di acquisto, è possibile creare una fattura pagamento anticipato. È possibile utilizzare le percentuali di default per ogni riga di vendita o di acquisto oppure rettificare l'importo come necessario. È ad esempio possibile specificare un importo totale per l'intero ordine.  

La procedura seguente descrive come fatturare un pagamento anticipato per un ordine di vendita. I passaggi sono simili per un ordine di acquisto.  

## <a name="to-create-a-prepayment-invoice"></a>Per creare una fattura di pagamento anticipato

1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Ordini vendita** e quindi scegliere il collegamento correlato.  
2. Creare un nuovo ordine di vendita per un cliente pertinente. Per ulteriori informazioni, vedere [Vendere prodotti](sales-how-sell-products.md).  

    Nella scheda dettaglio **Pagamento anticipato** il campo **% pagamento anticipato** specifica la percentuale da utilizzare per calcolare l'importo del pagamento anticipato. Se nella scheda cliente è impostata una percentuale pagamento anticipato di default, il campo viene compilato automaticamente. È possibile modificare la percentuale. <!--This percentage is applied to lines where the item on that line does not already specify a prepayment percentage. The prepayment percentage is only copied from the header to lines that do not copy the default prepayment percentage from the item.-->  

    Scegliere il campo **Comprimi pagamento anticipato** se si desidera creare righe nella fattura di pagamento anticipato che combinano righe dell'ordine cliente se:  

    - Le righe hanno lo stesso conto di contabilità generale per i pagamenti anticipati, come determinato in Setup registrazioni COGE.  
    - Le righe hanno le stesse dimensioni.  

    Se si desidera specificare una fattura pagamento anticipato con una riga per ogni riga dell'ordine di vendita associata a una percentuale pagamento anticipato, non scegliere il campo **Comprimi pagamento anticipato**.  

    La data di scadenza per il pagamento anticipato viene calcolata automaticamente in base al valore di **Cod. condizioni pagam. ant.**.

3. Compilare le righe di vendita.  

    Se è stata specificata una percentuale di pagamento anticipato predefinita per il cliente o nella scheda dettaglio **Pagamento anticipato** sul documento, questo valore viene copiato in ogni riga. È possibile modificare il contenuto del campo **% pagamento anticipato** nella riga.  

4. Per visualizzare l'importo del pagamento anticipato totale, scegliere l'azione **Statistiche**.

    Se si desidera rettificare l'importo del pagamento anticipato totale per l'ordine, è possibile modificare il contenuto del campo **Importo pagamento anticipato** nella pagina **Statistiche ordini vendita**.  

    Se il campo **Prezzi IVA inclusa** è selezionato, il campo **Importo pagam. ant. IVA incl.** è modificabile.  

    Se si modifica il contenuto del campo **Importo pagamento anticipato**, l'importo verrà distribuito proporzionalmente tra tutte le righe, ad eccezione di quelle in cui è presente il valore **0** nel campo **% pagamento anticipato**.  

5. Per stampare un report test prima di registrare una fattura pagamento anticipato, scegliere l'azione **Pagamento anticipato** e quindi scegliere l'azione **Report test pagamento anticipato**.  
6. Per registrare la fattura pagamento anticipato, scegliere l'azione **Pagamento anticipato** e quindi scegliere l'azione **Registra fattura pagamento anticipato**.  

    Per registrare e stampare la fattura pagamento anticipato, scegliere l'azione **Registra e stampa fattura pagam. ant.**  

È possibile emettere fatture pagamento anticipato aggiuntive per l'ordine. A tale scopo, aumentare l'importo pagamento anticipato in una o più righe, rettificare la data del documento, se necessario, e registrare la fattura pagamento anticipato. Verrà creata una nuova fattura per la differenza tra gli importi pagamento anticipato fatturati fino a quel momento e il nuovo importo pagamento anticipato.  

> [!NOTE]  
> Se ci si trova in America del Nord, non è possibile modificare la percentuale di pagamento anticipato dopo che la fattura pagamento anticipato è stata registrata. Ciò è impedito nella versione nordamericana di [!INCLUDE[prod_short](includes/prod_short.md)] perché altrimenti il calcolo dell'imposta sulle vendite risulterebbe errato.  

 Quando si è pronti per registrare il resto della fattura, effettuare la registrazione come con qualsiasi fattura. L'importo pagamento anticipato verrà automaticamente dedotto dall'importo dovuto.  

## <a name="see-also"></a>Vedi anche

[Fatturazione dei pagamenti anticipati](finance-invoice-prepayments.md)  
[Procedura dettagliata: impostazione e fatturazione dei pagamenti anticipati vendite](walkthrough-setting-up-and-invoicing-sales-prepayments.md)  
[Finanze](finance.md)  
[Utilizzo di [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]