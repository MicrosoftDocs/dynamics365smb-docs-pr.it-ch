---
title: Impostare i metodi preferiti per l'invio dei documenti di vendita | Documenti Microsoft
description: Descrive come impostare il metodo preferito di ogni cliente per l'invio dei documenti di vendita, ad esempio e-mail, PDF, documento elettronico, e così via.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: email, PDF, electronic document
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: b54decd14cfa1003747ef2a56244ed3865d1ccd2
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 03/31/2021
ms.locfileid: "5778565"
---
# <a name="set-up-document-sending-profiles"></a>Impostare profili di invio documenti
È possibile impostare per ogni cliente un metodo preferito di invio documenti di vendita, in modo da non dover selezionare un'opzione di invio ogni volta che si sceglie l'azione **Registra e invia**.

Nella pagina **Profili di invio documenti** si impostano differenti profili di vendita che è possibile selezionare dal campo **Profilo di invio documenti** nella scheda cliente. È possibile selezionare la casella di controllo **Default** per specificare che il profilo di invio documenti è il profilo predefinito per tutti i clienti, eccetto per quelli per i quali il campo **Profilo di invio documenti** è compilato con un altro profilo di invio.

Se si sceglie l'azione **Registra e invia** in un documento di vendita, nella finestra di dialogo **Registra e invia conferma** viene visualizzato anche il profilo di invio utilizzato, cioè quello impostato per il cliente o quello predefinito per tutti i clienti. Nella finestra di dialogo è possibile modificare il profilo di invio per il documento di vendita. Per ulteriori informazioni, vedere [Fatturare le vendite](sales-how-invoice-sales.md).
<br><br>  

> [!Video https://www.microsoft.com/en-us/videoplayer/embed/RE4jzHH?rel=0]

## <a name="to-set-up-a-document-sending-profile"></a>Per impostare un profilo di invio documenti
1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Profili di invio documenti** e quindi scegliere il collegamento correlato.
2. Nella pagina **Profili di invio documenti** scegliere l'azione **Nuovo**.
3. Compilare i campi come necessario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-specify-a-sending-profile-on-a-customer-card"></a>Per specificare un profilo di invio in una scheda cliente
1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Clienti** e quindi scegliere il collegamento correlato.
2. Aprire la scheda del cliente per cui si desidera impostare un profilo di invio.
3. Nel campo **Profilo di invio documenti** selezionare un profilo che è stato impostato secondo la procedura descritta in precedenza.

## <a name="see-also"></a>Vedere anche
[Setup Vendite](sales-setup-sales.md)  
[Vendite](sales-manage-sales.md)  
[Utilizzo di [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]