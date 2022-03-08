---
title: Come esportare pagamenti tramite LSV
description: È possibile esportare o creare file LSV+ (Lastschrift Verfahren) che contengono informazioni sui pagamenti dopo aver chiuso la riscossione LSV. È possibile inviare i file generati alla banca su un disco oppure usare un trasferimento file elettronico, ad esempio tramite il servizio di online banking o tramite un portale Internet.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: edupont
ms.openlocfilehash: 0532f4f5b3562ba48c27cce6a96469fc738bbbad
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 09/09/2020
ms.locfileid: "3779849"
---
# <a name="export-payments-using-lsv"></a>Esportare pagamenti tramite LSV
È possibile esportare o creare file LSV+ (Lastschrift Verfahren) che contengono informazioni sui pagamenti dopo aver chiuso la riscossione LSV. È possibile inviare i file generati alla banca su un disco oppure usare un trasferimento file elettronico, ad esempio tramite il servizio di online banking o tramite un portale Internet.  

## <a name="to-export-payments-using-lsv"></a>Per esportare pagamenti tramite LSV  

1.  Scegliere l'![icona a forma di lampadina che consente di aprire la funzionalità delle informazioni](../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Lista registrazioni LSV** e quindi scegliere il collegamento correlato.  
2.  Nella pagina **Lista registrazioni LSV** selezionare le registrazioni LSV desiderate.  
3.  Scegliere l'azione **Scrivi file LSV**.  
4.  Nella pagina **Scrivi file LSV**, nella Scheda dettaglio **Opzioni** compilare i campi come descritto nella tabella seguente.  

    |Campo|Descrizione|  
    |---------------------------------|---------------------------------------|  
    |**Nr.**|Specifica il numero di registrazioni LSV da esportare.|  
    |**Test**|Specifica se si inviano consegne di prova alla banca. La banca non elabora file di test.|  

5.  Tutte le righe correlate vengono trasferite alle registrazioni LSV. Il file LSV viene generato nella cartella determinata in precedenza.  

## <a name="see-also"></a>Vedi anche  
 [Pagamenti elettronici svizzeri tramite LSV+](swiss-electronic-payments-using-lsv-.md)   
 [Elaborare una riscossione LSV](how-to-process-an-lsv-collection.md)   
 [Chiudere una riscossione LSV](how-to-close-an-lsv-collection.md)   
 [Registrare pagamenti LSV+](how-to-post-lsv-payments.md)
