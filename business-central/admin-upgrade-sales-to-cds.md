---
title: Aggiornamento di un'integrazione con Dynamics 365 Sales
description: Informazioni su come passare l'integrazione di Dynamics 365 Business Central con Dynamics 365 Sales alla versione più recente.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sales, crm, integration, integrating
ms.date: 04/01/2021
ms.author: bholtorf
ms.openlocfilehash: 772052fc88e0b8be7ec5276600b0c237e2d2f8b2
ms.sourcegitcommit: a76475f124e79440a5bba20577b335c4d50a2d83
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 05/12/2021
ms.locfileid: "6025826"
---
# <a name="upgrading-an-integration-with-dynamics-365-sales"></a>Aggiornamento di un'integrazione con Dynamics 365 Sales
[!INCLUDE[prod_short](includes/prod_short.md)] si integra con [!INCLUDE[prod_short](includes/cds_long_md.md)], che semplifica la connessione e la sincronizzazione dei dati con altre applicazioni di Dynamics 365, come [!INCLUDE[crm_md](includes/crm_md.md)] o anche le app che crei autonomamente. Se stai effettuando l'integrazione per la prima volta, ti consigliamo di farlo tramite [!INCLUDE[prod_short](includes/cds_long_md.md)]. Per ulteriori informazioni, vedi [Integrazione con Dataverse](admin-common-data-service.md).

Se hai già integrato [!INCLUDE[crm_md](includes/crm_md.md)] con [!INCLUDE[prod_short](includes/prod_short.md)], puoi continuare a sincronizzare i dati utilizzando la tua configurazione. Tuttavia, se aggiorni [!INCLUDE[prod_short](includes/prod_short.md)] o disattivi la tua integrazione [!INCLUDE[crm_md](includes/crm_md.md)], per riattivarla devi connetterti tramite [!INCLUDE[prod_short](includes/cds_long_md.md)]. 

> [!NOTE]
> La riconnessione tramite [!INCLUDE[prod_short](includes/cds_long_md.md)] applicherà le impostazioni di sincronizzazione predefinite e sovrascriverà tutte le configurazioni a tua disposizione. Ad esempio, verranno applicati i mapping di tabella predefiniti.

## <a name="to-upgrade-your-connection-to-use-dataverse"></a>Per aggiornare la connessione per utilizzare Dataverse
1. Apri la pagina **Setup connessione a Microsoft Dynamics 365** e disattiva l'interruttore **Abilitato** per eseguire la disconnessione di [!INCLUDE[crm_md](includes/crm_md.md)].
2. Apri la pagina **Setup connessione a Dataverse** e scegli l'interruttore **Abilitato** per attivare la connessione a [!INCLUDE[prod_short](includes/cds_long_md.md)].
  
   > [!NOTE]
   > Dopo aver abilitato la connessione, la soluzione di integrazione di Business Central viene distribuita a Dataverse.
3. Scegli **Ridistribuzione soluzione di integrazione** per reinstallare la soluzione di integrazione di Business Central.
4. Nella pagina **Setup connessione a Microsoft Dynamics 365**, attiva l'interruttore **Abilitato** per eseguire di nuovo la connessione a [!INCLUDE[crm_md](includes/crm_md.md)].
  
   > [!NOTE]
   > Dopo aver abilitato la connessione, la soluzione di integrazione di Business Central viene distribuita a [!INCLUDE[prod_short](includes/prod_short.md)]. Ciò consente l'integrazione di tabelle specifiche in [!INCLUDE[crm_md](includes/crm_md.md)], ad esempio ordini vendita, offerte e fatture.
5. Scegli **Ridistribuzione soluzione di integrazione** per reinstallare la soluzione di integrazione di Business Central.
6. Nella pagina **Impostazione della connessione di vendita**, scegli **Usa impostazione di sincronizzazione predefinita** per inizializzare i mapping della tabella di integrazione per [!INCLUDE[crm_md](includes/crm_md.md)].

   > [!IMPORTANT]
   > L'uso dell'azione **Usa impostazione di sincronizzazione predefinita** applicherà le mappature della tabella di integrazione predefinita. Tutte le mappature personalizzate verranno sovrascritte. Se si dispone di mappature personalizzate che si desidera mantenere, è consigliabile esportarle in Excel o parlare con il proprio partner Microsoft di altri metodi per conservare le mappature personalizzate.    

## <a name="see-also"></a>Vedere anche
[Integrazione con Dynamics 365 Sales](admin-prepare-dynamics-365-for-sales-for-integration.md)  
[Integrazione con Microsoft Dataverse](admin-common-data-service.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]