---
title: Impostare e gestire un budget per una commessa| Documenti Microsoft
description: Descrive come pianificare le risorse, prevedere e controllare i costi di un progetto impostando un budget per ciascuna commessa.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project budget, forecast
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 995d181496dc1827f21c0b3edd9e52dd6c15c297
ms.contentlocale: it-ch
ms.lasthandoff: 09/28/2018

---
# <a name="manage-job-budgets"></a>Gestire budget per le commesse
È possibile impostare un budget per ogni commessa. Il budget viene utilizzato per pianificare le risorse allocate a una commessa. Il budget può essere generale con pochi movimenti oppure può contenere più movimenti divisi in livelli di attività. È quindi possibile confrontare gli importi previsti con l'utilizzo effettivo come registrato nelle registrazioni commesse. Monitorando le differenze tra l'utilizzo effettivo e quello a budget, è possibile controllare un progetto in corso e migliorare la qualità di commesse future riducendo il rischio di sottovalutazione dei costi.

Di seguito viene descritto come stimare i costi a budget durante la pianificazione. Per informazioni su come registrare i prezzi e i costi di commesse a budget rispetto a quelli effettivi, vedere [Registrare l'utilizzo nelle commesse](projects-how-record-job-usage.md).  

## <a name="JobBudgetCosts"></a> Per stimare i costi a budget per una commessa
Quando un cliente desidera conoscere il prezzo di una commessa che verrà fatturata in base all'utilizzo, è necessario determinare i costi a budget per la commessa. A tale scopo, utilizzare la finestra **Righe task commessa**.

1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Commesse** e quindi scegliere il collegamento correlato.  
2. Aprire una commessa appropriata.
3. Selezionare una riga di task di tipo Registrazione quindi scegliere l'azione **Righe pianificazione commessa**.
4. In una nuova riga, compilare i campi in base alle esigenze. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]   

Per il campo **Tipo riga** fare riferimento alle seguenti informazioni.  

| Tipo riga | Descrizione |
| --- | --- |
| **Sia Budget sia fatturabile** |Gli importi relativi a costi e prezzo immessi nella riga di pianificazione sono i costi a budget per la riga di pianificazione specifica. L'importo dei prezzi verrà fatturato. |
| **Budget** |Al cliente non viene addebitato l'utilizzo. L'utilizzo non è trasferito in una fattura ma verrà comunque utilizzato nel calcolo di WIP. |
| **Fatturabile** |Al cliente viene addebitato l'utilizzo. La quantità viene trasferita nella fattura, in base alla quantità specificata nel campo Qtà da trasferire in fattura. |

> [!NOTE]  
>   Il campo **Data pianificazione** per la riga di pianificazione contiene la data in cui è previsto il completamento dell'utilizzo correlato alla riga di pianificazione. È inoltre la data in cui la riga di pianificazione può essere trasferita a una fattura vendita ed essere registrata.  

> [!NOTE]  
>   Quando si compila il campo **Quantità**, tutte le informazioni sul prezzo totale e i costi totali saranno calcolate e immesse per quella riga di registrazione. È possibile modificarle in qualsiasi momento.

Nella finestra **Scheda commessa**, è possibile ora vedere un riepilogo dei costi a budget totali, del prezzo a budget, del costo e del prezzo fatturabili per ciascun task.

Per informazioni su come registrare i prezzi e i costi di commesse a budget rispetto a quelli effettivi, vedere [Registrare l'utilizzo nelle commesse](projects-how-record-job-usage.md).

## <a name="see-also"></a>Vedi anche
[Gestione progetti](projects-manage-projects.md)  
[Finanze](finance.md)  
[Acquisti](purchasing-manage-purchasing.md)         
[Vendite](sales-manage-sales.md)      
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
