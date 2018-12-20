---
title: Come utilizzare famiglie di articoli nella produzione | Microsoft Docs
description: "L'operazione principale da eseguire per personalizzare un calendario di base per la propria società, o per uno dei partner commerciali, è la modifica dello stato dei giorni lavorativi e non lavorativi."
services: project-madeira
documentationcenter: 
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
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 4e89cee3fb8b3c079cebf0665a1e068ac1f46fae
ms.contentlocale: it-ch
ms.lasthandoff: 09/28/2018

---
# <a name="work-with-production-families"></a>Utilizzare famiglie di prodotti
Una famiglia di prodotti consiste in un gruppo di articoli individuali la cui relazione si basa sulla similarità dei rispettivi processi di lavorazione. Formando delle famiglie di produzione, è possibile che alcuni articoli siano lavorati due o più volte nel corso di una produzione; questa operazione ottimizzerà il consumo di materiale.

Nel campo **Quantità** della finestra **Famiglie di prodotti**, immettere la quantità che sarà prodotta quando l'intera famiglia sarà stata lavorata una volta.

## <a name="example"></a>Esempio
Nei processi di perforazione, è possibile che da una lamina vengano prodotti contemporaneamente quattro pezzi di un articolo e 10 pezzi di un altro articolo differente. La perforatrice perforerà tutti i 14 pezzi in un'unica fase.

La creazione di famiglie di produzione riduce le quantità di scarto perché ciò che generalmente costituisce gli scarti rimanenti dalla produzione di pezzi di grandi dimensioni viene utilizzato per produrre i pezzi di piccole dimensioni.

## <a name="to-set-up-a-production-family"></a>Per impostare una famiglia di prodotti
1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Famiglie** e quindi scegliere il collegamento correlato.
2. Compilare i campi come necessario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-produce-based-on-a-production-familily"></a>Per produrre in base a una famiglia di prodotti
1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Ord. produzione confermati** e quindi scegliere il collegamento correlato.
2. Creare un nuovo ordine di produzione. Per ulteriori informazioni, vedere [Creare ordini di produzione](production-how-to-create-production-orders.md).
3. Nel campo **Tipo origine**, selezionare **Famiglie di prodotti**.  
4. Nel campo **Nr. risorsa**, selezionare la famiglia di prodotti pertinente.

## <a name="see-also"></a>Vedi anche
[Creare le distinte base di produzione](production-how-to-create-production-boms.md)  
[Impostazione della produzione](production-configure-production-processes.md)  
[Manufacturing](production-manage-manufacturing.md)    
[Pianif.](production-planning.md)   
[Magazzino](inventory-manage-inventory.md)  
[Acquisti](purchasing-manage-purchasing.md)  
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
