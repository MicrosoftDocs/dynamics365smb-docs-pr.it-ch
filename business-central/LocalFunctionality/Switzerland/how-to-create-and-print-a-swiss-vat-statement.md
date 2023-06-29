---
title: 'Creare e stampare una dichiarazione IVA svizzera [CH]'
description: Questo argomento spiega come creare e stampare una dichiarazione IVA svizzera in base alle informazioni specificate nella pagina Setup registrazioni IVA.
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: null
ms.search.form: '11023, 11024'
ms.date: 06/25/2021
ms.author: edupont
---
# <a name="create-and-print-a-swiss-vat-statement-in-the-swiss-version"></a><a name="create-and-print-a-swiss-vat-statement-in-the-swiss-version"></a>Creare e stampare una dichiarazione IVA svizzera nella versione per la Svizzera
In base alle informazioni specificate nella pagina **Setup registrazioni IVA**, [!INCLUDE[prod_short](../../includes/prod_short.md)] può creare automaticamente un nuovo setup di registrazioni IVA per il reporting dell'IVA a esigibilità immediata. Prima di eseguire le procedure indicate in questo argomento, verificare che la registrazione IVA sia stata impostata con i valori specificati nei campi cifrati di vendite e acquisti.  

## <a name="to-set-up-a-swiss-vat-statement-template"></a><a name="to-set-up-a-swiss-vat-statement-template"></a>Per impostare un modello di dichiarazione IVA svizzera

1.  Scegliere la ![lampadina che apre la funzionalità delle informazioni.](../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immettere **Aggiorna definizione dichiarazione IVA**, quindi selezionare il collegamento correlato.  
2.  Selezionare una definizione nel campo **Nome definizione dichiarazione IVA**.
3.  Scegliere il pulsante **OK**. Selezionare il pulsante **Sì** per confermare che si desidera creare una nuova definizione.  
4.  Verificare la dichiarazione IVA risultante e modificarla in base alle esigenze.  

     La pagina Dichiarazione IVA contiene il campo **Crittografia dichiarazione IVA**, che indica la crittografia del report con cui verrà stampato il risultato. Questo campo viene popolato automaticamente dal processo batch in base alle informazioni della pagina **Setup registrazioni IVA**. Il campo può essere modificato, se necessario.  

## <a name="to-print-the-swiss-vat-statement"></a><a name="to-print-the-swiss-vat-statement"></a>Per stampare la dichiarazione IVA svizzera

1.  Scegliere la ![lampadina che apre la funzionalità delle informazioni.](../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immettere **Dichiarazione IVA svizzera**, quindi selezionare il collegamento correlato.  
2.  Nella Scheda dettaglio **Opzioni** compilare i campi come descritto nella tabella riportata di seguito.  

    |Campo|Descrizione|  
    |---------------------------------|---------------------------------------|  
    |**Tipo di data periodo**|Specifica il tipo di data utilizzata per il periodo a partire dalla quale i movimenti IVA vengono elaborati nel processo batch.|
    |**Data Inizio**|Immettere la data in cui si desidera che inizi l'intervallo di tempo per le righe della dichiarazione IVA visualizzate nel report.|  
    |**Data fine**|Immettere la data in cui si desidera che termini l'intervallo di tempo per le righe della dichiarazione IVA visualizzate nel report.|  
    |**Chiusi con nr. registro IVA**|Selezionare il registro IVA che contiene l'origine di registrazione dei movimenti di rettifica IVA. Questa opzione valuta i periodi contabili già liquidati. Quando si sceglie questa opzione, non specificare opzioni nei campi **Includi movimenti IVA** seguenti.|  
    |**Includi movimenti IVA**|Selezionare una delle opzioni disponibili.|  
    |**Includi movimenti IVA**|Selezionare una delle opzioni disponibili.|  
    |**% aliquota normale**|Immettere l'aliquota IVA standard applicabile al periodo di tempo.|  
    |**Aliquota ridotta %**|Immettere l'aliquota IVA ridotta per determinati beni e servizi.|  
    |**Aliquota alloggio %**|Immettere l'aliquota IVA per alloggi applicabile al periodo di tempo.|  
    |**Normale (Altra aliquota) %**|Immettere un'aliquota IVA alternativa per le transazioni standard applicabile a determinate transazioni durante il periodo di tempo.|  
    |**Ridotta (Altra aliquota) %**|Immettere un'aliquota IVA alternativa per altre transazioni applicabile a determinate transazioni durante il periodo di tempo.|  
    |**Alloggio (altra aliquota) %**|Immettere un'aliquota IVA alternativa per alloggi applicabile a determinate transazioni durante il periodo di tempo.|  
    |**Mostra importi in valuta contabile addizionale**|Selezionare questa opzione per visualizzare una valuta contabile addizionale.|  

## <a name="see-also"></a><a name="see-also"></a>Vedere anche
 [IVA svizzera](swiss-value-added-tax.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
