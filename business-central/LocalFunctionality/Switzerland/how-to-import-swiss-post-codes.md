---
title: 'Come importare codici postali svizzeri [CH]'
description: È possibile importare l'ultimo file di codice postale svizzero e utilizzarlo per aggiornare la tabella NPA per definire i numeri postali di avviamento per clienti o fornitori.
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: null
ms.date: 11/14/2023
ms.author: bholtorf
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---
# Importare i codici postali svizzeri nella versione svizzera
È possibile importare l'ultimo file di codice postale e utilizzarlo per aggiornare la tabella **CAP**. Il file di codice postale può essere scaricato dal sito Web dei [codici postali svizzeri](https://go.microsoft.com/fwlink/?LinkId=150292). Dopo l'importazione del codice postale più recente, è possibile definire i codici postali per i clienti o i fornitori. Per ulteriori informazioni, vedere [Registrare nuovi fornitori](../../purchasing-how-register-new-vendors.md).  

## Per importare i codici postali  

1.  Scegliere la ![lampadina che apre la funzionalità delle informazioni.](../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immettere **NPA**, quindi selezionare il collegamento correlato.  
2.  Selezionare l'azione **Importa codici postali**.  
3.  Nella pagina **Importa codici postali** nel campo **Nome file** immettere il nome del file di codice postale da importare nella tabella **CAP**.  
4.  Scegliere il pulsante **OK**.  

    Le informazioni più recenti sui codici postali vengono importate.  

Di seguito viene descritto come definire i codici postali per i clienti, ma gli stessi passaggi si applicano anche per definire i codici postali per i fornitori.  

## Per definire i codici postali per i clienti  

1.  Scegliere la ![lampadina che apre la funzionalità delle informazioni.](../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immettere **Clienti**, quindi selezionare il collegamento correlato.  
2.  Selezionare il cliente per cui definire un codice postale, quindi scegliere l'azione **Modifica**.  
3.  Nella Scheda dettaglio **Generale** della pagina **Scheda cliente**, nel campo **CAP** selezionare il codice postale per l'indirizzo del cliente.  

    > [!NOTE]  
    >  Una volta selezionato il codice postale, i campi **Città** e **Codice paese** vengono popolati automaticamente con le informazioni della tabella **CAP**. Per ulteriori informazioni, vedere [Registrare nuovi clienti](../../sales-how-register-new-customers.md).  

4.  Scegliere il pulsante **OK**.  

## Vedere anche   
 [Documenti di acquisto e di vendita per la Svizzera](swiss-purchase-documents-and-sales-documents.md)   
 [Stampare una lista prelievi magazzino da un ordine di vendita](how-to-print-an-inventory-picking-list-from-a-sales-order.md)   
 [Registrare nuovi fornitori](../../purchasing-how-register-new-vendors.md)  


[!INCLUDE[footer-include](../../includes/footer-banner.md)]