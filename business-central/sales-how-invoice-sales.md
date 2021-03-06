---
title: Fatturare le vendite
description: Descrive come creare un fattura di vendita o un ordine di vendita per registrare l'accordo con un cliente per vendere prodotti secondo termini specifici.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: bill, sale, invoice, order
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: d0a48037123dee4a7c9282432cc2b357b335e794
ms.sourcegitcommit: f9a190933eadf4608f591e2f1b04c69f1e5c0dc7
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 05/28/2021
ms.locfileid: "6115583"
---
# <a name="invoice-sales"></a>Fatturare le vendite

Si crea una fattura di vendita o un ordine di vendita per registrare il contratto con un cliente per vendere alcuni prodotti con determinate condizioni di consegna e pagamento.  

In un paio di scenari è necessario utilizzare un ordine di vendita invece di una fattura di vendita:  

* Se è necessario spedire solo una parte della quantità degli ordini, ad esempio, perché la quantità completa non è disponibile.  
* Se si spediscono i prodotti dopo aver registrato le fatture di vendita corrispondenti.
* Se si vendono articoli che il fornitore consegna direttamente al cliente. Questa operazione viene denominata spedizione diretta. Per ulteriori informazioni, vedere [Effettuare spedizioni dirette](sales-how-drop-shipment.md).  

In tutti gli altri scenari, gli ordini di vendita e le fatture di vendita funzionano nello stesso modo. Per ulteriori informazioni, vedere [Vendere prodotti](sales-how-sell-products.md).

È possibile negoziare con il cliente prima di tutto creando un'offerta di vendita, che è possibile convertire in una fattura di vendita quando ci si accorda sulla vendita. Per ulteriori informazioni, vedere [Creare offerte di vendita](sales-how-make-offers.md).

## <a name="create-sales-invoices"></a>Crea fatture di vendita

Se il cliente decide di acquistare, registrare la fattura di vendita per creare i relativi movimenti di quantità e valore. Quando si registra la fattura di vendita, è possibile inviare via email il documento come allegato PDF. È possibile impostare il messaggio con un testo precompilato che riepiloga le informazioni della fattura e per il pagamento, ad esempio con un collegamento a PayPal. Per ulteriori informazioni, vedere [Inviare documenti via e-mail](ui-how-send-documents-email.md). Quando un cliente paga quindi la fattura, è possibile registrare il pagamento in diversi modi, a seconda della dimensione e dei flussi di lavoro preferiti dell'organizzazione. Per ulteriori informazioni, vedere la sezione [Registrazione dei pagamenti](#registering-payments).  

Le schede articolo possono essere di tipo **Inventario**, **Assistenza** e **Non in inventario** per specificare se l'articolo rappresenta un'unità fisica di inventario, un'unità di misura del tempo della manodopera o un'unità fisica non gestita in magazzino. Per ulteriori informazioni, vedere [Registrare nuovi articoli](inventory-how-register-new-items.md). Il processo della fattura di vendita è lo stesso per tutti e tre i tipi di articoli.

È possibile compilare i campi cliente nella fattura di vendita in due modi a seconda che il cliente sia già registrato o meno. Vedere il passaggio 2 della procedura riportata di seguito.

### <a name="to-create-a-sales-invoice"></a>Per creare una fattura di vendita

1. Scegliere l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immettere **Fatture vendite** e quindi scegliere il collegamento correlato.  
2. Nel campo **Cliente** immettere il nome di un cliente esistente.

   Altri campi nella pagina **Fattura di vendita** contengono informazioni standard sul cliente selezionato. Se il cliente non è registrato, è necessario attenersi alla seguente procedura:

    1. Nel campo **Cliente** immettere il nome del nuovo cliente.
    2. Nella finestra di dialogo relativa alla registrazione del nuovo cliente fare clic su **Sì**.
    3. Nella pagina **Selezionare un modello per un nuovo cliente** scegliere un modello su cui basare la scheda del nuovo cliente, quindi scegliere **OK**.
    4. Una nuova scheda cliente verrà visualizzata con le informazioni sul modello cliente selezionato. Compilare i campi rimanenti. Per ulteriori informazioni, vedere [Registrare nuovi clienti](sales-how-register-new-customers.md).  
    5. Una volta completata la scheda cliente, scegliere **OK** per tornare alla pagina **Fattura di vendita**.

   Diversi campi nella fattura di vendita sono ora compilati con le informazioni specificate nella nuova scheda cliente.  
3. Compilare i restanti campi della pagina **Fattura di vendita** in base alle proprie esigenze. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    > [!NOTE]  
    > Se si consente al cliente di pagare immediatamente, ad esempio, in contanti o tramite PayPal, compilare il campo **Codice metodo di pagamento**. Il pagamento viene quindi registrato non appena si registra la fattura di vendita. Se si seleziona CASSA, il pagamento viene registrato in un conto di contropartita specificato.

    È ora possibile compilare le righe della fattura di vendita per i prodotti che si sta vendendo al cliente o per ogni transazione con il cliente per il quale si desidera effettuare la registrazione in un conto C/G.  

    Se sono state impostate le righe di vendita periodiche per il cliente, ad esempio un ordine di rifornimento mensile, è possibile inserire queste righe nell'ordine scegliendo l'azione **Ottieni righe di vendita ricorrenti**.  
4. Nella Scheda dettaglio **Righe** nel campo **Tipo** selezionare il tipo di prodotto, addebito o transazione per cui si effettuerà la registrazione per il cliente con la riga di vendita.
5. Nel campo **Nr.** selezionare un record per effettuare la registrazione in base al valore nel campo **Tipo**.

    Lasciare il campo **Nr.** vuoto nei seguenti casi:

    * Se la riga è destinata a un commento. Compilare il commento nel campo **Descrizione**.
    * Se la riga è destinata a un articolo di catalogo. Scegliere l'azione **Seleziona articoli di catalogo**. Per ulteriori informazioni, vedere [Utilizzare gli articoli di catalogo](inventory-how-work-nonstock-items.md).

6. Nel campo **Quantità** immettere qui il numero di unità di articoli, addebiti o transazioni che la riga registrerà per il cliente.  

    > [!NOTE]  
    > Se l'articolo è di tipo **Assistenza** o se il campo **Tipo** contiene **Risorsa**, la quantità è un'unità temporale, ad esempio le ore, come indicato nel campo **Cod. unità di misura** nella riga. Per ulteriori informazioni, vedere [Impostare unità di misura articolo](inventory-how-setup-units-of-measure.md).

    Il valore nel campo **Importo riga** viene calcolato come *Prezzo unitario* x *Quantità*.  

    Il prezzo e gli importi riga sono con o senza le tasse di vendita a seconda della selezione nel campo **Prezzi IVA inclusa** della scheda cliente.  
7. Se si desidera assegnare uno sconto, immettere una percentuale nel campo **% sconto riga**. Il valore nel campo **Importo riga** viene aggiornato di conseguenza.  

    Se sono stati impostati prezzi articolo speciali nella Scheda dettaglio **Prezzi di vendita e sconti riga di vendita** per il cliente o la scheda articolo, la percentuale di sconto riga, il prezzo e l'importo nella riga dei vendita vengono automaticamente aggiornati se vengono soddisfatti i criteri di prezzo concordati. Per ulteriori informazioni, vedere [Registrazione di prezzi, sconti e contratti di pagamento per le vendite](sales-how-record-sales-price-discount-payment-agreements.md).  
8. Ripetere i passaggi da 9 a 12 per ogni prodotto o addebito che si desidera fatturare al cliente.  

    I campi dei totali sotto le righe vengono automaticamente aggiornati quando si creano o si modificano le righe per visualizzare gli importi che verranno registrati nei libri contabili.

    > [!NOTE]
    > In casi molto rari, gli importi registrati possono discostarsi da ciò che viene visualizzato nei campi dei totali. Ciò è in genere dovuto ai calcoli di arrotondamento in relazione all'IVA o all'imposta sulle vendite.<br /><br />Per verificare gli importi che verranno effettivamente registrati, è possibile utilizzare la pagina **Statistiche**, che tiene conto dei calcoli di arrotondamento. Inoltre, se si sceglie l'azione **Rilascia**, i campi dei totali verranno aggiornati per includere i calcoli di arrotondamento.
9. Nel campo **Importo sconto fattura** immettere un importo che deve essere dedotto dal valore indicato nel campo **Totale IVA incl.**.

    Se sono stati impostati degli sconti su fattura per il cliente, il valore percentuale specificato viene automaticamente inserito nel campo **% sconto fattura** se vengono soddisfatti i criteri e l'importo correlato viene inserito nel campo **Importo sconto fatt. IVA esclusa**. Per ulteriori informazioni, vedere [Registrazione di prezzi, sconti e contratti di pagamento per le vendite](sales-how-record-sales-price-discount-payment-agreements.md).  
10. Una volta completate le righe della fattura di vendita, scegliere l'azione **Registra e invia**.  

Viene visualizzata la finestra dialogo **Registra e invia conferma** con il metodo preferito del cliente per la ricezione dei documenti. È possibile modificare il metodo di invio scegliendo il pulsante di ricerca per il campo **Invia documento a**. Per ulteriori informazioni, vedere [Impostare profili di invio documenti](sales-how-setup-document-send-profiles.md).

I movimenti articolo e di contabilità cliente sono ora creati nel sistema e la fattura di vendita è emessa come documento PDF. La fattura di vendita viene rimossa dall'elenco delle fatture di vendita e sostituita con un nuovo documento nell'elenco delle fatture di vendita registrate.  

### <a name="calculating-invoice-discounts-on-sales"></a>Calcolo degli sconti fattura per le vendite

[!INCLUDE [sales-invoice-discounts](includes/sales-invoice-discounts.md)]

## <a name="posted-invoices"></a>Fatture registrate

[!INCLUDE [posted-invoices](includes/posted-invoices.md)]

È possibile correggere o annullare in modo semplice una fattura di vendita registrata prima che venga pagata. Ad esempio, ciò risulta utile se si desidera correggere un errore di digitazione o se il cliente richiede una modifica in anticipo nell'elaborazione dell'ordine. Per ulteriori informazioni, vedere [Correggere o annullare le fatture di vendita non pagate](sales-how-correct-cancel-sales-invoice.md). Se la fattura di vendita registrata è stata pagata, allora sarà necessario creare una nota di credito di vendita per stornare la vendita. Per ulteriori informazioni vedere [Elaborare i resi o gli annullamenti vendite](sales-how-process-sales-returns-cancellations.md).  

[Apri l'elenco **Fatture vendite registrate**](https://businesscentral.dynamics.com/?page=143) in [!INCLUDE [prod_short](includes/prod_short.md)].

## <a name="registering-payments"></a>Registrazione dei pagamenti

In base alle esigenze aziendali, è possibile ottenere pagato e registrare il pagamento in diversi modi: manualmente, in modo automatico e tramite i servizi di pagamento.  

È possibile elaborare i pagamenti direttamente dalla scheda cliente. Utilizzare l'azione **Registra pagamenti clienti** per ottenere una sintesi delle fatture pagate non per tale cliente. Quindi, contrassegnare la fattura come pagata parzialmente o interamente. Questi processi di riconciliazione pagamenti elaborano i pagamenti dei clienti facendo corrispondere gli importi ricevuti sul conto bancario alle relative fatture di vendita non pagate, quindi registrare i pagamenti. Per ulteriori informazioni, vedere [Per riconciliare i pagamenti individualmente](receivables-how-reconcile-customer-payments-list-unpaid-sales-documents.md#to-register-customer-payments-individually).  

Negli ambienti aziendali in cui il cliente paga qualche tempo dopo la consegna, in base al termine di pagamento, una fattura di vendita registrata rimane aperta (non pagata) fino a quando il reparto Contabilità clienti verifica che il pagamento sia stato ricevuto e applica il pagamento alla fattura di vendita pubblicata. Questo può essere fatto manualmente o automaticamente. Per ulteriori informazioni, vedere [Riconciliare i pagamenti clienti con la registrazione incassi o da movimenti contabili clienti](receivables-how-reconcile-payments-auto-application.md) e [Riconciliare i pagamenti utilizzando il collegamento automatico](receivables-how-apply-sales-transactions-manually.md).  

Negli ambienti aziendali in cui il cliente paga immediatamente, ad esempio tramite PayPal o contanti, il pagamento viene registrato immediatamente quando si registra la fattura di vendita, vale a dire la fattura di vendita pubblicata viene chiusa come interamente applicata. Selezionare il metodo rilevante nel campo **Codice metodo di pagamento** nell'ordine cliente. Vedere il passaggio 8. Per i pagamenti elettronici, come PayPal, compilare anche il campo **Servizio di pagamento**. Per ulteriori informazioni, vedere [Abilitare i pagamenti clienti tramite i servizi di pagamento](sales-how-enable-payment-service-extensions.md).  

È persino possibile creare fatture pagate direttamente per clienti non registrati impostando dapprima una scheda "cliente per vendite in contanti", selezionabile nella fattura di vendita. Per ulteriori informazioni, vedere [Impostare i clienti per vendite in contanti](finance-how-to-set-up-cash-customers.md).  

> [!TIP]
> Se si desidera inviare ai clienti solleciti per pagamenti in ritardo, è necessario impostare i livelli e i termini di sollecito. Per ulteriori informazioni, vedere [Impostare i termini e i livelli di sollecito](finance-setup-reminders.md).  

## <a name="external-document-numbers"></a>Numeri di documento esterno

[!INCLUDE [ext-doc-no-sales](includes/ext-doc-no-sales.md)]

## <a name="see-related-training-at-microsoft-learn"></a>Vedere le informazioni relative al training in [Microsoft Learn](/learn/modules/invoicing-customers-dynamics-365-business-central/index)

## <a name="see-also"></a>Vedere anche

[Vendite](sales-manage-sales.md)  
[Setup Vendite](sales-setup-sales.md)  
[Stampare la lista prelievo](sales-how-print-picking-list.md)  
[Magazzino](inventory-manage-inventory.md)  
[Inviare documenti via e-mail](ui-how-send-documents-email.md)  
[Riscuotere i saldi inevasi](receivables-collect-outstanding-balances.md)  
[Eseguire la fatturazione in blocco da Microsoft Bookings in Business Central](finance-bookings.md)  
[Utilizzo di [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]