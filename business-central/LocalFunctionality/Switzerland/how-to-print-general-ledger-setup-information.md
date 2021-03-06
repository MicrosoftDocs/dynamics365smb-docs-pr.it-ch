---
title: Come stampare le informazioni di setup della contabilità generale
description: Prima di usare Business Central nelle attività giornaliere, è possibile eseguire il report Informazioni setup C/G per visualizzare i dati master configurati.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 1c39ebde2206524d81f9beccecc80b1b385cc6ca
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 03/31/2021
ms.locfileid: "5776560"
---
# <a name="print-general-ledger-setup-information"></a>Stampare le informazioni di setup della contabilità generale
Prima di usare [!INCLUDE[prod_short](../../includes/prod_short.md)] nelle attività giornaliere, è possibile eseguire il report **Informazioni setup C/G** per visualizzare i dati master configurati. È possibile esaminare i dati master in modo da disporre di una base rispetto alla quale eseguire un confronto e quindi verificare, ad esempio, di aver impostato le categorie di registrazione in modo corretto.  

## <a name="to-print-general-ledger-setup-information"></a>Per stampare le informazioni di setup della contabilità generale  

1.  Scegliere l'![icona a forma di lampadina che consente di aprire la funzionalità delle informazioni](../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Informazioni setup C/G** e quindi scegliere il collegamento correlato.  
2.  Nella Scheda dettaglio **Opzioni**, nel campo **Informazioni sull'installazione** selezionare l'area di dati master come descritto nella tabella seguente.  

    |Opzione|Descrizione|  
    |-------------------------------------|---------------------------------------|  
    |**Setup Registrazioni Generali - Dati società - Consolidamento**|Visualizza tabelle per il setup di contabilità generale, le informazioni sulla società e le business unit.|  
    |**Categorie registrazione**|Visualizza le tabelle di categorie di registrazione clienti, fornitori, magazzino e conti correnti bancari.|  
    |**Matrice registrazione**|Visualizza le tabelle di categorie di registrazione business generale, di registrazione articoli/servizi e di registrazione generale.|  
    |**Setup VAT**|Visualizza le tabelle di categorie di registrazione business IVA e di registrazione articoli/servizi IVA e del registrazioni IVA.|  
    |**Codice origine - Causale**|Visualizza le tabelle di origine, di setup del codice origine e delle causali.|  
    |**Verifica numerazione**|Selezionare questa opzione per fornire una panoramica dell'uso delle numerazioni in modo da identificare quelle problematiche per l'esportazione dei dai per GDPdU (Grundsätze zum Datenzugriff und zur Prüfbarkeit digitaler Unterlagen). Il report visualizzerà le numerazioni con uno dei problemi seguenti:<br /><br /> -   La numerazione consente l'inserimento manuale di numeri di documento.<br />-   La numerazione non è cronologica.<br />-   La numerazione è usata in più di un campo o tabella.|  

3.  Scegliere il pulsante **Stampa** per stampare il report oppure scegliere il pulsante **Anteprima** per visualizzarlo sullo schermo.  

## <a name="see-also"></a>Vedere anche  
[Impostazione di dati finanziari](../../finance-setup-finance.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]