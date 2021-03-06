---
title: Creare interazioni per i contatti e i segmenti| Documenti Microsoft
description: Descrive come creare interazioni per comunicazioni intercorse con i contatti e i segmenti in Business Central, ad esempio messaggi di posta diretta.
services: project-madeira
documentationcenter: ''
author: jswymer
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, prospect
ms.date: 04/01/2021
ms.author: jswymer
ms.openlocfilehash: 92965b353dadb78e50b11138a832115885518f4f
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 03/31/2021
ms.locfileid: "5780725"
---
# <a name="create-interactions-on-contacts-and-segments"></a>Creare interazioni per i contatti e i segmenti
È possibile creare interazioni per registrare tutte le interazioni e le comunicazioni intercorse con i contatti e i segmenti, ad esempio messaggi di posta.

Prima di creare interazioni, è necessario impostare i modelli di interazione. Per ulteriori informazioni, vedere [Impostare modelli di interazione](marketing-interactions.md).

## <a name="to-create-an-interaction"></a>Per creare un'interazione
1. Aprire il contatto, l'agente o il movimento log interazione.
2. Selezionare l'azione **Crea interazione**.
3. Compilare i campi e scegliere **OK**.

> [!NOTE]  
>   Se è necessario eseguire un'altra attività prima di terminare l'interazione, è possibile scegliere **Annulla**, quindi terminare l'interazione in un secondo momento. Ciò pospone l'interazione.

## <a name="to-finish-and-delete-postponed-interactions"></a>Per completare ed eliminare le interazioni differite
1. Aprire il contatto, l'agente o il movimento log interazione.
2. Scegliere **Interazioni differite**.
3. Selezionare l'interazione che si desidera chiudere e scegliere l'azione **Riprendi**.

## <a name="to-create-an-interaction-on-a-segment"></a>Per creare un'interazione in un segmento
1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Segmenti** e quindi scegliere il collegamento correlato.
2. Nella pagina **Segmento**, nella sezione **Interazione**, compilare i campi per specificare l'interazione che si desidera assegnare al segmento.

    Una volta assegnata un'interazione al segmento, è possibile personalizzare l'interazione per ogni singolo contatto all'interno del segmento, ad esempio selezionando un altro modello di interazione nelle righe della pagina **Segmento**.  
3. Per registrare il segmento e interazioni, selezionare l'azione **Log**. Verrà visualizzata la pagina **Log segmento**.
4. Se si desidera creare un nuovo segmento contenente gli stessi contatti, selezionare la casella di controllo **Crea segmento di follow-up**. Per creare un segmento di follow-up, è necessario specificare la numerazione dei segmenti nella pagina **Setup marketing**.

Un'interazione viene registrata per ogni contatto all'interno del segmento nella tabella **Mov. log interazione** e il segmento viene registrato. È possibile individuare i segmenti registrati nella pagina **Segmento registrato**.

Se è stata selezionata la casella di controllo **Crea segmento di follow-up**, verrà creato un nuovo segmento contenente gli stessi contatti del segmento appena registrato.

## <a name="see-also"></a>Vedi anche
[Registrazione di interazioni](marketing-interactions.md)  
[Gestione dei contatti](marketing-contacts.md)  
[Gestione delle opportunità di vendita](marketing-manage-sales-opportunities.md)  
[Utilizzo di Business Central](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]