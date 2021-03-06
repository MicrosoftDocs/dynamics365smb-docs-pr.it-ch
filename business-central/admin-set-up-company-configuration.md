---
title: Impostare la configurazione della società | Documenti di Microsoft
description: Il processo di implementazione inizia con la soluzione Business Central necessaria. Riunificate tutte queste informazioni nei pacchetti di configurazione.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 3eefa0fcb40b4e925ca653f223f2d97ed10f370e
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 03/31/2021
ms.locfileid: "5777259"
---
# <a name="set-up-company-configuration"></a>Impostare la configurazione della società
Il processo di implementazione inizia con il partner Microsoft. Il partner è responsabile della valutazione dei dettagli relativi alla configurazione e della creazione di un pacchetto che il cliente è in grado di applicare in modo semplice. Prima di creare una nuova società, è necessario pianificare la modalità di configurazione. È necessario valutare i dati di setup di base e i tipi di dati che la soluzione [!INCLUDE[prod_short](includes/prod_short.md)] richiede. Riunificate tutte queste informazioni in pacchetti di configurazione.

RapidStart Services fornisce inoltre gli strumenti per eseguire la migrazione dei dati legacy, ad esempio clienti e fornitori.  

È consigliabile creare pacchetti di configurazione con la maggior parte delle tabelle di setup già compilate, in modo che, dopo l'applicazione del pacchetto, i clienti dovranno modificare soltanto alcune impostazioni. Ad esempio, quando si crea una nuova società, le tabelle **Nr. serie** e **Riga nr. serie** vengono compilate con numerazioni e numeri iniziali. Anche i campi corrispondenti **Nr. serie** corrispondenti nelle tabelle di setup vengono compilati automaticamente. Non è necessario immettere le serie di numerazione e altri dati di setup di base. È inoltre possibile modificare manualmente tutti i dati di default utilizzati con RapidStart Services utilizzando il foglio di lavoro configurazione.  

I pacchetti di configurazione sono costruiti in base a una società preconfigurata. Dopo aver configurato una società in base alle proprie esigenze, è possibile creare un pacchetto di configurazione contenente i dati pertinenti relativi a tale società. Dopo avere definito un modello di società, è quindi possibile utilizzarlo per creare una nuova società da configurare allo stesso modo.  

Per semplificare l'importazione dei dati master, quali informazioni relative a clienti e fornitori, è possibile utilizzare modelli di configurazione. I modelli di configurazione contengono una serie di impostazioni di default che vengono automaticamente assegnate ai record importati in [!INCLUDE[prod_short](includes/prod_short.md)].

Nella tabella seguente viene descritta una sequenza di task, con collegamenti agli argomenti che li descrivono.

|**Task**|**Vedere**|  
|------------|-------------|  
|Pianificare la configurazione di una società compilando il foglio di lavoro configurazione.|[Gestione della configurazione della società in un foglio di lavoro](admin-how-to-manage-company-configuration-in-a-worksheet.md)|  
|Creare un pacchetto di configurazione, personalizzare un pacchetto, assegnare tabelle a un pacchetto, esaminare o modificare dati esistenti del cliente, creare la nuova società e quindi spostare i dati dei test nell'ambiente di produzione.|[Preparazione di un pacchetto di configurazione](admin-how-to-prepare-a-configuration-package.md)| 

## <a name="see-also"></a>Vedere anche  
[Impostazione una società con RapidStart Services](admin-set-up-a-company-with-rapidstart.md)  
[Amministrazione](admin-setup-and-administration.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]