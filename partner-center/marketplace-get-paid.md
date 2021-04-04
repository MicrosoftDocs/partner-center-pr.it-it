---
title: Pagamento nel centro per i partner
description: Scopri come ricevere i pagamenti per i guadagni come partner Microsoft, ad esempio tramite offerte per Marketplace commerciali, programmi incentive e il programma Cloud Solution Provider. Include i criteri di pagamento, lo stato dei pagamenti e le istruzioni di pagamento.
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.topic: conceptual
ms.date: 11/25/2020
author: eunjkim520
ms.author: eunjkim
ms.openlocfilehash: 94ed17106b64b078c51de351d1e44e29d3745921
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/01/2021
ms.locfileid: "106133081"
---
# <a name="getting-paid-in-partner-center"></a>Pagamento nel centro per i partner

**Ruoli appropriati**

- Amministratore degli account
- Amministratore globale

Questo articolo contiene informazioni importanti su come ricevere pagamenti per le offerte, i componenti aggiuntivi e i guadagni pubblicitari. Vengono riepilogati i criteri di pagamento, i passaggi necessari prima di ricevere il pagamento e la panoramica delle istruzioni di pagamento.

## <a name="payout-policies-and-agreements"></a>Criteri di pagamento e contratti

Per ricevere i pagamenti, è necessario rispettare i contratti e i criteri di pagamento.

- [Microsoft Azure Marketplace contratto di pubblicazione](https://go.microsoft.com/fwlink/p/?LinkID=699560): prima di ricevere il pagamento, è necessario accettare il contratto di pubblicazione. Il presente contratto spiega la relazione tra l'utente e Microsoft, in quanto riguarda le offerte del venditore nel Marketplace commerciale, inclusa la tariffa del negozio addebitata da Microsoft per ogni vendita effettuata.
- Il [criterio](payout-policy-details.md) di pagamento Mostra i criteri di pagamento pagamenti, inclusi i metodi di pagamento e la pianificazione dei pagamenti. Il criterio spiega anche il processo per i pagamenti non effettuati dai clienti.
- I [Dettagli delle](tax-details-marketplace.md) imposte illustrano la considerazione fiscale per la selezione dei prezzi e la responsabilità fiscale nel [Contratto Microsoft Publisher](https://go.microsoft.com/fwlink/p/?LinkID=699560).
- Le **tariffe di archiviazione** sono definite ufficialmente nel contratto di pubblicazione. La tariffa di archiviazione viene applicata a tutte le vendite di offerte raccolte dal Marketplace commerciale, inclusi i componenti aggiuntivi.
- I **pagamenti** vengono effettuati su base mensile (purché sia stata soddisfatta la soglia di pagamento). In genere si inviano pagamenti a causa di un determinato mese entro il 15 ° giorno del mese. I pagamenti in genere importano da 3 a 10 giorni lavorativi aggiuntivi per raggiungere l'account di pagamento. Per informazioni dettagliate, vedere [Soglie, metodi e intervalli di pagamento](payment-thresholds-methods-timeframes.md).

## <a name="prerequisite-steps-before-getting-paid"></a>Passaggi prerequisiti prima di ricevere il pagamento

Prima di ricevere il pagamento per la prima volta, è necessario configurare l'account di pagamento e completare i moduli di Bank and Tax necessari. Nei moduli Bank e Tax, si forniranno i metodi di pagamento preferiti e le forme fiscali per la ritenuta delle imposte. I moduli Bank e Tax sono necessari prima di poter pagare l'utente. Per informazioni dettagliate, vedere [configurare l'account di pagamento e i moduli fiscali](set-up-your-payout-account.md).

### <a name="payout-hold-status"></a>Stato di blocco dei pagamenti

Per impostazione predefinita, i pagamenti verranno corrisposti su base mensile, come descritto sopra. Tuttavia, è possibile mettere in attesa i pagamenti per un programma e Microsoft non rilascerà i pagamenti al proprio account. Se si sceglie di mettere in attesa i pagamenti, si continuerà a registrare eventuali guadagni nella pagina dei **pagamenti** . Non verranno tuttavia inviati pagamenti all'account fino a quando non sarà rimosso il blocco.

Per inserire i pagamenti in attesa, selezionare l'icona dell'ingranaggio **Impostazioni** in alto a destra, quindi **Impostazioni account**. Selezionare **pagamenti e imposte** nel menu a sinistra e nella sezione **assegnazione profilo di pagamento e imposta** individuare il programma per il quale si desidera che vengano mantenuti i pagamenti. Selezionare la casella di controllo **Mantieni il pagamento** per mantenere i pagamenti per il programma. È possibile modificare lo stato di mantenimento dei pagamenti in qualsiasi momento, ma la decisione influirà sul pagamento mensile successivo. Se ad esempio si vuole bloccare il pagamento di aprile, assicurarsi di impostare lo stato di blocco dei pagamenti su **Sì** entro la fine di marzo.

Dopo aver impostato lo **stato di mantenimento** dei pagamenti **su on**, tutti i pagamenti per il programma saranno in attesa finché la casella di controllo non verrà deselezionata. Quando si esegue questa operazione, si verrà inclusi durante il successivo ciclo di pagamento mensile (purché sia stata soddisfatta la soglia di pagamento). Se i pagamenti sono in attesa, ma si vuole che venga generato un pagamento in giugno, deselezionare la casella di **controllo prima della** fine di maggio.

>[!Note]
> Lo stato di mantenimento dei pagamenti si applica a ogni programma individualmente (Microsoft Store, Advertising, Azure Marketplace e così via). Se si desidera mantenere i pagamenti per tutti i programmi, effettuare il pagamento in ogni programma individualmente.

## <a name="payout-statements"></a>Estratti conto

L'istruzione di pagamento Mostra i guadagni delle vendite delle offerte e dei componenti aggiuntivi nella cronologia delle transazioni. È anche possibile visualizzare i dettagli di pagamento e scaricare i report in formato TSV o CSV. Per ulteriori informazioni su come accedere al rendiconto dei pagamenti e sui dettagli relativi alla cronologia delle transazioni e ai report sui pagamenti, vedere la pagina relativa alle [istruzioni](payout-statement.md) per i pagamenti. Inoltre, è possibile utilizzare l' [API](https://apidocs.microsoft.com/services/partnerpayouts) per i pagamenti dei partner per effettuare sistematicamente il pull dei report sui pagamenti.

## <a name="next-steps"></a>Passaggi successivi

- [API per i pagamenti partner](https://apidocs.microsoft.com/services/partnerpayouts)
- [Domande frequenti su Proventi](payout-faq.md)
