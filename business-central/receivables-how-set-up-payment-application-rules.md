---
title: Regole per il collegamento automatico dei pagamenti
description: Leggi come impostare le regole per il collegamento automatico dei pagamenti nella pagina Regole di collegamento pagamenti.
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'payment process, direct payment posting, reconcile payment, expenses, cash receipts'
ms.search.form: '1290, 1294, 1287'
ms.date: 06/25/2021
ms.author: bholtorf
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---
# Impostare le regole per il collegamento automatico dei pagamenti

Nella pagina **Regole di collegamento pagamenti**, si impostano le regole per stabilire in che modo il testo del pagamento (in una transazione bancaria) viene collegato automaticamente al testo sulle relative fatture aperte (non pagate), note di credito o altre voci quando viene utilizzata la funzione **Applica automaticamente** nella pagina **Registrazione riconciliazione pagamenti**. Per ulteriori informazioni, vedere [Riconciliare i pagamenti utilizzando il collegamento automatico](receivables-how-reconcile-payments-auto-application.md).

Impostare una nuova regola di collegamento dei pagamenti scegliendo quali tipi di dati presenti in una riga di registrazione riconciliazione pagamenti devono corrispondere ai dati di uno o più movimenti aperti prima che il pagamento correlato venga collegato automaticamente ai movimenti aperti. La qualità di ogni collegamento automatico in base alle regole di collegamento viene visualizzata come valore da **Basso** ad **Alto** nel campo **Affidabilità corrispondenza** della pagina **Registrazione riconciliazione pagamenti** in base alla regola di collegamento del pagamento utilizzata.

Ogni riga della pagina **Regole di collegamento pagamenti** rappresenta una regola per il collegamento del pagamento. Le regole si collegano nell'ordine specificato dal campo **Ordinamento**. Se vengono utilizzate più regole contemporaneamente, viene utilizzata la regola con affidabilità di corrispondenza più alta.

La funzione di collegamento automatico è basata sui criteri di corrispondenza prioritaria. In primo luogo la funzione prova, seguendo un ordine di priorità, ad associare il testo nei cinque campi **Parte correlata** in una riga di registrazione con testo in conto corrente bancario, nome o indirizzo dei clienti o fornitori con i documenti non pagati che rappresentano movimenti aperti. Quindi, la funzione tenta di far corrispondere il testo nei campi **Testo transazione** e **Informazioni transazione aggiuntive** in una riga di registrazione con il testo nei campi **Nr. documento esterno** e **Nr. documento** di movimenti aperti. Infine, la funzione prova ad associare l'importo presente nel campo **Importo estratto conto** di una riga di registrazione con l'importo nei movimenti aperti.

> [!NOTE]
> La corrispondenza del testo è possibile solo per il testo più lungo di quattro caratteri.

Oltre ai criteri di corrispondenza, il segno dell'importo del pagamento dipende da quanto riportato di seguito:

- Per gli importi negativi, viene creata una corrispondenza innanzitutto con i movimenti aperti che rappresentano le fatture cliente e poi con le note di credito fornitore.
- Per gli importi positivi, viene creata una corrispondenza innanzitutto con i movimenti aperti che rappresentano le fatture fornitore e poi con le note di credito cliente.

## Per impostare una regola di collegamento del pagamento
1. Scegli la ![lampadina che apre la funzione Dimmi.](media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immetti **Regole di collegamento pagamenti**, quindi seleziona il collegamento correlato.
2. Definire una regola dell'applicazione di pagamento nuova o modificata compilando i campi di una riga come descritto nella tabella.

|Campo|Descrizione|
|-|-|
|**Affidabilità corrispondenza**|Specifica l'affidabilità della regola di applicazione definita nella riga. <br /></br>Un valore specificato in questo campo viene visualizzato nel campo **Affidabilità corrispondenza** nella pagina **Registrazione riconciliazione pagamenti** in base alla qualità del collegamento automatico di pagamento nella riga di registrazione.|
|**Priorità**|Specifica la priorità della regola di collegamento relativa alle altre regole di collegamento definite come righe nella pagina **Regole di collegamento pagamenti**. 1 rappresenta la priorità più alta.|
|**Parte correlata corrispondente**|Specifica quante informazioni sul cliente o fornitore, ad esempio indirizzo, città e il numero di conto corrente bancario, nella riga di registrazione della riconciliazione di pagamento devono corrispondere alle informazioni sul movimento aperto prima che la regola di collegamento venga utilizzata per collegare automaticamente il pagamento al movimento aperto.|
|**Nr. doc./nr. doc. est. corrispondente**|Specifica se il testo nella riga di registrazione riconciliazione pagamenti deve corrispondere al valore nel campo **Nr. documento** o nel campo **Nr. documento esterno** nel movimento aperto prima che venga utilizzata la regola di collegamento per collegare automaticamente il pagamento al movimento aperto.|
|**Importo incl. tolleranza corrispondente**|Specifica quanti movimenti per un cliente o fornitore devono corrispondere all'importo, compresa la tolleranza pagamento, prima che la regola di collegamento sia utilizzata per collegare automaticamente un pagamento al movimento aperto.|
|**Revisione necessaria**|Specifica se il collegamento dei pagamenti automatico è consigliato per la revisione manuale da parte dell'utente prima della registrazione. Scegliendo il campo **Righe per la revisione** nella pagina **Registrazione collegamenti pagamenti**, viene avviata un'esperienza guidata durante la quale è possibile rivedere con facilità più collegamenti in sequenza nella pagina **Revisione collegamento del pagamento**.|

La tabella seguente descrive le regole di collegamento dei pagamenti standard in [!INCLUDE[prod_short](includes/prod_short.md)].

> [!Important]
> Le regole di collegamento dei pagamenti possono essere diverse nella propria installazione di [!INCLUDE[prod_short](includes/prod_short.md)].

| Affidabilità corrispondenza | Priorità | Parte correlata corrispondente | Nr. doc./nr. doc. est. Corrispondente | Importo incl. tolleranza corrispondente |
|------------------|----------|-----------------------|--------------------------------|--------------------------------|
| Alta             | 1        | Completamente                 | Sì - Multiplo                 | Una corrispondenza                      |
| Alta             | 2        | Completamente                 | Sì - Multiplo                 | Più corrispondenze               |
| Alta             | 3        | Completamente                 | Sì                            | Una corrispondenza                      |
| Alta             | 4        | Completamente                 | Sì                            | Più corrispondenze               |
| Alta             | 5        | Parzialmente             | Sì - Multiplo                 | Una corrispondenza                      |
| Alta             | 6        | Parzialmente             | Sì - Multiplo                 | Più corrispondenze               |
| Alta             | 7        | Parzialmente             | Sì                            | Una corrispondenza                      |
| Alta             | 8        | Completamente                 | Nr.                             | Una corrispondenza                      |
| Alta             | 9        | Nr.                    | Sì - Multiplo                 | Una corrispondenza                      |
| Alta             | 10       | Nr.                    | Sì - Multiplo                 | Più corrispondenze               |
| Media           | 1        | Completamente                 | Sì - Multiplo                 | Non considerato                 |
| Media           | 2        | Completamente                 | Sì                            | Non considerato                 |
| Media           | 3        | Completamente                 | Nr.                             | Più corrispondenze               |
| Media           | 4        | Parzialmente             | Sì - Multiplo                 | Non considerato                 |
| Media           | 5        | Parzialmente             | Sì                            | Non considerato                 |
| Media           | 6        | Nr.                    | Sì                            | Una corrispondenza                      |
| Media           | 7        | Nr.                    | Sì-Multiplo                   | Non considerato                 |
| Media           | 8        | Parzialmente             | Nr.                             | Una corrispondenza                      |
| Media           | 9        | Nr.                    | Sì                            | Non considerato                 |
| Bassa              | 1        | Completamente                 | Nr.                             | Nessuna corrispondenza                     |
| Bassa              | 2        | Parzialmente             | Nr.                             | Più corrispondenze               |
| Bassa              | 3        | Parzialmente             | Nr.                             | Nessuna corrispondenza                     |
| Bassa              | 4        | Nr.                    | Nr.                             | Una corrispondenza                      |
| Bassa              | 5        | Nr.                    | Nr.                             | Più corrispondenze               |

## Vedere anche
[Riconciliare i pagamenti utilizzando il collegamento automatico](receivables-how-reconcile-payments-auto-application.md)  
[Gestione della contabilità clienti](receivables-manage-receivables.md)  
[Vendite](sales-manage-sales.md)  
[Utilizzare [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
