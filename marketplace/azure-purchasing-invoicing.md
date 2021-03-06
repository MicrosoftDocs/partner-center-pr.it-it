---
title: Acquisto di software e soluzioni da Azure Marketplace
description: Informazioni sugli strumenti che semplificano e semplificano gli acquisti e la gestione del software in Azure Marketplace.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 06/22/2021
ms.openlocfilehash: 0e79674825f8ab28fa4b0e68dd01c9c1b7e8c27a
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565186"
---
# <a name="azure-marketplace-purchasing"></a>Azure Marketplace acquisto

Azure Marketplace offre numerosi strumenti e funzionalità che semplificano e semplificano il processo di acquisto, fatturazione e gestione dei criteri di acquisto.

## <a name="simplified-procurement"></a>Approvvigionamento semplificato

Azure Marketplace semplifica di processo di approvvigionamento offrendo varie opzioni di acquisto. Se si acquistano prodotti usando una carta di credito associata all'account Azure, tutti gli acquisti verranno consolidati in una singola fattura e fatturati sulla carta di credito scelta. Se si è un cliente di grandi dimensioni, è possibile acquistare usando un Contratto Enterprise. Con un contratto EA, tutti gli acquisti di software vengono inclusi automaticamente nella fattura di Azure. che indicherà prima gli addebiti per l'utilizzo di Azure e quindi gli addebiti di Azure Marketplace.

Quando si acquista tramite Azure Marketplace, si elimina la complessità di gestione delle relazioni e delle fatture dei singoli fornitori. Si ottiene una singola fattura mensile consolidata da Microsoft che include sia gli Azure Marketplace e gli addebiti di Azure.

## <a name="permission-to-purchase"></a>Autorizzazione per l'acquisto

Dopo aver trovato l'applicazione software giusta, completare l'acquisto è semplice. Saranno tuttavia necessarie le autorizzazioni appropriate all'interno della sottoscrizione di Azure. Poiché Azure opera [](/azure/role-based-access-control/overview) su un modello di controllo degli accessi in base al ruolo, l'account deve avere le autorizzazioni di proprietario della sottoscrizione o **collaboratore** per effettuare un acquisto. 

Prima di completare un acquisto, assicurarsi che l'utente abbia la configurazione corretta nel tenant di Azure. Ciò consente di evitare errori durante l'acquisto.

Nell'Azure Marketplace nel portale di Azure trovare l'applicazione che si vuole acquistare e selezionare **Crea** o **Configura e sottoscrive**. Verrà richiesto di completare alcune informazioni prima di poter usare la nuova soluzione.

> [!CAUTION]
> L'approvazione nel Marketplace privato non indica l'approvvigionamento di una soluzione.

:::image type="content" source="media/overview/offer-create-screen.png" alt-text="Pulsante Crea offerta.":::

:::image type="content" source="media/overview/button-set-up-and-subscribe.png" alt-text="Pulsante Configura e sottoscrive.":::

Se si vuole distribuire una soluzione dal negozio online  Azure Marketplace, selezionare Scarica adesso nella pagina di descrizione del prodotto e quindi accedere con le credenziali dell'account Azure.

:::image type="content" source="media/overview/sign-in-to-azure-marketplace.png" alt-text="Finestra Azure Marketplace di accesso.":::

Dopo l'accesso, si verrà reindirizzati al prodotto nel portale di Azure per completare l'acquisto.

## <a name="purchase-policy-management"></a>Gestione dei criteri di acquisto

Microsoft consente di gestire gli acquisti degli utenti tramite il profilo di fatturazione come amministratore della sottoscrizione di Azure. Scegliere tra tre opzioni:

- **Gratuito e a pagamento:** consente agli utenti di acquisire qualsiasi Azure Marketplace software.
- **Gratuito:** consente agli utenti di distribuire solo software gratuito Azure Marketplace.
- **No:** impedisce agli utenti di distribuire software Azure Marketplace.

Queste impostazioni si applicano a tutti gli utenti con accesso alla sottoscrizione di Azure, che consente di controllare l'approvvigionamento IT tramite il portale di Azure.

:::image type="content" source="media/overview/billing-profile-policy-settings.png" alt-text="Controllo dell'approvvigionamento IT tramite portale di Azure.":::

## <a name="cost-management"></a>Gestione dei costi

Quando si acquistano prodotti da Azure Marketplace, si vogliono ottenere informazioni dettagliate che consentono di gestire i costi. Gestione costi di Azure è uno strumento gratuito per visualizzare informazioni sui prodotti acquistati. È possibile usare Gestione costi per visualizzare i dettagli sui servizi per i quali si spende denaro nel tempo e su come tenere traccia di tali costi rispetto ai budget impostati. Oltre a impostare i budget, è possibile pianificare report e analizzare i costi della sottoscrizione. Per altre informazioni Gestione costi di Azure, completare il modulo Microsoft Learn analizzare i costi e [creare budget con Gestione costi di Azure](/learn/modules/analyze-costs-create-budgets-azure-cost-management/).

È possibile visualizzare le fatture e gli addebiti di Azure Marketplace nello strumento di analisi dei costi disponibile in Gestione costi di Azure.

:::image type="content" source="media/overview/azure-cost-management.png" alt-text="Usare Gestione costi di Azure per ottenere informazioni dettagliate sui prodotti acquistati.":::

## <a name="purchase-validation-checks"></a>Controlli di convalida degli acquisti

L'acquisto di un'offerta Azure Marketplace può avere esito negativo per motivi diversi. È più probabile che l'uso dell'interfaccia della riga di comando per un acquisto possa causare errori perché è possibile che si stia tentando di acquistare un'offerta non disponibile o visibile in Azure Marketplace. Di seguito sono riportati i controlli che possono causare l'esito negativo di un acquisto:

1. La sottoscrizione appartiene a un Contratto Enterprise (EA) e l'amministratore EA ha disabilitato Azure Marketplace acquisti.
1. L'amministratore EA ha abilitato gli acquisti solo per le offerte gratuite e l'offerta è a pagamento.
1. L'offerta non è stata trovata nel marketplace.
1. Il fornitore di software indipendente (ISV) ha interrotto la vendita dell'offerta, almeno nella propria area.
1. La sottoscrizione in uso appartiene a un account di fatturazione in un'area in cui l'offerta non è disponibile.
1. L'account di sottoscrizione/fatturazione non è associato a uno strumento di pagamento valido, ad esempio una carta di credito valida.
1. La sottoscrizione appartiene a un Cloud Solution Provider (CSP) e l'ISV ha rifiutato di vendere tramite un CSP.
1. Il Marketplace privato è abilitato per la sottoscrizione e l'offerta non è presente nell'elenco delle offerte consentite.
1. L'offerta è Privata/Anteprima per clienti specifici e la sottoscrizione non è presente nell'elenco dei clienti consentiti.

L'acquisto di offerte del marketplace potrebbe non riuscire se è in conflitto Criteri di Azure definito dall'amministratore di Azure nell'organizzazione. Ad esempio, non è possibile acquistare Microsoft.SaaS se non  è presente nell'elenco di elementi consentiti dell'organizzazione. Per informazioni dettagliate, [vedere Criteri di Azure documentazione di](/azure/governance/policy/).

## <a name="next-steps"></a>Passaggi successivi

- [Fatturazione](billing-invoicing.md)