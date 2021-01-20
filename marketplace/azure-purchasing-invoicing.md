---
title: Acquisto di software e soluzioni da Azure Marketplace
description: Informazioni sugli strumenti che semplificano e semplificano gli acquisti e la gestione di software in Azure Marketplace.
ms.prod: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 01/18/2021
ms.openlocfilehash: de58fad7af7dd2cd6b8c98e5763557d54cc776a2
ms.sourcegitcommit: c46658f4d70004596e758fe4cd8671b6e9dadeab
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/20/2021
ms.locfileid: "98584211"
---
# <a name="azure-marketplace-purchasing"></a>Acquisto in Azure Marketplace

Azure Marketplace offre numerosi strumenti e funzionalità che semplificano e semplificano il processo di acquisto, fatturazione e gestione dei criteri di acquisto.

## <a name="simplified-procurement"></a>Approvvigionamento semplificato

Azure Marketplace semplifica di processo di approvvigionamento offrendo varie opzioni di acquisto. Se si acquistano prodotti usando una carta di credito associata all'account Azure, tutti gli acquisti verranno consolidati in una singola fattura e addebitati alla carta di credito scelta. Se sei un cliente di grandi dimensioni, puoi acquistare usando un Enterprise Agreement. Con un contratto Enterprise, tutti gli acquisti di software vengono inclusi automaticamente nella fattura di Azure. che indicherà prima gli addebiti per l'utilizzo di Azure e quindi gli addebiti di Azure Marketplace.

Quando si acquista tramite Azure Marketplace, si elimina la complessità della gestione delle relazioni e delle fatture dei singoli fornitori. Si ottiene una singola fattura mensile consolidata da Microsoft che include gli acquisti in Azure Marketplace e i costi di Azure.

## <a name="permission-to-purchase"></a>Autorizzazione per l'acquisto

Una volta individuata l'applicazione software corretta, il completamento dell'acquisto è semplice. Tuttavia, sarà necessario disporre di autorizzazioni appropriate nella sottoscrizione di Azure. Poiché Azure opera su un modello di [controllo degli accessi in base al ruolo](/azure/role-based-access-control/overview) , è necessario che l'account disponga delle autorizzazioni di proprietario o **collaboratore** della **sottoscrizione** per effettuare un acquisto.

Prima di completare un acquisto, assicurarsi che l'utente abbia la configurazione corretta nel tenant di Azure. Ciò consente di evitare errori durante l'acquisto.

In Azure Marketplace nell'portale di Azure trovare l'applicazione che si vuole acquistare e selezionare **Crea** o **Configura + Sottoscrivi**. Prima di poter usare la nuova soluzione verrà richiesto di completare alcune informazioni.

:::image type="content" source="media/overview/offer-create-screen.png" alt-text="Pulsante Crea offerta.":::

:::image type="content" source="media/overview/button-set-up-and-subscribe.png" alt-text="Pulsante Imposta + Sottoscrivi.":::

Se si vuole distribuire una soluzione da Azure Marketplace Online Store, selezionare **Get it now** nella pagina Product Description (Descrizione prodotto) e quindi accedere con le credenziali dell'account Azure.

:::image type="content" source="media/overview/sign-in-to-azure-marketplace.png" alt-text="La finestra di dialogo di accesso ad Azure Marketplace.":::

Una volta effettuato l'accesso, si verrà reindirizzati al prodotto nella portale di Azure per completare l'acquisto.

## <a name="purchase-policy-management"></a>Gestione dei criteri di acquisto

Microsoft consente di gestire gli acquisti degli utenti tramite il proprio profilo di fatturazione come amministratore della sottoscrizione di Azure. Scegliere tra tre opzioni:

- **Gratuito** e a pagamento: consente agli utenti di acquisire qualsiasi applicazione software di Azure Marketplace.
- **Gratuito** : consente agli utenti di distribuire solo software gratuito da Azure Marketplace.
- **No** : impedisce agli utenti di distribuire software da Azure Marketplace.

Queste impostazioni si applicano a tutti gli utenti con accesso alla sottoscrizione di Azure, che offre la possibilità di controllare l'approvvigionamento IT tramite il portale di Azure.

:::image type="content" source="media/overview/billing-profile-policy-settings.png" alt-text="Controllo dell'approvvigionamento IT tramite il portale di Azure":::

## <a name="cost-management"></a>Gestione dei costi

Quando si acquistano prodotti da Azure Marketplace, è possibile ottenere informazioni dettagliate che consentono di gestire i costi. Gestione costi di Azure è uno strumento gratuito per la visualizzazione di informazioni sui prodotti acquistati. È possibile usare gestione costi per visualizzare i dettagli dei servizi di cui si spende il denaro nel tempo e il modo in cui questi costi si rilevano rispetto ai budget impostati. Oltre a impostare i budget, è possibile pianificare i report e analizzare i costi di sottoscrizione. Scopri di più su gestione costi di Azure completando il modulo Microsoft Learn in [analizzare i costi e creare budget con gestione costi di Azure](/learn/modules/analyze-costs-create-budgets-azure-cost-management/).

È possibile visualizzare le fatture e gli addebiti di Azure Marketplace nello strumento di analisi dei costi disponibile in Gestione costi di Azure.

:::image type="content" source="media/overview/azure-cost-management.png" alt-text="Usa gestione costi di Azure per ottenere informazioni dettagliate sui prodotti acquistati.":::

## <a name="purchase-validation-checks"></a>Acquistare i controlli di convalida

L'acquisto di un'offerta tramite Azure Marketplace può avere esito negativo per diversi motivi. L'uso dell'interfaccia della riga di comando (CLI) per un acquisto è più probabile che causi errori poiché è possibile che si stia tentando di acquistare un'offerta non disponibile o visibile in Azure Marketplace. Di seguito sono riportati i controlli che possono causare un errore di acquisto:

1. La sottoscrizione appartiene a un Enterprise Agreement (EA) e l'amministratore EA ha disabilitato gli acquisti su Azure Marketplace.
1. L'amministratore EA ha abilitato gli acquisti solo per le offerte gratuite e l'offerta è un'offerta a pagamento.
1. L'offerta non è disponibile nel Marketplace.
1. Il fornitore di software indipendente (ISV) ha interrotto la vendita dell'offerta, almeno nella propria area geografica.
1. La sottoscrizione in uso appartiene a un account di fatturazione in un'area in cui l'offerta non è disponibile.
1. L'account di sottoscrizione/fatturazione non è associato a uno strumento di pagamento valido, ad esempio una carta di credito valida.
1. La sottoscrizione appartiene a un provider di soluzioni cloud (CSP) e l'ISV ha rifiutato la vendita tramite un CSP.
1. Il Marketplace privato è abilitato per la sottoscrizione e l'offerta non è presente nell'elenco delle offerte consentite.
1. L'offerta è privata/anteprima per clienti specifici e la sottoscrizione non è presente nell'elenco dei clienti autorizzati.

## <a name="next-steps"></a>Passaggi successivi

- [Fatturazione](billing-invoicing.md)