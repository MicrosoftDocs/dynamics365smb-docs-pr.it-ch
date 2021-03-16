---
title: Come esportare pagamenti tramite LSV
description: È possibile esportare o creare file LSV+ (Lastschrift Verfahren) che contengono informazioni sui pagamenti dopo aver chiuso la riscossione LSV. È possibile inviare i file generati alla banca su un disco oppure usare un trasferimento file elettronico, ad esempio tramite il servizio di online banking o tramite un portale Internet.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: f17eedb34a61dbfbc279e442fc87d5e1cb516f0f
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 02/15/2021
ms.locfileid: "5383995"
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


[!INCLUDE[footer-include](../../includes/footer-banner.md)]