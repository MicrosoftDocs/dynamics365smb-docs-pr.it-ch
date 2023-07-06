---
title: 'Elaborare una riscossione LSV [CH]'
description: Utilizzare registrazioni LSV per creare ed elaborare i pagamenti di clienti Lastschrift Verfahren (LSV+).
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: null
ms.search.form: '3010830, 3010831, 3010832,3010834, 3010835'
ms.date: 06/21/2021
ms.author: edupont
---
# <a name="process-an-lsv-collection-in-the-swiss-version"></a><a name="process-an-lsv-collection-in-the-swiss-version"></a><a name="process-an-lsv-collection-in-the-swiss-version"></a>Elaborare una riscossione LSV nella versione per la Svizzera
Utilizzare la pagina **Registrazioni LSV** per creare ed elaborare i pagamenti di clienti Lastschrift Verfahren (LSV+). È possibile registrare questi pagamenti nella registrazione incassi, creare un file LSV e stampare il RIBA. Per ulteriori informazioni, vedere la pagina Registrazioni incassi e [Esportare pagamenti tramite LSV](how-to-export-payments-using-lsv.md).  

Quando si esegue il processo batch **Riscossione suggerimenti LSV**, ogni riscossione suggerita viene registrata nella riga registrazioni LSV e le fatture aperte vengono trasferite nelle registrazioni LSV. Per ulteriori informazioni, vedere la tabella Registrazioni LSV.  

È possibile visualizzare, modificare o eliminare le righe pagamenti suggeriti. Se si corregge l'importo suggerito, la differenza viene contrassegnata come uno sconto. È possibile eseguire più volte il processo batch per diversi gruppi di clienti. Le linee di suggerimento possono essere collocate nelle stesse registrazioni.  

## <a name="to-create-an-lsv-collection"></a><a name="to-create-an-lsv-collection"></a><a name="to-create-an-lsv-collection"></a>Per creare una riscossione LSV

1.  Scegliere la ![lampadina che apre la funzionalità delle informazioni.](../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immettere **Lista registrazioni LSV**, quindi selezionare il collegamento correlato.  
2.  Scegliere l'azione **Nuovo**.  
3.  Nella pagina **Lista registrazioni LSV** compilare i campi obbligatori come indicato nella tabella riportata di seguito.  

    |Campo|Descrizione|  
    |---------------------------------|---------------------------------------|  
    |**Codice banca LSV**|Selezionare il codice banca LSV per la banca che eseguirà la riscossione.|  
    |**Descrizione Registro LSV**|Immettere una descrizione per il movimento.|

4.  Selezionare il movimento registrazioni LSV e scegliere l'azione **Riscossione suggerimenti LSV** per creare i pagamenti da riscuotere automaticamente da LSV+.  
5.  Nella pagina **Riscossione suggerimenti LSV**, nella Scheda dettaglio **Opzioni** compilare i campi come descritto nella tabella seguente.  

    |Campo|Descrizione|  
    |---------------------------------|---------------------------------------|  
    |**Nr.**|Immettere il numero registrazioni LSV.|  
    |**Scadenza dal**|Specificare la data di scadenza iniziale per i movimenti aperti da suggerire per la riscossione.|  
    |**Scadenza fino al**|Specificare la data di scadenza finale per i movimenti aperti da suggerire per la riscossione.|  
    |**Data incasso**|Specifica la data di chiusura della riscossione. L'ordine LSV+ deve essere inviato almeno tre giorni lavorativi prima della data di riscossione.|  

6.  Scegliere il pulsante **OK**.  

Tutte le righe correlate vengono trasferite alle registrazioni LSV. Dopo aver elaborato la riscossione LSV, è possibile visualizzare, controllare o modificare i pagamenti suggeriti nella pagina **Registrazioni LSV**. Per ulteriori informazioni, vedere la tabella Riga delle registrazioni LSV.  

## <a name="to-manage-suggested-payments"></a><a name="to-manage-suggested-payments"></a><a name="to-manage-suggested-payments"></a>Per gestire i pagamenti suggeriti

1.  Nella pagina **Lista registrazioni LSV**, selezionare il movimento registrazioni richiesto e scegliere l'azione **Riga delle registrazioni LSV**.  

    È possibile visualizzare e modificare i pagamenti suggeriti in questa pagina. È possibile inserire manualmente i pagamenti richiesti. Perle righe registrazioni nuove, il campo **Stato LSV** è impostato su **Aperto** per indicare che la fattura non è pagata.  

3.  Scegliere il pulsante **OK**.  

## <a name="see-also"></a><a name="see-also"></a><a name="see-also"></a>Vedi anche
 [Pagamenti elettronici svizzeri tramite LSV+](swiss-electronic-payments-using-lsv-.md)   
 [Chiudere una riscossione LSV](how-to-close-an-lsv-collection.md)   
 [Registrare pagamenti LSV+](how-to-post-lsv-payments.md)   
 [Esportare pagamenti tramite LSV](how-to-export-payments-using-lsv.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
