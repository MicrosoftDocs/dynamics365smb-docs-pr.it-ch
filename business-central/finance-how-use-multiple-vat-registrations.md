---
title: Numeri di registrazione IVA multipli
description: Scopri di più sulla funzionalità dei numeri di registrazione IVA (alternativi) multipli.
author: altotovi
ms.topic: conceptual
ms.reviewer: null
ms.search.keywords: 'VAT, multiple, alternative, customer, tax, value-added tax'
ms.search.form: '212, 301,'
ms.date: 08/21/2024
ms.author: altotovi
ms.service: dynamics-365-business-central
---

# <a name="multiple-vat-registration-numbers"></a>Numeri di registrazione IVA multipli

Per le aziende con magazzini in più paesi dell'UE, la gestione dell'IVA (imposta sul valore aggiunto) può essere complicata, poiché ogni magazzino richiede un numero di partita IVA diverso per rispettare le normative specifiche di ciascun paese. Il presente articolo fornisce informazioni su questo requisito e spiega la funzionalità per più numeri di registrazione IVA. Questa funzionalità consente agli utenti di impostare i numeri di registrazione fiscale per i propri clienti in diversi paesi/regioni.  

> [!NOTE]
> La funzionalità *Numeri IVA multipli per i clienti* è disponibile solo da Business Central 2024 ciclo di rilascio 2 (versione 25).

## <a name="how-to-set-up-the-alternative-vat-registration-numbers"></a>Come impostare i numeri di registrazione IVA alternativi

Per impostare numeri di registrazione IVA alternativi per diversi paesi/regioni, seguire segui questi passaggi: 

1. Seleziona l'icona ![lampadina che apre la funzionalità Dimmi](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), Icona, immettere **Registrazione IVA cliente alternativa**, quindi Seleziona il relativo collegare. 
2. Aggiungere il cliente nel campo  **Numero cliente** e il paese/regione correlato a questa registrazione IVA nel campo  **Codice paese/regione IVA**.  
3. È necessario aggiungere il numero di partita IVA nel campo **Numero di registrazione IVA** . Quando si utilizza il  **codice Paese/Regione**, è necessario attenersi al formato. 
4. Se si desidera utilizzare gruppi di registrazione IVA o generali diversi, è possibile aggiungerli in alternativa alla configurazione nei campi  **Gruppo di registrazione IVA Bus** e  **Gruppo di registrazione Bus generale** . 
5. Chiudere la pagina.   

Per creare un indirizzo alternativo per il tuo cliente, seguire segui questi passaggi:  

1. Apri il **Cliente** scheda per il cliente a cui vuoi aggiungere un nuovo **Indirizzo di spedizione**. 
2. Seleziona **Cliente** e scegli l'azione **Indirizzi di spedizione** .   
3. Si apre la pagina  **Elenco indirizzi di spedizione**, seleziona  **Nuovo**. 
4. Inserisci le informazioni sulla destinazione della spedizione del tuo cliente.  
5. Selezionare il **codice Paese/Regione** corretto.   
6. Se hai già configurato un nuovo **numero di registrazione IVA** sulla **registrazione IVA alternativa del cliente** per questo paese o questa regione, non accadrà nulla. 
7. Tuttavia, se non hai configurato in precedenza il **numero di registrazione IVA** nella **registrazione IVA alternativa del cliente** per questo paese o regione, verrà visualizzata la seguente notifica: **Fai clic su Aggiungi se desideri inserire la registrazione IVA alternativa per questo codice paese di spedizione.** 
8. Apparirà una notifica che ti avvisa che dovresti aggiungere un nuovo numero di partita IVA. Per farlo, è necessario selezionare l'azione  **Aggiungi** nella notifica e si aprirà la pagina  **Registrazione IVA alternativa del cliente** . 
9. Questa pagina compila il tuo **numero cliente.** E il **codice Paese/Regione IVA**. Quindi, devi solo aggiungere la configurazione che desideri utilizzare. 

## <a name="work-with-the-sales-documents"></a>Lavorare con i documenti di vendita

È possibile creare una nuova [fattura di vendita](sales-how-invoice-sales.md) o [ordine di vendita](sales-how-sell-products.md) in [!INCLUDE[prod_short](includes/prod_short.md)]. Se devi utilizzare un indirizzo di spedizione diverso dall'indirizzo del cliente e situato in un paese diverso, seguire i passaggi:  

### <a name="alternate-shipping-address"></a>Indirizzo di spedizione alternativo

1. Espandi la scheda rapida  **Spedizione e fatturazione** .   
2. Nel campo Spedisci a, seleziona l'opzione  **Indirizzo di spedizione alternativo** . 
3. Viene visualizzata la pagina  **Elenco indirizzi di spedizione** con gli indirizzi alternativi disponibili. 
4. Scegli uno degli indirizzi con un diverso **codice Paese/Regione**. 
5. Viene visualizzata la pagina di dialogo  **Conferma registrazione IVA cliente alternativo** con un elenco di campi modificati a causa della modifica della configurazione  **Registrazione IVA cliente alternativo** . 
6. Seleziona **OK** per confermare.   

> [!NOTE]
> Se non vuoi più confermare tale scelta, puoi Seleziona il campo **Non mostrare più** e in futuro non vedrai più questo tipo di notifica sulle modifiche. Ma se vuoi abilitarlo di nuovo, puoi farlo abilitando il campo  **Conferma registrazione IVA alternativa** in  **Impostazione IVA**.  
   
7. Una volta confermati, i valori vengono sovrascritti con i valori della configurazione della  **Registrazione IVA cliente alternativa** . Puoi controllare tutti i campi relativi all'IVA che si trovano nella scheda rapida  **Dettagli fattura** .  
8. Registrare il documento.  

### <a name="custom-address"></a>Indirizzo personalizzato

Se non hai configurato l'indirizzo di spedizione ma vuoi comunque utilizzare un indirizzo diverso per la spedizione, puoi usare questa opzione.  

1. Espandi la scheda rapida  **Spedizione e fatturazione** .   
2. Nel campo Spedisci a, seleziona l'opzione  **Indirizzo personalizzato** .  
3. Cambia il Paese nel campo  **Paese/Regione** .  
4. Dopo aver modificato il codice paese/regione in modo che corrisponda al **codice paese/regione IVA** della **registrazione IVA alternativa del cliente**, viene visualizzata la pagina di dialogo **Conferma registrazione IVA alternativa del cliente** con un elenco dei campi modificati. 
5. [!INCLUDE[prod_short](includes/prod_short.md)] modificherà anche tutti i campi relativi all'IVA che si trovano nella scheda rapida  **Dettagli fattura** .  

### <a name="work-with-no-shipment"></a>Lavora senza spedizione

Se non è prevista alcuna spedizione come processo, puoi comunque sfruttare la configurazione della  **Registrazione IVA alternativa per il cliente** .

Nell'ordine di vendita o nella fattura puoi trovare il **Codice Paese/Regione IVA** nella scheda rapida **Dettagli fattura** e specificare il valore che corrisponde alla configurazione **Registrazione IVA cliente alternativa** . Dovresti visualizzare la stessa pagina di dialogo di conferma di cui sopra. 

In questa situazione puoi registrare la fattura di vendita con il numero di partita IVA corretto per il tuo cliente anche se non spedisci articoli con questo documento. **·**  

### <a name="work-with-the-sales-credit-memo"></a>Lavorare con la nota di accredito delle vendite

Una volta registrata la fattura con un **Indirizzo di spedizione** o **Codice Paese/Regione IVA** con dati di registrazione diversi, la **Nota di accredito vendita** correttiva prende i valori dall'intestazione **Fattura di vendita registrata** dove questi valori vengono presi dalla **Registrazione IVA alternativa del cliente**, quindi non sono necessarie altre azioni. 

## <a name="see-also"></a>Vedere anche

[Panoramica sulla gestione dell'IVA](finance-manage-vat.md)    
[Impostare l'imposta sul valore aggiunto](finance-setup-vat.md)    
[Utilizzare l'IVA nelle vendite e negli acquisti](finance-work-with-vat.md)    
[Segnalare l'IVA all'autorità fiscale](finance-how-report-vat.md)    
[Funzionalità locale in Business Central](about-localization.md)    


[!INCLUDE[footer-include](includes/footer-banner.md)]
