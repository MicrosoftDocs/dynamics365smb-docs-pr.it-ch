---
title: Come registrare pagamenti LSV+
description: È possibile registrare pagamenti dopo aver ricevuto l'avviso di pagamento LSV+ (Lastschrift Verfahren) dalla banca.
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
ms.openlocfilehash: f8dc03d4b11a14f442901ed40375467e9b8bf210
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 03/31/2019
ms.locfileid: "934064"
---
# <a name="post-lsv-payments"></a>Registrare pagamenti LSV+
È possibile registrare pagamenti dopo aver ricevuto l'avviso di pagamento LSV+ (Lastschrift Verfahren) dalla banca.  

## <a name="to-post-lsv-payments"></a>Registrare pagamenti LSV+  

1.  Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Registrazioni incassi**, quindi scegliere il collegamento correlato.  
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
