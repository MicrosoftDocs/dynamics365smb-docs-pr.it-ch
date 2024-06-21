---
title: Come stampare dichiarazioni IVA svizzere (versione precedente)
description: La dichiarazione IVA svizzera è il rapporto di calcolo standard per la realizzazione dell'IVA. È possibile stampare questo rapporto e utilizzarlo per le dichiarazioni fiscali trimestrali.
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: null
ms.date: 04/01/2021
ms.author: bholtorf
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---
# <a name="print-swiss-vat-statements-older-version"></a>Stampare dichiarazioni IVA svizzere (versione precedente)

> [!NOTE]  
>  Questo argomento è mantenuto per la compatibilità con le versioni precedenti del report **Dichiarazione IVA svizzera**. Per informazioni sull'utilizzo della più recente dichiarazione IVA svizzera, vedere Dichiarazione IVA svizzera.  

La **dichiarazione IVA svizzera** è il rapporto di calcolo standard per la realizzazione dell'IVA. È possibile stampare questo rapporto e utilizzarlo per le dichiarazioni fiscali trimestrali. Nella **dichiarazione IVA svizzera** vengono incluse le seguenti informazioni:  

- Un movimento IVA.  
- I movimenti di rettifica IVA.  
- Una scheda contabile.  

## <a name="to-print-the-swiss-vat-statement"></a>Per stampare la dichiarazione IVA svizzera

1.  Scegliere la ![lampadina che apre la funzionalità delle informazioni.](../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immettere **Dichiarazione IVA svizzera**, quindi selezionare il collegamento correlato.  

    > [!NOTE]  
    >  Verrà ricevuto un messaggio indicante che la **dichiarazione IVA svizzera** viene aperta nella lingua locale.  

2.  Nella Scheda dettaglio **Opzioni** compilare i campi come descritto nella tabella riportata di seguito.  

    |Campo|Descrizione|  
    |---------------------------------|---------------------------------------|  
    |**Chiusi con nr. di registrazione**|Selezionare le registrazioni di contabilità generale che contengono l'origine di registrazione dei movimenti di rettifica IVA. Questo campo valuta i periodi contabili già liquidati.|  
    |**Aperti fino alla data**|Seleziona l'ultima data per la liquidazione di movimenti IVA aperti o non liquidati.|  
    |**Mostrare registrazioni**|Specifica se verranno stampati tutti i movimenti IVA per ciascun gruppo.|  
    |**Mostrare registrazioni di conguaglio**|Specifica se verranno stampati i movimenti IVA e i movimenti di contabilità generale con riepiloghi chiusi o imposta registrata.|  
    |**Aliquota normale IVA %**|Selezionare le aliquote IVA tipiche correnti utilizzate per assegnare le aliquote corrette ai gruppi di attività e prodotti definiti nelle impostazioni IVA.|  
    |**Aliquota ridotta IVA %**|Selezionare le aliquote di imposta ridotte correnti utilizzate per assegnare le aliquote corrette ai gruppi di attività e prodotti definiti nelle impostazioni IVA.|  
    |**% IVA aliquota speciale**|Selezionare le aliquote di imposta speciali correnti utilizzate per assegnare le aliquote corrette ai gruppi di attività e prodotti definiti nelle impostazioni IVA.|  
    |**Conto C/G IVA investimenti/costi d'esercizio**|Selezionare il conto di contabilità generale per l'IVA.|  
    |**Consumo proprio cat. reg. bus. IVA**|Seleziona il gruppo di attività e prodotti per il proprio consumo.|  
    |**Categoria reg. business servizi esteri**|Seleziona il gruppo di attività e prodotti per il servizio estero.|  
    |**Esportazioni cat. reg. bus.**|Seleziona il gruppo di attività e prodotti per le esportazioni.|  

3.  Scegliere il pulsante **Stampa** per stampare la dichiarazione IVA oppure scegliere il pulsante **Anteprima** per visualizzarla sullo schermo.  

## <a name="see-also"></a>Vedere anche
 [IVA svizzera](swiss-value-added-tax.md)   
 [Aliquote IVA per la Svizzera](vat-rates-for-switzerland.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
