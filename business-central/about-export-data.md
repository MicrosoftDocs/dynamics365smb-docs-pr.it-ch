---
title: Esportare i dati di Business Central in Excel | Documenti Microsoft
description: È possibile esportare i report finanziari e i dati di Business Intelligence da Business Central in Excel o aprire i dati di Business Central in Excel.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: analysis, reporting, financial report, business intelligence, BI, Excel
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 4a6bfb8d20c13019807b2308737380c4fd31dcc6
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 03/31/2021
ms.locfileid: "5776515"
---
# <a name="exporting-your-business-data-to-excel"></a>Esportazione dei dati aziendali in Excel
Se si desidera utilizzare i dati di [!INCLUDE[prod_short](includes/prod_short.md)] in Excel, è possibile aprire tutti gli elenchi in Excel quindi utilizzarli con questo programma. Analogamente, se si desidera annullare la sottoscrizione a [!INCLUDE[prod_short](includes/prod_short.md)], è possibile esportare i dati in Excel per averli sempre a disposizione.

## <a name="opening-lists-in-excel"></a>Aprire gli elenchi in Excel
È possibile visualizzare i dati in Excel da qualsiasi registrazione, elenco o foglio di lavoro. Aprire la pagina che si desidera quindi scegliere **Apri in Excel**. Ad esempio, aprire l'elenco dei clienti (cercare **Clienti**) quindi scegliere **Apri in Excel**. Il browser chiederà conferma dell'apertura o del salvataggio della cartella di lavoro di Excel generata.  

> [!NOTE]
> Utilizzare questa opzione se non si desidera apportare modifiche e pubblicare di nuovo tali modifiche su [!INCLUDE[prod_short](includes/prod_short.md)].  

Ogni elenco include una serie di colonne e l'esportazione in Excel includerà tutte le colonne che sono incluse nella visualizzazione corrente. Se si desidera aggiungere o rimuovere colonne prima di aprire l'elenco in Excel, è sufficiente aprire il menu di scelta rapida per qualsiasi colonna e specificare le colonne che si desidera visualizzare. L'elenco delle colonne è diverso dalla maggior parte degli elenchi e riflette la struttura del database in cui i dati sono archiviati. Se non si è certi di tipo di dati contenuti in una determinata colonna, è possibile aggiungerla alla visualizzazione e quindi decidere di rimuoverlo di nuovo eventualmente.  

### <a name="edit-data-in-excel"></a>Modifica dei dati in Excel
L'esperienza [!INCLUDE[prod_short](includes/prod_short.md)] include un componente aggiuntivo per Excel in modo da poter modificare i dati in Excel. Per ulteriori informazioni, vedere [Analisi dei rendiconti finanziari in Microsoft Excel](finance-analyze-excel.md).  

## <a name="exporting-data-to-other-finance-systems"></a>Esportare i dati in altri sistemi contabili
Se si decide di annullare la sottoscrizione a [!INCLUDE[prod_short](includes/prod_short.md)], è possibile esportare i dati in Excel e averli a disposizione nel sistema finanziario.  

È possibile esportare tutte le pagine, naturalmente, ma potrebbe essere più di quanto effettivamente necessario. Prendere in considerazione di esportare le seguenti pagine essenziali e ricordarsi di aggiungere tutte le colonne come descritto in precedenza:  

* Piano dei conti  
* Clienti  
* Fornitori  
* Banche  
* Articoli  

Se si desidera esportare anche tutte le transazioni finanziarie, ovvero una grande quantità di dati, l'esportazione richiederà un tempo superiore. Le transazioni finanziarie sono visualizzate nella pagina **Movimenti C/G**.  

È consigliabile anche esportare i dati dalle pagine seguenti:  

* Movimenti contabili clienti  
* Movimenti contabili fornitori  
* Mov. contabili C/C bancari  
* Mov. contabili articoli  
* Setup registrazioni COGE  
* Cat. reg. clienti  
* Cat. reg. fornitori  
* Cat. reg. articoli  
* Cat. reg. bancarie  
* Budget C/G  
* Movimenti budget C/G  
* Offerte vendita  
* Fatture vendite  
* Fatture di acquisto  
* Contatti  
* Agenti  

> [!NOTE]  
> Se è stata impostata più di uno società in [!INCLUDE[prod_short](includes/prod_short.md)], è necessario esportare i dati relativi a ogni società.

> [!NOTE]
> È necessario disporre di almeno una delle seguenti autorizzazioni per aprire o modificare i dati in Excel:
>    - Set di autorizzazioni *D365 Azione esportazione Excel*  
>    - Autorizzazione di sistema 6110 *Consenti l'azione Esporta in Excel*.  

Per ulteriori informazioni, vedere [Per ottenere una sintesi delle autorizzazioni di un utente](ui-define-granular-permissions.md#to-get-an-overview-of-a-users-permissions).

## <a name="see-related-training-at-microsoft-learn"></a>Vedere le informazioni relative al training in [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)

## <a name="see-also"></a>Vedere anche
[Annullamento della sottoscrizione per [!INCLUDE[prod_short](includes/prod_short.md)]](admin-cancel.md)  
[Importazione dei dati aziendali da altri sistemi contabili](across-import-data-configuration-packages.md)  
[Analisi dei rendiconti finanziari in Microsoft Excel](finance-analyze-excel.md)  
[Finanze](finance.md)  
[Funzionalità aziendali generali](ui-across-business-areas.md)  
[Utilizzo di [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]