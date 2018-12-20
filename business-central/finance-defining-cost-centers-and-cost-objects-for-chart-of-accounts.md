---
title: Definizione dei centri di costo e degli oggetti di costo per il piano dei conti | Microsoft Docs
description: "È possibile trasferire automaticamente i movimenti delle entrate e delle spese della contabilità generale alla contabilità industriale per ogni registrazione di contabilità generale o tramite un processo batch. Durante il trasferimento, il sistema trasferisce solo i movimenti che sono già stati collegati a un centro di costo o a un oggetto di costo. Per stabilire un trasferimento significativo, è necessario assicurarsi che i centri di costo e gli oggetti di costi siano correttamente definiti."
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
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 5da3967e99bf8a1d5628159a542885ffd1113a02
ms.contentlocale: it-ch
ms.lasthandoff: 03/22/2018

---
# <a name="defining-cost-centers-and-cost-objects-for-chart-of-accounts"></a>Definizione dei centri di costo e degli oggetti di costo per il piano dei conti
È possibile trasferire automaticamente i movimenti delle entrate e delle spese della contabilità generale alla contabilità industriale per ogni registrazione di contabilità generale o tramite un processo batch. Durante il trasferimento, con [!INCLUDE[d365fin](includes/d365fin_md.md)] è possibile trasferire solo i movimenti che sono già stati collegati a un centro di costo o a un oggetto di costo. Per stabilire un trasferimento significativo, è necessario assicurarsi che i centri di costo e gli oggetti di costi siano correttamente definiti.  

## <a name="defining-default-dimension-values-for-general-ledger-accounts"></a>Definizione dei valori dimensioni di default per i conti di contabilità generale  
Per ogni conto di contabilità generale, è possibile definire i valori dimensioni di default nella tabella **Dimensione di default**. Nell'esempio seguente viene illustrato come sia sempre necessaria la presenza di un centro di costo REPARTO e mai quella di un oggetto di costo PROGETTO quando si effettua una registrazione in un conto di contabilità generale.  

|**Codice dimensione**|**Registrazione valore**|  
|------------------------------------------|-----------------------------------------|  
|Reparto|Codice obbligatorio|  
|Progetto|Nessun Cod.|  

## <a name="defining-dimension-values-for-overhead-costs-and-direct-costs"></a>Definizione dei valori dimensioni per i costi generali e diretti  
 È possibile trasferire i costi generali a un centro di costo e i costi diretti a un oggetto di costo. Nella tabella seguente viene mostrata la combinazione ottimale dei valori di impostazione delle dimensioni.  

|Trasferisci a|Registrazione del centro di costo|Registrazione dell'oggetto di costo|  
|-----------------|-------------------------|-------------------------|  
|Centro di costo|Codice obbligatorio|Nessun Cod.|  
|Oggetto di costo|Nessun Cod.|Codice obbligatorio|  

> [!NOTE]  
>  Per garantire che il centro di costo e l'oggetto di costo predefiniti impostati nella contabilità generale vengano riportati automaticamente nella contabilità industriale, selezionare la casella di controllo **Verifica registrazioni CG** nella finestra Setup contabilità industriale.  

## <a name="see-also"></a>Vedi anche  
[Contabilizzazione dei costi](finance-manage-cost-accounting.md)  
[Impostare i centri di costo](finance-how-to-set-up-cost-centers.md)   
[Impostare gli oggetti di costo](finance-how-to-set-up-cost-objects.md)  
[Utilizzo di [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
