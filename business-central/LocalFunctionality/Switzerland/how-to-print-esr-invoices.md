---
title: 'Procedura: Stampare fatture ESR'
description: "È possibile stampare il bollettino bancario ESR (Einzahlungsschein mit Referenznummer) in diversi modi."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: 9f345827f1cc705727f80d21a00839f221044059
ms.contentlocale: it-ch
ms.lasthandoff: 11/26/2018

---
# <a name="print-esr-invoices"></a>Stampare fatture ESR
È possibile stampare il bollettino bancario ESR (Einzahlungsschein mit Referenznummer) nei seguenti modi:  

- Incluso nell'ESR della fattura di vendita.  
- Come documento separato chiamato tagliando ESR.  

Il report ESR della fattura di vendita corrisponde alla fattura di vendita accompagnata da un tagliando ESR aggiuntivo. Utilizzando il report tagliando ESR di vendita è possibile stampare la distinta di deposito blu.  

> [!NOTE]  
>  È necessario selezionare una stampante e selezionare le impostazioni durante l'installazione del modulo di pagamento ESR per stampare correttamente la distinta di deposito. Per ulteriori informazioni, vedere la tabella Selezioni stampante.  

La procedura seguente descrive come stampare le fatture di vendita ESR, ma gli stessi passaggi si applicano anche alla stampa dei tagliandi ESR.  

## <a name="to-print-esr-invoices"></a>Per stampare fatture ESR  

1.  Scegliere l'icona ![Cerca pagina o report](../../media/ui-search/search_small.png "icona Cerca pagina o report"), immettere **Fattura ESR**, quindi scegliere il collegamento correlato.  
2.  Nel processo batch **Fattura di vendita ESR**, nella Scheda dettaglio **Opzioni** compilare i campi come descritto nella tabella seguente.  

    |Campo|Descrizione|  
    |---------------------------------|---------------------------------------|  
    |**Nr di copie**|Immettere il numero richiesto di copie del report.|  
    |**Banca ESR**|Selezionare il codice bancario ESR da stampare nel report.<br /><br /> Se il valore in questo campo è <Blank> e il codice del metodo di pagamento ESF non è definito nella pagina **Setup ESR**, verrà stampata la banca principale ESR selezionata nella pagina **Setup ESR**.|  
    |**LogInteraction**|Specificare se le interazioni con i tuoi contatti verranno registrate.|  
    |**Sistema ESR**|Selezionare il sistema ESR con cui è possibile inviare i nuovi tagliandi ESR ai clienti. Per utilizzare il sistema ESR utilizzato dalla banca che hai specificato nel campo **Banca ESR**, selezionare **Basato su banca ESR**.|  

3.  Scegliere il pulsante **Stampa** per stampare il report oppure scegliere il pulsante **Anteprima** per visualizzarlo sullo schermo.  

È inoltre possibile ristampare il report ESR della fattura di vendita o il report del tagliando ESR di vendita.  

## <a name="see-also"></a>Vedi anche  
 [Pagamenti elettronici svizzeri tramite ESR](swiss-electronic-payments-using-esr.md)   
 [Importare i pagamenti ESR](how-to-import-esr-payments.md)

