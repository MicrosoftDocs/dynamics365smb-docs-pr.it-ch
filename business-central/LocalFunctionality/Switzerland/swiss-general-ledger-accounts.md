---
title: Conti di contabilità generale per la Svizzera
description: I miglioramenti svizzeri includono funzioni speciali di conto C/G.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: 8e480a889182a33e51cb5a4dece751bb98b5a058
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 04/29/2019
ms.locfileid: "1240784"
---
# <a name="swiss-general-ledger-accounts"></a>Conti di contabilità generale per la Svizzera
[!INCLUDE[d365fin](../../includes/d365fin_md.md)] include i miglioramenti svizzeri per i conti C/G.

- Gestire i saldi in valuta estera di un conto bancario nella contabilità generale.  
- Ordinare i numeri di conto della contabilità generale nella pagina **Piano dei conti**.  
- Visualizzare l'anteprima degli effetti che avrebbe la contabilizzazione delle registrazioni COGE sui saldi di alcuni conti di contabilità generale prima di effettuarla effettivamente.  

## <a name="general-ledger-accounts-and-general-journals"></a>Conti di contabilità generale e registrazioni COGE  
Le aziende hanno spesso conti bancari diversi per le valute estere e hanno un conto C/G per ogni conto bancario. In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], è possibile impostare le informazioni relative al codice valuta e al saldo in valuta estera nella pagina **Piano dei conti**. Ciò consente di mantenere il saldo originale in valuta estera di un conto bancario. Per ulteriori informazioni, vedere [Contabilità generale e piano dei conti](../../finance-general-ledger.md).  

Ad esempio, un'azienda ha due conti bancari: uno per la valuta locale (VL) e uno per gli euro (EUR). È necessario creare un conto C/G per ciascun conto bancario. Per il conto in EUR, definire il codice valuta come **EUR** e contabilizzare le registrazioni in EUR o VL.  

Quando cambia il tasso di cambio per EUR e VL, è possibile aggiornare e modificare il saldo in valuta locale per il conto C/G EUR usando il processo di batch di rettifica dei tassi di cambio. Questo processo batch crea e registra i movimenti di rettifica della valuta nella contabilità generale e aggiorna il saldo VL.  

## <a name="data-type-for-general-ledger-accounts"></a>Tipo di dati per i conti C/G  
Il tipo di dati è impostato su un testo per il numero di conto C/G o il codice conto per supportare i requisiti di ordinamento per il piano dei conti comune Kontenrahmen Käfer (KMU) svizzero standardizzato. La lista dei numeri di conto viene ordinata in base al tipo di dati di testo. Il piano di conti KMU contiene i seguenti numeri di conto:  

- 1176  
- 119.0  
- 1190  

## <a name="viewing-temporary-balances-in-general-journals"></a>Visualizzazione di saldi temporanei nelle registrazioni di contabilità generale  
Prima di contabilizzare una registrazione COGE è possibile visualizzare l'anteprima degli effetti che avrebbe la contabilizzazione sui saldi di alcuni conti di contabilità generale. È possibile aprire una pagina di statistiche che mostra i saldi dei conti e i saldi delle righe attive che includevano i valori non registrati per la registrazione corrente. Per ulteriori informazioni, vedere [Visualizzare i saldi temporanei nelle registrazioni di contabilità generale](how-to-view-temporary-balances-in-general-ledger-journals.md).  

## <a name="see-also"></a>Vedi anche

[Visualizzare i saldi temporanei nelle registrazioni di contabilità generale](how-to-view-temporary-balances-in-general-ledger-journals.md)  
[Funzionalità locale per la Svizzera](switzerland-local-functionality.md)  
