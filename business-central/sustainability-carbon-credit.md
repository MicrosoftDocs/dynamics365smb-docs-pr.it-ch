---
title: Lavorare con i crediti di carbonio
description: Scopri come impostare e acquistare crediti di carbonio.
author: altotovi
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'Sustainability, ESG, emission, GHG, CSRD, carbon, credit, CO2'
ms.search.form: null
ms.date: 08/20/2024
ms.author: altotovi
ms.service: dynamics-365-business-central
ms.reviewer: solsen
---

# <a name="work-with-carbon-credit"></a>Lavora con il credito di carbonio

Quando le aziende non riescono a ridurre le proprie emissioni per vari motivi, possono acquistare crediti di carbonio per compensarle. Acquistando crediti di carbonio, un'azienda può comunque emettere la stessa quantità di gas mantenendo la neutralità carbonica. Questi crediti vengono acquistati da fornitori specializzati, incentivando la riduzione delle emissioni.  

In generale, i crediti di carbonio sono permessi che consentono al proprietario di emettere una certa quantità di anidride carbonica (CO₂) o altri gas serra (GHG). Un credito di carbonio in genere rappresenta il diritto di emettere una tonnellata di CO₂ o una quantità equivalente di un altro gas serra, quindi è importante abilitare questa opzione per alcune organizzazioni.  

## <a name="set-up-the-carbon-credit"></a>Imposta il credito di carbonio

Il credito di carbonio in [!INCLUDE[prod_short](includes/prod_short.md)] può essere impostato come **elemento**. Per impostare l' **elemento** come credito di carbonio, seguire i passaggi:
  
1. Seleziona l'icona ![lampadina che apre la funzionalità Dimmi](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire"), immetti **Articoli** e seleziona il collegamento correlato. 
2. [Crea un nuovo elemento come spiegato](inventory-how-register-new-items.md).   
3. Una volta creato l'elemento, Seleziona il campo  **Credito GHG** nella scheda rapida  **Sostenibilità** e aggiungi il valore del credito di carbonio utilizzando il campo  **Credito di carbonio per UOM** .

> [!NOTE]
> **Il credito di carbonio per UOM** rappresenta la quantità di CO₂ nell'unità di misura configurata nel **codice dell'unità di misura delle emissioni** nella **impostazione della sostenibilità**. Ciò significa che il valore totale del credito di carbonio è pari alla quantità di CO₂ accreditata per un' **unità di misura di base** articolo utilizzato.  

> [!NOTE]
> È possibile impostare qualsiasi tipo di articolo, che si tratti di inventario, servizio o non inventario, come credito di carbonio.  

## <a name="to-purchase-carbon-credit"></a>Per acquistare crediti di carbonio

### <a name="purchase-documents"></a>Documenti di acquisto

Per lavorare con qualsiasi documento relativo all'acquisto, seguire segui questi passaggi:

1. Seleziona l'icona ![lampadina che apre la funzionalità Dimmi 3.](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") Icona e:  
   1. Inserisci **Fatture di acquisto** se desideri la fattura come **Tipo di documento**, quindi Seleziona il relativo collegare.  
   2. Inserisci **Ordini di acquisto** se vuoi ordinare come **Tipo di documento**, quindi Seleziona il relativo collegare.   
2. Compilare l'intestazione del documento in base alle seguenti istruzioni [su come lavorare con fatture e ordini di acquisto](purchasing-how-record-purchases.md). 
3. Seleziona l'elemento da configurare come credito di carbonio nel  **Numero.** Campo nelle righe del documento di acquisto e aggiungere la **Quantità** e il **Costo unitario diretto** appropriati. 
4. Aggiungi il **numero di conto sostenibilità** che utilizzeresti per ridurre il valore di anidride carbonica (CO₂). Il sistema popolerà automaticamente il valore nel campo  **Emissioni di CO2** in base al valore configurato nel campo  **Credito di carbonio per UOM** sull' **Articolo** scheda.
5. Registrare il documento.

> [!NOTE]
> Sebbene il credito di carbonio diminuisca il valore delle voci, vedrai un valore positivo nella colonna  **Emissione CO2**. Ma una volta pubblicato il documento, vedrai un valore con un registro negativo nella  **Voce del registro sostenibilità** con il  **Credito GHG** come  **Tipo di documento**.  

### <a name="sustainability-journals"></a>Giornali di registrazione della sostenibilità

Per lavorare con  **Sustainability Journal** seguire i passaggi sono:  

1. Seleziona l'icona ![lampadina che apre la funzionalità Dimmi 3.](media/ui-search/search_small.png "Dimmi cosa vuoi fare") immetti **Registrazione sostenibilità**, quindi seleziona il collegamento correlato. 
2. Nella pagina  **Giornale della sostenibilità**, inserisci tutte le righe che intendi pubblicare nello stesso batch.  
3. Selezionare il **Credito GHG** nel campo **Tipo di documento** .    
4. Nel campo **Nr. conto** puoi selezionare solo i conti di sostenibilità non bloccati dove il campo **Registrazione diretta** è selezionato e il campo **Tipo di contabilità** è impostato su **Registrazione**. I conti devono inoltre essere configurati con una categoria e una sottocategoria. Selezionare l'account appropriato per registrare i crediti di carbonio.
5. Seleziona **Inserimento manuale** e inserisci il valore che vuoi pubblicare come credito di carbonio nel campo **Emissioni CO2** .  
6. Effettuare la registrazione.   

## <a name="see-also"></a>Vedere anche

[Finanze](finance.md)    
[Registrare movimenti di sostenibilità](finance-sustainability-journal.md)    
[Panoramica della gestione della sostenibilità](finance-manage-sustainability.md)    
[Setup sostenibilità](finance-sustainability-setup.md)   
[Contabilità generale e piano dei conti di sostenibilità](finance-sustainability-accounts-ledger.md)  
[Analisi ad hoc dei dati di sostenibilità](ad-hoc-analysis-sustainability.md)    
[Rapporti e analisi sulla sostenibilità in [!INCLUDE[prod_short](includes/prod_short.md)]](sustainability-reports.md)   
[API per la sostenibilità](/dynamics365/business-central/dev-itpro/api-sustainability/sustainability-api?toc=/dynamics365/business-central/toc.json)    
[Utilizzare [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)    

[!INCLUDE[footer-include](includes/footer-banner.md)]
