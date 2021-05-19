---
title: Credito ottenuto dai partner per i servizi gestiti
ms.topic: article
ms.date: 12/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come viene calcolato e pagato il credito ottenuto dai partner Microsoft per i servizi gestiti e come verificare se si possiedono i requisiti necessari.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: ba422a2feae2affb9c2b60ad345c4d6bb0d525c7
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110145865"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a>Come viene calcolato e pagato il credito ottenuto dai partner

**Ruoli appropriati:** Amministratore globale | Amministratore di gestione utenti | Agente amministratore | Gestione della fatturazione | Agente di vendita

Il credito ottenuto dai partner per i servizi gestiti (PEC) riconosce e premia i partner a cui sono affidati il controllo e la gestione operativi IT 24 ore su 24, 7 giorni su 7, dell'ambiente Azure intero o parziale dei clienti. Per impostazione predefinita, in CSP ai partner vengono concessi i necessari diritti di accesso alla sottoscrizione del cliente, in modo che possano eseguire 24 ore su 24, 7 giorni su 7 la gestione e il controllo operativi delle risorse della sottoscrizione. Altri modi in cui i clienti possono effettuare il provisioning dell'accesso per i partner transazionali sono descritti nella sezione seguente. L'importo della fattura mensile è il netto del credito ottenuto dal partner. I partner possono esaminare nel file di riconciliazione mensile i dettagli del credito ottenuto. Per gli altri modi in cui il cliente può effettuare il provisioning dell'accesso per il partner di transazione, leggi [Gestire sottoscrizioni e risorse nel piano di Azure](azure-plan-manage.md).

Leggi anche [Ripristinare i privilegi di amministratore per le sottoscrizioni di Azure CSP](revoke-reinstate-csp.md).

## <a name="eligibility"></a>Idoneità

Per ricevere il credito ottenuto dal partner (PEC), si applicano i requisiti seguenti: 

- È necessario disporre di un contratto MPN attivo e di un ruolo controllo degli accessi in base al ruolo valido per ricevere il credito ottenuto per gli asset di Azure gestiti.

- È necessario esercitare 24 ore su 24, 7 giorni su 7 il controllo e la gestione operativi delle risorse di Azure del cliente in CSP. Ciò significa che è necessario disporre dei privilegi di amministratore per la sottoscrizione di Azure del cliente, il gruppo di risorse di Azure e la risorsa di Azure. Nel caso di provider indiretti e dei relativi rivenditori indiretti, il provider indiretto sarà idoneo per il credito ottenuto dal partner se egli stesso, il rivenditore indiretto oppure entrambi esercitano questo controllo operativo. Per altre informazioni, vedere [Ripristinare i privilegi di amministratore per le sottoscrizioni di Azure CSP](./revoke-reinstate-csp.md).

- Oltre ai requisiti precedenti, il credito ottenuto dal partner è applicabile ai servizi elencati nei prezzi per l'utilizzo del piano di Azure che è possibile esportare dalla pagina dei [prezzi del piano di Azure](https://partner.microsoft.com/commerce/sales).

- Il credito ottenuto dal partner **non** è applicabile ai servizi seguenti:
    - Prenotazioni del piano di Azure
    - Prodotti di terze parti identificati come Terze parti nella colonna Tag del prezzo di utilizzo del piano di Azure
    - Prodotti inclusi nel listino prezzi del marketplace
    - [Macchine virtuali Spot di Azure](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

- Il credito viene ottenuto dai partner a livello delle risorse di Azure. Se si dispone di un accesso valido a livello di sottoscrizione o di gruppo di risorse, otterrà il credito ogni risorsa con ruolo autorizzato fino all'entità più alta.

- Informazioni dettagliate sul credito ottenuto dal partner sono disponibili anche nella pagina [Gestione costi di Azure](/azure/cost-management-billing/costs/get-started-partners).

### <a name="calculation"></a>Calcolo

Il credito ottenuto dai partner viene calcolato quotidianamente e può essere controllato nel file di utilizzo giornaliero e nel file di riconciliazione della fattura mensile. Un partner (provider indiretto o rivenditore indiretto) deve avere accesso per l'intero giorno (24 ore su 24, 7 giorni su 7) per ottenere il credito. Il credito ottenuto dal partner viene calcolato quotidianamente per gli asset di Azure gestiti. I partner che mantengono l'accesso con privilegi permanenti per tutto il mese (intervallo di accesso) e per tutte le risorse idonee (ambito di accesso) ottengono un pec completo. Una riduzione dell'ambito e dell'intervallo avrà come risultato una diminuzione della percentuale di credito per il mese. Il file relativo all'utilizzo quotidiano stimato mostra ogni giorno se per un asset di Azure è applicabile o meno il credito ottenuto dal partner. I partner possono inoltre registrarsi in modo da ricevere avvisi per il monitoraggio delle modifiche all'accesso con privilegi permanenti.

## <a name="azure-cost-management"></a>Azure Cost Management

Gestione costi di Azure (ACM) con Analisi dei costi consente a ogni partner di visualizzare i costi che hanno ricevuto il vantaggio di credito ottenuto dai partner.  

1. Nel [portale di Azure](https://portal.azure.com) accedere al tenant del partner e selezionare **Gestione dei costi e fatturazione**.

2. Seleziona **Gestione costi**.

3. Seleziona **Analisi dei costi**.

   Nella visualizzazione Analisi dei costi verranno visualizzati i costi per l'account di fatturazione relativi a tutti i servizi acquistati e utilizzati ai prezzi pagati a Microsoft.

4. Selezionare **PartnerEarnedCreditApplied** nell'elenco a discesa di un grafico pivot per visualizzare i costi a cui è applicata la pec. Quando la proprietà **PartnerEarnedCreditApplied** è True, il costo associato ha il vantaggio di credito ottenuto dai partner. 

   Quando la proprietà PartnerEarnedCreditApplied è False, il costo associato non soddisfa il criterio di idoneità del credito o il servizio acquistato non è idoneo al credito ottenuto dai partner.

   >[!NOTE] 
   >Sono in genere necessarie 8-24 ore prima che l'uso dei servizi in **Gestione costi** diventi visibile, mentre i crediti ottenuti dai partner vengono visualizzati entro 48 ore dal momento dell'accesso in Gestione costi di Azure.

5. Puoi anche raggruppare o filtrare in base alla proprietà **PartnerEarnedCreditApplied** usando le funzionalità di filtro **Raggruppa per e Aggiungi** per visualizzare in dettaglio i costi a cui è applicato il credito ottenuto dai partner e quelli a cui tale credito non è applicato.

## <a name="next-steps"></a>Passaggi successivi

- [Credito ottenuto dai partner - Panoramica](partner-earned-credit.md)

- Esempi dettagliati di calcoli del credito ottenuto dal partner si trovano nel listino prezzi che è possibile raggiungere tramite il dashboard Partner Center (è necessario accedere).

- [Passare al piano di Azure - Introduzione](azure-plan-get-started.md)

- [Gestire sottoscrizioni e risorse nel piano di Azure](azure-plan-manage.md)

- [Revocare o ripristinare i privilegi di amministratore per Azure CSP sottoscrizioni](revoke-reinstate-csp.md)
