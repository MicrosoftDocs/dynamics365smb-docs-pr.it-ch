---
title: Come rettificare i tassi di cambio
description: Se è presente una vendita imponibile in una valuta estera, è necessario usare il tasso ufficiale per la conversione di valuta IVA, come definito dall'ente Federal Tax Administration.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: 3662736f462e488d1ac2c42e2195accf4352dcff
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 03/31/2019
ms.locfileid: "937915"
---
# <a name="adjust-exchange-rates"></a>Rettifica tassi di cambio
Se è presente una vendita imponibile in una valuta estera, è necessario usare il tasso ufficiale per la conversione di valuta IVA, come definito dall'ente Federal Tax Administration.  

Se tali tassi non corrispondono ai tassi di valuta usati nelle fatture di acquisto o di vendita, in seguito sarà necessario rettificare le aliquote IVA con un processo batch. Tali rettifiche possono essere eseguite solo tramite un'aliquota IVA autorizzata.  

È possibile eseguire questo processo batch ogni volta che si desidera, purché si verifichi di eseguirlo sempre prima di creare una dichiarazione IVA.  

> [!NOTE]  
>  Quando si usa una valuta contabile, verificare che il campo **Rettif. tasso di cambio IVA** nella pagina **Setup contabilità generale** sia impostato su **Nessuna rettifica**.  

Per ulteriori informazioni sulla valute IVA ed estere, vedere il sito Web [ESTV](https://go.microsoft.com/fwlink/?LinkId=285999).  

## <a name="to-adjust-an-exchange-rate"></a>Per rettificare un tasso di cambio  

1.  Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Valute**, quindi scegliere il collegamento correlato.  
2.  Scegliere l'azione **Tassi di cambio**.  
3.  Nella pagina **Tassi di cambio valuta** immettere l'aliquota IVA ufficiale per periodo per ogni valuta nei campi **Importo tasso di cambio IVA** e **Importo tasso di cambio IVA relazionale**.  
4.  Scegliere il pulsante **OK**.  
5.  Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Rettifica tassi di cambio**, quindi scegliere il collegamento correlato.  
6.  Nella Scheda dettaglio **Opzioni** compilare i campi come descritto nella tabella riportata di seguito.   

    |Campo|Descrizione|  
    |---------------------------------|---------------------------------------|  
    |**Data inizio**|Immettere una data per specificare l'inizio del periodo per cui verranno rettificati i movimenti.|  
    |**Data fine**|Immettere la data finale per la quale i movimenti verranno rettificati. Solitamente questa data equivale alla data di registrazione indicata nel campo **Data di registrazione**.|  
    |**Rettifica cambio per ammin. IVA**|Specificare se si desidera rettificare il tasso di cambio IVA.|  

7.  Scegliere **Stampa** per avviare il processo batch. Il processo batch controlla se i movimenti IVA devono essere rettificati e prepara un movimento di rettifica per ciascuno di tali movimenti per i conti di rettifica del tasso di cambio per IVA a esigibilità immediata o differita. Vengono rettificati anche i movimenti IVA esistenti.  

## <a name="see-also"></a>Vedi anche  
 [IVA svizzera](swiss-value-added-tax.md)   
 [Aliquote IVA per la Svizzera](vat-rates-for-switzerland.md)   
[Aggiornare i tassi di cambio valuta](../../finance-how-update-currencies.md)  
[Impostare una valuta contabile addizionale](../../finance-how-setup-additional-currencies.md)
