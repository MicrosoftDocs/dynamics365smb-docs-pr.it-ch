---
title: "Come disattivare la tracciabilità dei costi articolo"
description: "Quando le scorte per un articolo non sono tracciate, non è necessario tenere traccia del costo dell'articolo né creare un movimento contabile articolo."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: f618203725ec854f3a66ef2501b16613a0394bd6
ms.contentlocale: it-ch
ms.lasthandoff: 03/22/2018

---
# <a name="deactivate-item-cost-tracking"></a>Disattivare la tracciabilità dei costi articolo
Quando le scorte per un articolo non sono tracciate, non è necessario tenere traccia del costo dell'articolo né creare un movimento contabile articolo.  

È possibile disattivare la tracciabilità dei costi per un articolo. In genere, la tracciabilità dei costi articolo deve essere disattivata per articoli di consumo, ad esempio prodotti di carta riciclata e servizi contati come articoli, quali i costi di parcheggio forfettari. La tracciabilità dei costi articolo deve essere disattivata per gli articoli per cui potrebbe essere fuorviante. Gli articoli per cui la tracciabilità dei costi è stata disattivata sono esclusi dagli impegni, dal controllo di disponibilità, dalla tracciabilità articolo e dai sistemi di pianificazione dei materiali.  

## <a name="to-deactivate-item-cost-tracking"></a>Per disattivare la tracciabilità dei costi articolo  

1.  Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "Cerca pagina o report"), immettere **Articoli**, quindi scegliere il collegamento correlato.  
2.  Selezionare l'articolo richiesto, quindi scegliere l'azione **Modifica**.  
3.  Nella Scheda dettaglio **Generale** selezionare la casella di controllo **Nessun stockkeeping**.  

    Quando si registra una transazione per questo articolo, non verrà creato alcun movimento contabile. Per ulteriori informazioni, vedere la tabella Mov. contabili articoli.  

    > [!NOTE]  
    >  Non è possibile selezionare la casella di controllo **Nessun stockkeeping** per un articolo per cui i movimenti contabili sono già stati registrati.  

4.  Scegliere il pulsante **OK**.  

## <a name="see-also"></a>Vedi anche  
 [Gestione del magazzino per la Svizzera](swiss-inventory-management.md)   
 [Bloccare gli articoli in magazzino per le vendite o gli acquisti](how-to-block-inventory-items-for-sales-or-purchases.md)

