---
title: Gestione del magazzino per la Svizzera
description: I miglioramenti svizzeri includono funzioni speciali di gestione magazzino.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 03/06/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: c6f10f8252c00bf0a599f9fa794ee36c41ce92be
ms.openlocfilehash: 5daae157434867c07bac55310ac1b24ea34df06c
ms.contentlocale: it-ch
ms.lasthandoff: 07/31/2018

---
# <a name="swiss-inventory-management"></a>Gestione del magazzino per la Svizzera
[!INCLUDE[d365fin](../../includes/d365fin_md.md)] include i miglioramenti svizzeri per la gestione magazzino. È incluso quanto segue:  

- Dichiarazione dettagliata.  Per ulteriori informazioni vedere il report Magazzino - Statistiche di vendita e il report Magazzino - Lista.  
- La capacità di monitorare una fattura con più spedizioni.  
- L'inclusione di un codice ubicazione scheda articolo come il codice ubicazione predefinito per le righe di vendita e le registrazioni articoli. Per ulteriori informazioni, vedere [Impostare le ubicazioni](../../inventory-how-setup-locations.md).

## <a name="managing-item-details"></a>Gestione dettagli articolo  
Le aziende possono disporre di magazzini diversi per categorie di prodotti diversi. In questi casi, è necessario utilizzare il codice ubicazione predefinito recuperato dalla scheda articolo. Quando si definisce un codice ubicazione per un articolo, questo viene trasferito nelle righe di vendita e nelle registrazioni articoli come codice di ubicazione articoli predefinito. Per ulteriori informazioni, vedere le tabelle Righe vendite e Righe reg. magazzino.  

Ulteriori informazioni, come il numero cliente, il codice dell'indirizzo di spedizione e il codice venditore del cliente, vengono memorizzate nei movimenti contabili articoli. Queste informazioni consentono di creare criteri di dichiarazione personalizzati, come i ricavi per cliente e gli accantonamenti per articoli o vendite per i venditori. Per ulteriori informazioni, vedere la tabella Mov. contabili articoli.  

## <a name="invoices-with-multiple-shipments"></a>Fatture con più spedizioni  
Se sono state registrate più spedizioni per un cliente, è possibile creare una fattura combinata con la funzione **Prendi righe di spedizione**. Per ulteriori informazioni, vedere la finestra Prendi righe di spedizione. Quando si utilizza questa funzione, il testo creato nelle righe della fattura include informazioni sul numero di spedizione e sulla data di spedizione. Ad esempio, il testo potrebbe essere Nr. spedizione 102040 di 25.01.01. Ciò consente di tracciare facilmente le fatture con più spedizioni.  

## <a name="see-also"></a>Vedi anche  
 [Copiare articoli esistenti in nuovi articoli](how-to-copy-existing-items-to-new-items.md)   
 [Disattivare la tracciabilità dei costi articolo](how-to-deactivate-item-cost-tracking.md)   
 [Funzionalità locale per la Svizzera](switzerland-local-functionality.md)   
 [Impostare le ubicazioni](../../inventory-how-setup-locations.md)

