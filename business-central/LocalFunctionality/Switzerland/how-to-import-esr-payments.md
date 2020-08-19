---
title: Come importare pagamenti ESR
description: Dopo aver ricevuto un pagamento da un cliente, si riceve un file che contiene informazioni sulle fatture pagate. È possibile ricevere questo file dalla banca in formato elettronico oppure tramite e-mail.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: 19c9947e8a036df4755846e0ae3f627097d21ebf
ms.sourcegitcommit: 007b331b6974983ee614db0406f00777da359ecb
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 08/10/2020
ms.locfileid: "3677101"
---
# <a name="import-esr-payments"></a>Importare i pagamenti ESR
Dopo aver ricevuto un pagamento da un cliente, si riceve un file che contiene informazioni sulle fatture pagate. È possibile ricevere questo file dalla banca in formato elettronico oppure tramite e-mail.  

È possibile importare dati di fattura ESR (polizza di versamento con numero di riferimento, in tedesco ESR, Einzahlungsschein mit Referenznummer) dal file, stampare i dati tramite il report ESR della fattura di vendita o tramite il report di tagliandi ESR di vendita ed eseguire la verifica prima della registrazione. Per ulteriori informazioni, vedere [Stampare fatture ESR](how-to-print-esr-invoices.md).  

## <a name="to-import-esr-payments"></a>Per importare pagamenti ESR  

1.  Scegliere l'![icona a forma di lampadina che consente di aprire la funzionalità delle informazioni](../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Registrazioni incassi** e quindi scegliere il collegamento correlato.  
2.  Nel campo **Nome batch** selezionare il batch contabile necessario.  

    > [!NOTE]  
    >  Prima di importare il file ESR, è necessario che le registrazioni siano vuote. Non è possibile importare più di un file ESR nelle stesse registrazioni incassi.  

3.  Scegliere l'azione **Leggi file ESR**.  

    > [!NOTE]  
    >  Se è stata definita più di una banca ESR, viene visualizzato un messaggio di avviso che indica di scegliere la banca pertinente. Per ulteriori informazioni, vedere la tabella Setup ESR.  

4.  Scegliere il pulsante **Sì**, quindi scegliere il pulsante **OK**.  

Le informazioni sui pagamenti vengono importate nelle righe di registrazioni. I pagamenti vengono applicati automaticamente alle rispettive fatture in base a numeri di riferimento ESR univoci.  

## <a name="see-also"></a>Vedere anche  
 [Pagamenti elettronici svizzeri utilizzando ESR](swiss-electronic-payments-using-esr.md)   
 [Stampare fatture ESR](how-to-print-esr-invoices.md)
