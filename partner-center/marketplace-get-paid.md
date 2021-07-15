---
title: Pagamento in Partner Center
description: Informazioni su come ricevere pagamenti per gli utili come partner Microsoft, ad esempio tramite offerte del marketplace commerciale, programmi di incentivi e Cloud Solution Provider programma. Include i criteri di pagamento, lo stato di blocco dei pagamenti e gli estratti conto.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
ms.date: 07/12/2021
author: eunjkim520
ms.author: eunjkim
ms.openlocfilehash: 99cc0172f9cb1e09bdc77bbd9187ad2452c19c61
ms.sourcegitcommit: 207c86406e56346d01d85ce50ea494c0c293519a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/14/2021
ms.locfileid: "113798137"
---
# <a name="getting-paid-in-partner-center"></a>Pagamento in Partner Center

**Ruoli appropriati:** amministratore account | Amministratore globale

Questo articolo contiene informazioni importanti sulla ricezione del pagamento per le offerte, i componenti aggiuntivi e gli utili pubblicitari. Vengono riepilogati i criteri di pagamento, i passaggi necessari prima del pagamento e la panoramica dell'estratto conto.

## <a name="payout-policies-and-agreements"></a>Criteri e contratti di pagamento

Per ottenere il pagamento è necessario rispettare i contratti e i criteri di pagamento.

- [Microsoft Azure marketplace Publisher:](/legal/marketplace/msft-publisher-agreement)prima di essere pagato, è necessario accettare questo contratto per editori. Questo contratto illustra la relazione tra l'utente e Microsoft in relazione alle offerte dei venditori nel marketplace commerciale, inclusa la tariffa per lo store che Microsoft addebita per ogni vendita effettuata.
- [I criteri di pagamento](payout-policy-details.md) mostrano i criteri di pagamento dei pagamenti, inclusi la pianificazione e i metodi di pagamento. I criteri spiegano anche il processo per i non pagamenti dei clienti.
- [Dettagli fiscali](tax-details-marketplace.md) spiega la considerazione fiscale per la selezione dei prezzi e la responsabilità fiscale ai sensi del Contratto Microsoft [Publisher.](/legal/marketplace/msft-publisher-agreement)
- **Le tariffe dello** Store sono ufficialmente previste nelle [tariffe del marketplace commerciale.](/azure/marketplace/marketplace-commercial-transaction-capabilities-and-considerations)
- **I** pagamenti vengono effettuati su base mensile ,a condizione che sia stata raggiunta la soglia di pagamento. In genere i pagamenti dovuti in un determinato mese vengono inviati entro il 15° giorno del mese. I pagamenti in genere sono da 3 a 10 giorni lavorativi aggiuntivi per raggiungere l'account dei pagamenti. Per informazioni dettagliate, vedere [Soglie, metodi e intervalli di pagamento](payment-thresholds-methods-timeframes.md).

## <a name="prerequisite-steps-before-getting-paid"></a>Passaggi preliminari prima del pagamento

Prima di ricevere il primo pagamento, è necessario configurare l'account dei pagamenti e completare i moduli bancari e fiscali necessari. Nei moduli bancari e fiscali verranno forniti i metodi di pagamento preferiti e i moduli fiscali per la ritenuta d'acconto. I moduli bancari e fiscali sono necessari prima del pagamento. Per informazioni dettagliate, [vedere Configurare l'account dei pagamenti e i moduli fiscali.](set-up-your-payout-account.md)

### <a name="payout-hold-status"></a>Stato di blocco dei pagamenti

Per impostazione predefinita, i pagamenti verranno corrisposti su base mensile, come descritto sopra. Tuttavia, è possibile mettere in attesa i pagamenti per un programma e Microsoft non rilascerà i pagamenti all'account. Se si sceglie di mettere in attesa i pagamenti, gli utili continueranno a essere registrati nella **pagina Proventi.** Non verranno tuttavia inviati pagamenti all'account fino a quando non sarà rimosso il blocco.

Per mettere in attesa i pagamenti, selezionare l Impostazioni **icona** a forma di ingranaggio in alto a destra, quindi **Impostazioni account.** Selezionare **Payout and tax** (Pagamenti e imposte) nel menu a sinistra e nella sezione **Payout and tax profile assignment** (Assegnazione profilo di pagamento e imposta) individuare il programma per il quale si desidera effettuare i pagamenti. Selezionare la **casella di controllo Hold my Payment** (Mantieni pagamento) per contenere i pagamenti per questo programma. È possibile modificare lo stato di blocco dei pagamenti in qualsiasi momento, ma la decisione influirà sul pagamento mensile successivo. Se ad esempio si vuole bloccare il pagamento di aprile, assicurarsi di impostare lo stato di blocco dei pagamenti su **Sì** entro la fine di marzo.

Dopo aver impostato lo stato di blocco dei pagamenti su On **,** tutti i pagamenti per questo programma saranno in attesa fino a quando non si deseleziona la casella di controllo **su Off**. In questo caso, l'utente verrà incluso durante il ciclo di pagamento mensile successivo ( a condizione che sia stata raggiunta la soglia di pagamento). Se i pagamenti sono in attesa, ma si vuole generare un pagamento a giugno,  deselezionare la casella di controllo Su Disattivato prima della fine di maggio.

>[!Note]
> Lo stato di blocco dei pagamenti si applica a ogni singolo programma (Microsoft Store, annunci pubblicitari, Azure Marketplace e così via). Se si desidera mantenere i pagamenti per tutti i programmi, mantenere il pagamento per ogni programma singolarmente.

## <a name="payout-statements"></a>Estratti conto

L'estratto conto mostra gli utili delle vendite delle offerte e dei componenti aggiuntivi nella cronologia delle transazioni. È anche possibile visualizzare i dettagli del pagamento e scaricare i report in formato tsv o csv. Per [altre informazioni su come](payout-statement.md) accedere all'estratto conto e sui dettagli della cronologia delle transazioni e dei report di pagamento, vedere Estratto conto. È anche possibile usare [l'API dei pagamenti dei partner](https://apidocs.microsoft.com/services/partnerpayouts) per eseguire sistematicamente il pull dei report sui pagamenti.

## <a name="next-steps"></a>Passaggi successivi

- [API dei pagamenti dei partner](https://apidocs.microsoft.com/services/partnerpayouts)
- [Domande frequenti su Proventi](payout-faq.yml)