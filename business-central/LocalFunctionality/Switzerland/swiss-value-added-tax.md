---
title: 'IVA svizzera [CH]'
description: Questo articolo spiega diversi miglioramenti apportati alle funzionalità di dichiarazione IVA svizzera.
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: null
ms.date: 06/25/2021
ms.author: edupont
---
# <a name="swiss-value-added-tax"></a><a name="swiss-value-added-tax"></a>IVA svizzera

[!INCLUDE[prod_short](../../includes/prod_short.md)] includono i seguenti miglioramenti alla dichiarazione IVA svizzera:  

- Rettifica automatica degli importi IVA per fatture, in base agli sconti di pagamento.  
- Tassi di cambio IVA aggiuntivi per le fatture in valute estere.  

Per ulteriori informazioni sui requisiti di codifica a reporting dell'IVA svizzera, vedi [Informazioni sull'IVA svizzera](https://www.estv.admin.ch/estv/en/home/value-added-tax.html). Le informazioni sono disponibili in francese, tedesco, italiano e inglese.  

## <a name="vat-amounts-and-vat-exchange-rates"></a><a name="vat-amounts-and-vat-exchange-rates"></a>Importi IVA e tassi di cambio IVA

Secondo le leggi locali dell'IVA, l'importo base dell'IVA per una fattura può essere ridotto dello sconto di pagamento se viene concesso uno sconto. Per consentire la rettifica automatica dell'IVA per uno sconto di pagamento su una fattura, il campo **Rettifica per sconto pagamento** viene attivato per impostazione predefinita nella pagina **Setup contabilità generale**. È anche possibile attivare questa funzione nel setup registrazioni IVA. Per ulteriori informazioni, vedere la tabella Setup contabilità generale e Setup registrazioni IVA.  

### <a name="currency-exchange-rates-for-vat-reporting"></a><a name="currency-exchange-rates-for-vat-reporting"></a>Tassi di cambio valuta per dichiarazione IVA

Per le fatture in valuta estera è necessario utilizzare il tasso di cambio ufficiale fornito dal governo per il calcolo dell'IVA. È inoltre possibile impostare ulteriori tassi di cambio per l'IVA, che è possibile utilizzare per aspetti della fattura diversi dal calcolo dell'IVA. È possibile fornire il corretto tasso di cambio dell'IVA di governo per ogni valuta estera rilevante nel setup dei tassi di cambio per le fatture. Per ulteriori informazioni, vedere la tabella Tassi di cambio valute.  

È inoltre possibile rettificare tutti gli importi IVA nei movimenti IVA risultanti da transazioni in valuta estera. Quando si attiva la funzione di rettifica del tasso di cambio IVA, i tassi di cambio IVA vengono rettificati automaticamente. Le differenze positive derivanti dai tassi di cambio sono registrate in conti di utili di conversione. Le differenze negative derivanti dai tassi di cambio sono registrate in conti di perdite di conversione. Per ulteriori informazioni, vedere il processo batch Rettifica tassi di cambio.  

Ulteriori informazioni, come l'aliquota IVA e l'importo in valuta originale, vengono trasferiti ai movimenti IVA. Per ulteriori informazioni, vedere la tabella Movimenti IVA.  

## <a name="see-also"></a><a name="see-also"></a>Vedi anche

[Aliquote IVA per la Svizzera](vat-rates-for-switzerland.md)   
[Creare e stampare una dichiarazione IVA svizzera](how-to-create-and-print-a-swiss-vat-statement.md)   
[Funzionalità locale per la Svizzera](switzerland-local-functionality.md)   


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
