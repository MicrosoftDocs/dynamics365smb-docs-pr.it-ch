---
title: Registrare e rimborsare le spese dei dipendenti
description: Registra le spese di un dipendente con le registrazioni COGE nel conto del dipendente e successivamente registra un pagamento verso il conto bancario per rimborsare le spese sostenute per il lavoro.
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: reimbursement
ms.search.form: '63, 234, 625, 5224, 5237, 5238, 5239, 5240'
ms.date: 03/13/2024
ms.author: bholtorf
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---
# <a name="record-and-reimburse-employees-expenses"></a>Registrare e rimborsare le spese dei dipendenti

[!INCLUDE[prod_short](includes/prod_short.md)] supporta le transazioni per i dipendenti in modo simile alle transazioni per i fornitori. Di conseguenza, sono disponibili alcune categorie di registrazione dipendenti che consentono di assicurarsi che i movimenti contabili per i dipendenti siano registrati nei conti di pertinenza nella contabilità COGE.

> [!NOTE]  
> I rimborsi ai dipendenti non supportano sconti e e tolleranze sui pagamenti.

Se i dipendenti spendono denaro personale durante le attività lavorative, è possibile registrare le spese nei conti dei dipendenti. È quindi possibile rimborsare il dipendente effettuando un pagamento sul conto bancario del dipendente, analogamente a quando si pagano i fornitori.  

Questo articolo spiega come registrare le spese nei libri e come rimborsare il dipendente. L'organizzazione potrebbe avere un portale o un'app in cui i dipendenti possono inviare le proprie note spese.

[!INCLUDE [prod_short](includes/prod_short.md)] è sufficientemente flessibile per adattarsi a molte pratiche diverse. I numeri di account esatti da utilizzare dipendono dalla configurazione e dai processi dell'organizzazione.  

È possibile utilizzare le registrazioni generali dei conti dei dipendenti per registrare le spese dei dipendenti e le transazioni di rimborso in valuta estera, quindi tenere facilmente traccia degli importi e confrontarli con le entrate. Lascia la calcolatrice nel cassetto della scrivania: Business Central può modificare il tasso di cambio per te. Quando utilizzi le registrazioni generali per registrare le transazioni per i conti dei dipendenti, ad esempio rimborsi le spese, puoi utilizzare il campo **Codice valuta** per specificare la valuta per le transazioni. La specifica di una valuta ti consente di utilizzare le stesse funzionalità di quando registri le transazioni nei registri clienti e fornitori. Ad esempio, i dipendenti possono registrare una spesa in euro ma essere pagati in dollari.

Per garantire che il tasso di cambio degli importi sia aggiornato, puoi rettificare i saldi dei dipendenti quando esegui il processo batch del tasso di cambio valuta. Se desideri utilizzare la tabella dei tassi di cambio, ma liquidare i saldi dei dipendenti nella valuta locale, puoi escludere i conti dei dipendenti quando rettifichi i tassi di cambio.

## <a name="to-record-an-employees-expense"></a>Per registrare le spese di un dipendente

Le spese del dipendente vengono registrate nella pagina **Contabilità generale**.

1. Scegli la ![lampadina che apre la funzione Dimmi.](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immetti **Registrazioni COGE**, quindi scegli il collegamento correlato.  
2. Aprire il batch registrazioni COGE appropriato. Per ulteriori informazioni, vedere [Elaborazione delle registrazioni COGE](ui-work-general-journals.md).
3. In una nuova riga di registrazione, compilare i campi in base alle esigenze. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

    > [!NOTE]
    > [!INCLUDE[journal-showhide-columns-inline-tip](includes/journal-showhide-columns-inline-tip.md)]
4. Ripetere il passaggio 3 per le spese che il dipendente ha pagato.

    > [!TIP]  
    > Se si desidera immettere più righe di spesa sopra una riga di contropartita per il conto bancario del dipendente, selezionare la casella di controllo **Suggerisci importo contropartita** nella riga del batch nella pagina **Batch registrazioni COGE**. Il campo **Importo** nella riga di contropartita viene precompilato automaticamente con il valore necessario per pareggiare le spese.
5. Scegliere l'azione **Registra** per registrare spese nel conto del dipendente.

## <a name="to-reimburse-an-employee"></a>Per rimborsare un dipendente

I dipendenti vengono rimborsati registrando i pagamenti nei relativi conti bancari nella pagina **Registrazioni pagamenti**.  

1. Scegli la ![lampadina che apre la funzione Dimmi.](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immetti **Registrazioni pagamenti**, quindi scegli il collegamento correlato.
2. Aprire il batch registrazioni pagamenti appropriato. Per ulteriori informazioni, vedere [Elaborazione delle registrazioni COGE](ui-work-general-journals.md).
3. Compilare i campi in base alle esigenze. Per ulteriori informazioni, vedere [Effettuare i pagamenti](payables-make-payments.md).
4. In alternativa, scegliere l'azione **Suggerisci pagamenti dipendente** per inserire automaticamente righe di registrazione per rimborsi in sospeso al dipendente.
5. Scegliere l'azione **Registra** per registrare il rimborso.  

## <a name="to-reconcile-reimbursements-with-employee-ledger-entries"></a>Per riconciliare i rimborsi con movimenti contabili del dipendente

I pagamenti dei dipendenti si applicano ai movimenti contabili aperti correlati come si fa per i pagamenti dei fornitori, ad esempio nella pagina **Registrazione riconciliazione pagamenti**, in base ai movimenti relativi dell'estratto conto. Per ulteriori informazioni, vedere [Collegare i pagamenti automaticamente e riconciliare i conti correnti bancari](receivables-apply-payments-auto-reconcile-bank-accounts.md). In alternativa, è possibile applicarli manualmente nella pagina **Movimenti contabili dipendente**. Per ulteriori informazioni, vedere [Riconciliare manualmente i pagamenti ai fornitori con la registrazioni pagamenti o dai movimenti contabili fornitori](payables-how-apply-purchase-transactions-manually.md).  

## <a name="see-also"></a>Vedere anche

[Registrare le transazioni direttamente nella contabilità generale](finance-how-post-transactions-directly.md)  
[Usare le registrazioni COGE](ui-work-general-journals.md)  
[Stornare le registrazioni e annullare carichi/spedizioni errati.](finance-how-reverse-journal-posting.md)  
[Finanze](finance.md)  
[Utilizzare [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
