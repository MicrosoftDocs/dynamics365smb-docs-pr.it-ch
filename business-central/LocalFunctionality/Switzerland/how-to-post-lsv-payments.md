---
title: Come registrare pagamenti LSV+
description: È possibile registrare pagamenti dopo aver ricevuto l'avviso di pagamento LSV+ (Lastschrift Verfahren) dalla banca.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 4df119680c453db8e5f3b1bdc4ad8d3cb3d750b6
ms.sourcegitcommit: a7cb0be8eae6ece95f5259d7de7a48b385c9cfeb
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 07/08/2021
ms.locfileid: "6435698"
---
# <a name="post-lsv-payments"></a>Registrare pagamenti LSV+
È possibile registrare pagamenti dopo aver ricevuto l'avviso di pagamento LSV+ (Lastschrift Verfahren) dalla banca.  

## <a name="to-post-lsv-payments"></a>Registrare pagamenti LSV+  

1.  Scegliere la ![lampadina che apre la funzionalità delle informazioni.](../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immettere **Registrazioni incassi**, quindi selezionare il collegamento correlato.  
2.  Selezionare le registrazioni richieste, quindi scegliere l'azione **Modifica registrazioni**.  

    > [!NOTE]  
    >  È possibile selezionare il batch registrazioni per LSV in cui è definito il conto di contropartita da considerare. Non è possibile importare più di una riga delle registrazioni LSV nelle stesse registrazioni incassi. Per ulteriori informazioni, vedere la pagina Registrazioni incassi.  

3.  Scegliere l'azione **Recupera da registrazioni LSV**.  
4.  Nella pagina **Lista registrazioni LSV** selezionare la riga di registrazioni LSV da importare nelle registrazioni incassi.  

    > [!NOTE]  
    >  È possibile importare solo righe di registrazioni in cui il campo **Stato LSV** è impostato su **File creato**.  

5.  Scegliere il pulsante **OK**.  

    La riga delle registrazioni LSV viene importata nelle registrazioni incassi. Il valore del campo **Stato LSV** nella pagina **Lista registrazioni LSV** viene modificato da **File creato** a **Completato**.  

    È possibile verificare i pagamenti importati e confrontarli con l'avviso di pagamento bancario nella pagina **Registrazioni incassi**. È anche possibile eliminare le righe di pagamento che la banca non ha potuto elaborare e per cui è necessario contattare direttamente il cliente.  

6.  Scegliere l'azione **Registra**.  

## <a name="see-also"></a>Vedi anche  
 [Pagamenti elettronici svizzeri tramite LSV+](swiss-electronic-payments-using-lsv-.md)   
 [Elaborare una riscossione LSV](how-to-process-an-lsv-collection.md)   
 [Chiudere una riscossione LSV](how-to-close-an-lsv-collection.md)   
 [Esportare pagamenti tramite LSV](how-to-export-payments-using-lsv.md) 


[!INCLUDE[footer-include](../../includes/footer-banner.md)]