---
title: Risoluzione dei problemi di sincronizzazione tra Shopify e Business Central
description: Scopri cosa fare in caso di errore durante la sincronizzazione dei dati tra Shopify e Business Central
ms.date: 08/19/2022
ms.topic: article
ms.service: dynamics365-business-central
ms.search.form: 30118, 30119, 30120,
author: edupont04
ms.author: andreipa
ms.reviewer: solsen
ms.openlocfilehash: 47b0d72283b4d017bb522c3e71f6c61501b59d5b
ms.sourcegitcommit: 38b1272947f64a473de910fe81ad97db5213e6c3
ms.translationtype: HT
ms.contentlocale: it-CH
ms.lasthandoff: 08/29/2022
ms.locfileid: "9361960"
---
# <a name="troubleshooting-shopify-and-business-central-synchronization"></a>Risoluzione dei problemi di sincronizzazione tra Shopify e Business Central

È possibile imbattersi in situazioni in cui è necessario risolvere i problemi quando si sincronizzano i dati tra Shopify e [!INCLUDE[prod_short](../includes/prod_short.md)]. Questa pagina definisce i passaggi per la risoluzione dei problemi di alcuni scenari comuni che potrebbero verificarsi.

## <a name="logs"></a>Log

Se un'attività di sincronizzazione non riesce, è possibile attivare la registrazione attivando **Abilita registro** nella pagina **Scheda punto vendita Shopify**. Quindi attiva manualmente l'attività di sincronizzazione e rivedi i log.

1. Scegli l'icona a forma di ![lampadina che apre la funzione Dimmi 1.](../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") icona, immetti **Movimenti di registri Shopify**, quindi scegli il collegamento correlato.
2. Seleziona la voce di registro correlata e apri la pagina **Voce di registro Shopify**.
3. Esamina la richiesta, il codice di stato e la descrizione e i valori di risposta.

Quindi ricordati di disattivare la registrazione per evitare un impatto negativo sulle prestazioni e aumentare le dimensioni del database.

Dalla pagina **Voci di registro Shopify**, è possibile attivare l'eliminazione di tutte le voci di registro o di quelle più vecchie di sette giorni.

## <a name="data-capture"></a>Acquisizione dati

Indipendentemente dalle impostazioni **Log attivato** alcune risposte da Shopify vengono sempre registrate in modo da poterle esaminare o scaricare tramite la pagina **Lista acquisizione dati**.

Scegli l'azione **Dati Shopify recuperati** in una delle seguenti pagine:

- **Ordine Shopify**
- **Evasioni ordini Shopify**
- **Costi di spedizione ordine Shopify**
- **Transazioni ordine Shopify**
- **Pagamenti Shopify**
- **Transazioni di pagamento Shopify**
- **Transazioni Shopify**

## <a name="reset-sync"></a>Reimposta sincronizzazione

Per prestazioni ottimali, il connettore importa solo clienti, prodotti e ordini creati o modificati dall'ultima sincronizzazione. Nella pagina **Scheda punto vendita Shopify**, sono disponibili funzioni per modificare la data/ora dell'ultima sincronizzazione o ripristinarla completamente. Questa funzione garantisce che quando viene eseguita la sincronizzazione, tutti i dati vengano sincronizzati e non solo le modifiche dall'ultima sincronizzazione.

Questa funzione si applica solo alle sincronizzazioni da Shopify a [!INCLUDE[prod_short](../includes/prod_short.md)]. Può essere utile se è necessario ripristinare i dati eliminati come prodotti, clienti o ordini eliminati.

## <a name="request-the-access-token"></a>Richiedere il token di accesso

Se [!INCLUDE[prod_short](../includes/prod_short.md)] non si connette al tuo account Shopify, prova a richiedere il token di accesso da Shopify. Questa richiesta potrebbe essere necessaria in caso di rotazione delle chiavi di sicurezza o modifiche alle autorizzazioni (ambito) richieste.

1. Scegli l'icona a forma di ![lampadina che apre la funzione Dimmi 1.](../media/ui-search/search_small.png "Dimmi cosa vuoi fare") e immetti **Punti vendita Shopify**, quindi scegli il collegamento correlato.
2. Seleziona il punto vendita per il quale desideri recuperare il token di accesso per l'apertura della pagina **Scheda del punto vendita Shopify**.
3. Scegli l'azione **Richiedi accesso**.
4. Se richiesto, accedi al tuo account Shopify.

L'interruttore **Con chiave di accesso** verrà attivato.

### <a name="verify-and-enable-permissions-to-make-http-requests-when-running-in-a-non-production-environment"></a>Verifica e abilita le autorizzazioni per effettuare richieste http durante l'esecuzione in un ambiente non di produzione

Per funzionare correttamente, l'estensione connettore Shopify richiede l'autorizzazione per effettuare richieste http. Durante il test nel sandbox, le richieste http sono vietate per tutte le estensioni.

1. Scegli l'icona a forma di ![lampadina che apre la funzione Dimmi 1](../media/ui-search/search_small.png "Dimmi cosa vuoi fare") e immetti **Gestione estensioni**, quindi scegli il collegamento correlato.
2. Seleziona l'estensione *Connettore Shopify*.
3. Scegli l'azione **Configura** per aprire la pagina **Impostazione estensione**.
4. Assicurati che l'interruttore **Consenti richieste HTTPClient** sia abilitato.

## <a name="rotate-the-shopify-access-token"></a>Ruotare il token di accesso Shopify

Le procedure seguenti descrivono come ruotare il token di accesso utilizzato dal connettore Shopify per accedere al tuo punto vendita Shopify online.

### <a name="in-shopify"></a>In Shopify

1. Da **Amministratore Shopify**, vai ad [App](https://www.shopify.com/admin/apps).
2. Seleziona **Elimina** nella riga con l'app **Dynamics 365 Business Central**.
3. Nel messaggio che viene visualizzato, seleziona **Elimina**.

### <a name="in-prod_short"></a>In [!INCLUDE[prod_short](../includes/prod_short.md)]

1. Scegli l'icona a forma di ![lampadina che apre la funzione Dimmi 1](../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") e immetti **Punti vendita Shopify**, quindi scegli il collegamento correlato.
2. Seleziona il punto vendita per il quale desideri ruotare il token di accesso per l'apertura della pagina **Scheda del punto vendita Shopify**.
3. Scegli l'azione **Richiedi accesso**.
4. Se richiesto, accedi al tuo account Shopify, rivedi privacy e autorizzazioni, quindi scegli il pulsante **Installa app**.

## <a name="known-issues"></a>Problemi noti

Il campo *Cat. Reg. Business* non può essere zero o vuoto; deve esserci un valore nel campo del cliente. Per correggere:

Nella pagina **Scheda punto vendita Shopify** compila il campo **Codice modello cliente** con il modello che include il campo **Categoria registrazione business** popolato. Il modello cliente viene utilizzato non solo per la creazione di clienti, ma anche per il calcolo del prezzo di vendita e durante la creazione di documenti di vendita.

### <a name="importing-data-to-your-shopify-shop-isnt-enabled-go-to-the-shop-card-to-enable-it"></a>L'importazione dei dati nel negozio Shopify non è abilitata. Vai alla scheda del punto vendita per abilitarla

Nella finestra **Scheda punto vendita Shopify**, abilitare l'interruttore **Consenti sincronizzazione dati in Shopify**.  Questo interruttore ha lo scopo di proteggere il punto vendita online dall'ottenere dati dimostrativi da [!INCLUDE[prod_short](../includes/prod_short.md)].

## <a name="see-also"></a>Vedere anche

[Iniziare a utilizzare il connettore per Shopify](get-started.md)