---
title: Analizzare sottoscrizioni e licenze
description: Informazioni su come usare le metriche nella pagina sottoscrizione e analisi licenze per identificare i successi e le aree che richiedono maggiore attenzione.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.topic: article
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 03/31/2021
ms.openlocfilehash: 3f84026cc6402bea71837b06a5e330f2c879a06b
ms.sourcegitcommit: 766b2bb46dffd29e532b42106359f83e51b96700
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/31/2021
ms.locfileid: "106103792"
---
# <a name="analyze-subscriptions-and-licenses-to-help-you-drive-business-decisions-and-new-goals"></a>Analizza le sottoscrizioni e le licenze per aiutarti a promuovere decisioni aziendali e nuovi obiettivi

**Ruoli appropriati**

- Amministratore globale
- Amministratore gestione utenti
- Agente amministratore
- Agente di vendita

I dati prendono le decisioni aziendali. Usare le metriche nella pagina **sottoscrizione e analisi licenze** per identificare i successi e le aree che richiedono maggiore attenzione. Utilizzare queste informazioni durante la pianificazione di nuovi obiettivi aziendali.

**CSP TTM ricavi (USD)**: questa metrica rappresenta l'aggregato CSP fatturato ricavi (USD) per i dodici mesi finali (TTM) per gli account del percorso partner e l'account globale del partner (PGA) a cui è associato questo account CSP. Se si dispone di altri account CSP con un altro PGA, è necessario accedere a ognuno di essi per visualizzare il corrispondente ricavo TTM aggregato.  Fai clic sul collegamento Dettagli download per ottenere una ripartizione dei ricavi TTM (USD) per ID MPN.

>[!NOTE]
>I prezzi di valuta locali (Legacy Commerce FX) in commerciale vengono gestiti entro +/-5% di dollari USA. Il tasso di cambio di borsa (FX) Legacy è diverso dalle tariffe FX per la fatturazione usate da Azure nell'esperienza commerciale moderna. Le tariffe FX per la fatturazione moderna di Commerce sono basate sulle tariffe di Microsoft P&L (tariffe FX Reuters del feed di tesoreria). Le tariffe FX di Commerce legacy sono riservate a Microsoft.


Il resto del report può essere trasformato tramite pivot in base ai prodotti seguenti:

 - **Dynamics 365**: dati di Dynamics 365  
 - **EMS**: dati di Enterprise Management Services  
 - **Microsoft 365**: Microsoft 365 dati  
 - **Office 365**: dati di Office 365  


## <a name="types-of-subscription-and-license-metrics-you-can-view"></a>Tipi di metriche di sottoscrizione e di licenza che è possibile visualizzare

Vengono monitorate le metriche seguenti:

**Summary**  
 - **Sottoscrizioni vendute**: numero di sottoscrizioni create per il periodo di tempo specificato  
  
 - **Licenze vendute**: numero di licenze vendute per il periodo di tempo specificato  
  
 - **Rinnovo delle sottoscrizioni in 30 giorni**: numero di sottoscrizioni in cui lo stato è attivo per il periodo di tempo specificato e dove **autorenew** è true
 
 - **Sottoscrizioni attive**: sottoscrizioni in cui lo stato è **attivo**  
 
 - **Sottoscrizioni sospese**: numero di sottoscrizioni sospese senza filtro data  

**Suddivisione del prodotto**
  
 - **Conteggio delle sottoscrizioni**: primi 5 prodotti ordinati per sottoscrizioni vendute  
 
 - **Numero di licenze**: i primi 5 prodotti ordinati per licenze

**Conservazione della sottoscrizione**

 - **Sottoscrizioni rinnovate**: sottoscrizioni rinnovate negli ultimi 30 giorni  

**Varianza sottoscrizione**  
 - **Nuove sottoscrizioni**: numero di nuove sottoscrizioni per il periodo di tempo, escluse le offerte di valutazione  
 
 - **Sottoscrizioni con provisioning**: numero di sottoscrizioni sottoposte a provisioning o sospese per data  

**Sottoscrizioni sospese** 
 
 - Elenco di tutte le sottoscrizioni con stato **sospeso**, escluse le offerte di valutazione  
  
**Sottoscrizioni attive**

 - Elenco di tutte le sottoscrizioni attive  

**Conversioni della sottoscrizione di valutazione**  

 - **Conversione della versione di valutazione**: numero di tutte le sottoscrizioni **attive** in cui la versione di valutazione è stata pagata durante il periodo di tempo  

**Sottoscrizioni di valutazione che terminano tra 30 giorni**  

 - Elenco delle versioni di valutazione avviate, in cui la data di fine è entro 30 giorni e non è presente alcuna data di inizio a pagamento associata alla sottoscrizione  



## <a name="next-steps"></a>Passaggi successivi

- [Analizzare le prestazioni dei rivenditori indiretti](analyze-indirect-resellers.md)