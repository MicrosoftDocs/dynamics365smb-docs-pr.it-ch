---
title: Come importare pagamenti ESR
description: "Dopo aver ricevuto un pagamento da un cliente, si riceve un file che contiene informazioni sulle fatture pagate. È possibile ricevere questo file dalla banca in formato elettronico oppure tramite e-mail."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b34f276a764f0e828fbc1f015429df9852242a4c
ms.openlocfilehash: d1918ebb1be6d4b9dac0a190385081a5e3b71b42
ms.contentlocale: it-ch
ms.lasthandoff: 03/22/2018

---
# <a name="import-esr-payments"></a>Importare i pagamenti ESR
Dopo aver ricevuto un pagamento da un cliente, si riceve un file che contiene informazioni sulle fatture pagate. È possibile ricevere questo file dalla banca in formato elettronico oppure tramite e-mail.  

È possibile importare dati di fattura ESR (polizza di versamento con numero di riferimento, in tedesco ESR, Einzahlungsschein mit Referenznummer) dal file, stampare i dati tramite il report ESR della fattura di vendita o tramite il report di tagliandi ESR di vendita ed eseguire la verifica prima della registrazione. Per ulteriori informazioni, vedere [Stampare fatture ESR](how-to-print-esr-invoices.md).  

## <a name="to-import-esr-payments"></a>Per importare pagamenti ESR  

1.  Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Registrazioni incassi**, quindi scegliere il collegamento correlato.  
2.  Nel campo **Nome batch** selezionare il batch contabile necessario.  

    > [!NOTE]  
    >  Prima di importare il file ESR, è necessario che le registrazioni siano vuote. Non è possibile importare più di un file ESR nelle stesse registrazioni incassi.  

3.  Scegliere l'azione **Leggi file ESR**.  

    > [!NOTE]  
    >  Se è stata definita più di una banca ESR, viene visualizzato un messaggio di avviso che indica di scegliere la banca pertinente. Per ulteriori informazioni, vedere la tabella Setup ESR.  

4.  Scegliere il pulsante **Sì**, quindi scegliere il pulsante **OK**.  

Le informazioni sui pagamenti vengono importate nelle righe di registrazioni. I pagamenti vengono applicati automaticamente alle rispettive fatture in base a numeri di riferimento ESR univoci.  

## <a name="see-also"></a>Vedi anche  
 [Pagamenti elettronici svizzeri tramite ESR](swiss-electronic-payments-using-esr.md)   
 [Stampare fatture ESR](how-to-print-esr-invoices.md)
