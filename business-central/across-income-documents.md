---
title: Utilizzare i documenti in entrata| Documenti Microsoft
description: È possibile gestire i documenti aziendali esterni in entrata, ad esempio le ricevute di pagamento o i PDF, gestire attività OCR e convertire i file in record e documenti in formato elettronico.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 8e02cd4627219c7ea439155b2b91b61e03534dc2
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 03/31/2021
ms.locfileid: "5788501"
---
# <a name="incoming-documents"></a>Documenti in entrata

Alcune transazioni commerciali non vengono registrate in [!INCLUDE[prod_short](includes/prod_short.md)] dall'inizio. Invece, un documento commerciale esterno arriva nella propria società come allegato a un messaggio e-mail o copia cartacea che è possibile scansionare e trasformare in file. Ciò è tipico degli acquisti, dove questi file di documenti in entrata rappresentano le ricevute di pagamento per le spese o i piccoli acquisti.

Dai PDF o dai file di immagine dei documenti in entrata è possibile impostare un servizio esterno OCR (Optical Character Recognition, riconoscimento ottico dei caratteri) in modo che generi documenti elettronici che possono essere convertiti in record di documenti in [!INCLUDE[prod_short](includes/prod_short.md)]. Scegliere un pacchetto di servizi appropriato per l'organizzazione e/o paese/area geografica. In alternativa, è possibile creare manualmente voci per rappresentare i documenti esterni.  

Nella pagina **Documenti in entrata** è possibile utilizzare diverse funzioni per esaminare le ricevute relative alle spese, gestire le attività OCR e convertire i file dei documenti in entrata, manualmente o automaticamente, nei relativi documenti o in righe di registrazione. I file esterni possono essere allegati in qualsiasi fase dell'elaborazione, ad esempio ai documenti registrati, nonché ai fornitori, clienti e movimenti di contabilità generale risultanti.

L'elaborazione di documenti in entrata è costituita dalle seguenti operazioni principali:

* Registrare i documenti esterni in [!INCLUDE[prod_short](includes/prod_short.md)] creando le righe nella pagina **Documenti in entrata** attenendosi a uno dei modi seguenti:
  * Manualmente, utilizzando le funzioni semplici da un PC o un dispositivo mobile, in uno dei seguenti modi:
    * Utilizzare il pulsante **Crea da file** e compilare i campi pertinenti nella pagina **Documento in entrata**. Il file viene automaticamente allegato.  
    * Utilizzare il pulsante **Nuovo** e compilare i campi pertinenti nella pagina **Documento in entrata** e allegare manualmente il relativo file.
    * Da un tablet o un telefono, utilizzare il pulsante **Crea da fotocamera** per creare un nuovo record di documento in entrata e quindi inviare l'immagine, ad esempio al servizio OCR.
  * Automaticamente, ricevendo il documento dal servizio OCR come documento elettronico dopo aver inviato tramite e-mail il PDF o il file di immagine correlato al servizio OCR. La Scheda dettaglio **Informazioni finanziarie** viene automaticamente compilata nella pagina **Documento in entrata**.
* Utilizzare il servizio OCR per convertire PDF o file di immagine in documenti elettronici che possono essere convertiti in record di documento in [!INCLUDE[prod_short](includes/prod_short.md)].
* Creare nuovi documenti o righe registrazione COGE dai record di un documento in entrata immettendo le informazioni mentre vengono lette nei file del documento in entrata.
* Allegare i file di documenti in entrata ai documenti di acquisto e vendita con qualsiasi stato, ad esempio fornitore, cliente e movimenti di contabilità generale derivanti dalla registrazione.
* Visualizzare i record di documenti in entrata e i relativi allegati in qualsiasi documento o movimento di acquisto e vendita oppure individuare tutti i movimenti di contabilità generale senza i record di documenti in entrata nella pagina **Piano dei conti**.

| A | Vedere |
| --- | --- |
| Impostare la funzionalità Documenti in entrata e impostare il servizio OCR. |[Impostare documenti in entrata](across-how-setup-income-documents.md) |
| Creare i record dei documenti in entrata, allegare i file, utilizzare OCR per convertire i file PDF in documenti elettronici, convertire documenti elettronici in record di documento, controllare i documenti di vendita e di acquisto registrati dei record di documenti in entrata. |[Elaborazione di documenti in entrata](across-process-income-documents.md) |

## <a name="see-related-training-at-microsoft-learn"></a>Vedere le informazioni relative al training in [Microsoft Learn](/learn/modules/incoming-documents-dynamics-365-business-central/index)

## <a name="see-also"></a>Vedere anche

[Acquisti](purchasing-manage-purchasing.md)  
[Utilizzo di [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]