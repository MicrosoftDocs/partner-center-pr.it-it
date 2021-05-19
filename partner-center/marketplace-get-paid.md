---
title: Pagamento in Partner Center
description: Informazioni sulla ricezione di pagamenti per gli utili come partner Microsoft, ad esempio tramite offerte del marketplace commerciale, programmi di incentivi e Cloud Solution Provider programma. Include i criteri di pagamento, lo stato di blocco dei pagamenti e gli estratti conto.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
ms.date: 11/25/2020
author: eunjkim520
ms.author: eunjkim
ms.openlocfilehash: 3dc8b728ef20da77b9a6d2a925ebb0388ea53837
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146494"
---
# <a name="getting-paid-in-partner-center"></a>Pagamento in Partner Center

**Ruoli appropriati:** Account admin | Amministratore globale

Questo articolo contiene informazioni importanti sulla ricezione del pagamento per le offerte, i componenti aggiuntivi e gli utili pubblicitari. Riepiloga i criteri di pagamento, i passaggi necessari prima del pagamento e la panoramica dell'estratto conto.

## <a name="payout-policies-and-agreements"></a>Criteri e contratti di pagamento

Per ottenere il pagamento è necessario rispettare i contratti e i criteri di pagamento.

- [Microsoft Azure Marketplace Contratto per gli editori:](/legal/marketplace/msft-publisher-agreement)prima di ricevere il pagamento, è necessario accettare il contratto dell'editore. Questo contratto illustra la relazione tra l'utente e Microsoft in relazione alle offerte del venditore nel marketplace commerciale, inclusa la tariffa del negozio che Microsoft addebita per ogni vendita effettuata.
- [I criteri di pagamento](payout-policy-details.md) mostrano i criteri di pagamento dei pagamenti, inclusi la pianificazione dei pagamenti e i metodi di pagamento. I criteri illustrano anche il processo per i non pagamenti dei clienti.
- [Dettagli fiscali](tax-details-marketplace.md) illustra la considerazione fiscale per la selezione dei prezzi e la responsabilità fiscale in base al Contratto Microsoft [Publisher.](/legal/marketplace/msft-publisher-agreement)
- **I costi dello** Store sono definiti ufficialmente nel Contratto per gli editori. La tariffa dello Store viene applicata a tutte le vendite di offerte raccolte dal marketplace commerciale, inclusi i componenti aggiuntivi.
- **I** pagamenti vengono effettuati su base mensile (a condizione che sia stata raggiunta la soglia di pagamento). In genere, i pagamenti dovuti in un determinato mese vengono inviati entro il 15° giorno del mese. I pagamenti in genere sono da 3 a 10 giorni lavorativi aggiuntivi per raggiungere l'account di pagamento. Per informazioni dettagliate, vedere [Soglie, metodi e intervalli di pagamento](payment-thresholds-methods-timeframes.md).

## <a name="prerequisite-steps-before-getting-paid"></a>Passaggi preliminari prima del pagamento

Prima di ricevere il primo pagamento, è necessario configurare l'account dei pagamenti e completare i moduli bancari e fiscali necessari. Nei moduli bancari e fiscali verranno forniti i metodi di pagamento preferiti e i moduli fiscali per la ritenuta d'acconto. I moduli bancari e fiscali sono necessari prima del pagamento. Per informazioni dettagliate, [vedere Configurare l'account dei pagamenti e i moduli fiscali.](set-up-your-payout-account.md)

### <a name="payout-hold-status"></a>Stato di blocco dei pagamenti

Per impostazione predefinita, i pagamenti verranno corrisposti su base mensile, come descritto sopra. Tuttavia, è possibile mettere in attesa i pagamenti per un programma e Microsoft non rilascerà i pagamenti all'account. Se si sceglie di mettere in attesa i pagamenti, gli utili continueranno a essere registrati nella **pagina Proventi.** Non verranno tuttavia inviati pagamenti all'account fino a quando non sarà rimosso il blocco.

Per mettere in attesa i pagamenti, selezionare **l'icona a** forma di ingranaggio Impostazioni in alto a destra, quindi **Impostazioni account.** Selezionare **Payout and tax** (Pagamenti e imposte) nel menu a sinistra e nella sezione **Payout and tax profile assignment** (Assegnazione del profilo di pagamento e fiscale) individuare il programma per cui si desidera effettuare i pagamenti. Selezionare la **casella di controllo Hold my Payment** (Mantieni pagamento) per contenere i pagamenti per questo programma. È possibile modificare lo stato di blocco dei pagamenti in qualsiasi momento, ma la decisione influirà sul pagamento mensile successivo. Se ad esempio si vuole bloccare il pagamento di aprile, assicurarsi di impostare lo stato di blocco dei pagamenti su **Sì** entro la fine di marzo.

Dopo aver impostato lo stato di blocco dei pagamenti su On **,** tutti i pagamenti per questo programma saranno in attesa fino a quando non si deseleziona la casella di controllo **su Off**. In questo caso, l'utente verrà incluso durante il ciclo di pagamento mensile successivo, a condizione che sia stata raggiunta la soglia di pagamento. Se i pagamenti sono in attesa, ma si vuole che venga generato un pagamento a  giugno, deselezionare la casella di controllo Su Disattivato prima della fine di maggio.

>[!Note]
> Lo stato di blocco dei pagamenti si applica a ogni programma singolarmente (Microsoft Store, annunci pubblicitari, Azure Marketplace e così via). Se si desidera mantenere i pagamenti per tutti i programmi, mantenere il pagamento per ogni programma singolarmente.

## <a name="payout-statements"></a>Estratti conto

L'estratto conto mostra gli utili delle vendite delle offerte e dei componenti aggiuntivi nella cronologia delle transazioni. È anche possibile visualizzare i dettagli del pagamento e scaricare i report in formato tsv o csv. Per [altre informazioni su](payout-statement.md) come accedere all'estratto conto dei pagamenti e sui dettagli della cronologia delle transazioni e dei report di pagamento, vedere Estratto conto. È anche possibile usare [l'API Pagamenti](https://apidocs.microsoft.com/services/partnerpayouts) partner per eseguire il pull sistematico dei report sui pagamenti.

## <a name="next-steps"></a>Passaggi successivi

- [API di pagamento dei partner](https://apidocs.microsoft.com/services/partnerpayouts)
- [Domande frequenti su Proventi](payout-faq.md)