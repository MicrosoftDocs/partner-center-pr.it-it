---
title: Richiedere crediti del contratto di servizio a Microsoft
ms.topic: article
ms.date: 03/31/2021
description: Informazioni su vantaggi, restrizioni e procedure per richiedere un credito del contratto di servizio a Microsoft in caso di interruzione del servizio da parte dei clienti.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 3a0bb85143efe3d4135b56985b9a04e2dbe5e4cc
ms.sourcegitcommit: 57442bbbef15a70bd9a042642140cbf2c8608b09
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/09/2021
ms.locfileid: "113519447"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a>Come e quando richiedere un credito del contratto di servizio a Microsoft

**Ruoli appropriati:** agente di amministrazione | Amministratore globale

È possibile richiedere **crediti del contratto** di servizio a Microsoft se si verifica un'interruzione del servizio fornito per i clienti.

## <a name="sla-credit-calculation"></a>Calcolo del credito del contratto di servizio

I crediti del contratto di servizio di Microsoft vengono determinati in base ai servizi che sono stati influenzati. Ad esempio, se il cliente ha una suite Office 365 ma ha riscontrato solo un'interruzione del SharePoint, il credito del contratto di servizio viene approvato solo per SharePoint e non per l'intero piano del cliente.

*I crediti vengono valutati in base al servizio interessato e alla durata dell'interruzione.* Per visualizzare i tipi di scenari idonei per i crediti del contratto di servizio, vedere il documento Contratto di [servizio consolidato di Online Services.](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37) Queste informazioni si applicano anche ai servizi venduti tramite Cloud Solution Provider (CSP).


## <a name="request-an-sla-credit"></a>Richiedere un credito per il contratto di servizio

*Il partner CSP deve inviare l'attestazione e tutte le informazioni necessarie entro la fine del mese di calendario successivo al mese in cui si è verificato l'evento imprevisto.* Ad esempio, se l'evento imprevisto si è verificato il 15 febbraio, Microsoft deve ricevere l'attestazione e tutte le informazioni necessarie entro il 31 marzo. I clienti finali e i rivenditori indiretti non possono inviare richieste di credito del contratto di servizio; Il provider indiretto o il partner con fatturazione diretta deve inviare attestazioni per loro conto.

> [!NOTE]
> Gli eventi imprevisti di consulenza non sono in genere idonei per i crediti del contratto di servizio. Un evento imprevisto pubblicato nel dashboard di integrità dei servizi indica che un *tenant* può essere inciso e rappresenta le informazioni migliori di Microsoft al momento della pubblicazione. I dati della pagina integrità rappresentano la disponibilità generale di un servizio. L'impatto, la mitigazione e la risoluzione dei singoli servizi possono variare. Per altri dettagli, è possibile esaminare il post di evento imprevisto finale e la revisione post-evento imprevisto. Per [altre informazioni, vedere Come Microsoft 365'integrità](/microsoft-365/enterprise/view-service-health#incidents-and-advisories) del servizio.

### <a name="required-information"></a>Informazioni necessarie

Il nome del cliente, l'identificatore del tenant, il ticket partner# e il timestamp di data/ora di creazione del ticket non sono sufficienti per l'elaborazione di un'attestazione.

Prima di [inviare una richiesta di credito del](#submit-sla-credit-request) contratto di servizio a Microsoft, è necessario raccogliere tutte le informazioni seguenti da includere nel ticket di supporto: 

- GUID del tenant del cliente
- Identificatore [dell'evento imprevisto di interruzione?](#outage-incident-identifier)
- Prova che il cliente è stato in impatto dall'interruzione del servizio e ha richiesto un credito del contratto di servizio.
- Le sottoscrizioni ermesse sono state acquistate tramite CSP? (*sì* o *no*)

#### <a name="evidence-that-proves-customer-impact"></a>Evidenza che dimostra l'impatto dei clienti

- Informazioni relative al tempo e alla durata del tempo di inattività
- Numero e località degli utenti interessati (se applicabile)
- Descrizioni dei tentativi di risolvere l'evento imprevisto al momento dell'occorrenza
- Un messaggio di posta elettronica dal cliente che ha richiesto supporto e successivamente il credito
- Numero del ticket di supporto e dettagli del contatto del cliente per la risoluzione dell'impatto del servizio


#### <a name="outage-incident-identifier"></a>Identificatore dell'evento imprevisto di interruzione

È possibile trovare l'identificatore per l'evento imprevisto di interruzione **nella** pagina Integrità dei servizi nel interfaccia di amministrazione di Microsoft 365. L'ID evento **imprevisto** di interruzione è un numero preceduto da un'abbreviazione di due lettere che indica il servizio interessato, ad esempio *EX25194* per un'interruzione Exchange Online servizio. La tabella seguente descrive le abbreviazioni di servizi comuni:

| Abbreviazione di due lettere | Servizio Microsoft |
| ----------------------- | ----------------- |
| EX | Exchange Online |
| FO | Exchange Online Protection |
| SB | Skype for Business Online (in precedenza Lync Online) |
| OS | Sottoscrizione a Office |
| PB | Power BI per Office 365 |
| SP | SharePoint Online |
| Ya | Yammer Enterprise |
| MO | Errore del portale |

### <a name="submit-sla-credit-request"></a>Inviare la richiesta di credito del contratto di servizio

Per inviare la richiesta di credito del contratto di servizio a Microsoft tramite il dashboard Partner Center:

1. Accedere al dashboard Centro per i partner.
2. Nel menu a sinistra scegliere Richieste di servizio **e** quindi selezionare Richieste di **supporto partner.**
3. Nella pagina **Richiesta partner** scegliere **Nuova richiesta.**
4. Nella pagina **Avvia la richiesta** individuare la sezione **CSP - clienti, ordini e sottoscrizioni**. In questa sezione scegliere Selezionare un **tipo di problema e** quindi selezionare Richieste di credito per i servizi **clienti.**
5. Nella pagina **Soluzioni consigliate,** in **Servono altre informazioni?**, scegliere **Sì.**
6. Nella pagina **Dettagli** compilare la sezione **Dettagli** problema. Nella casella **di** testo Dettagli assicurarsi di immettere le [informazioni necessarie](#required-information) raccolte in precedenza.
7. Scegliere **Invia per** inviare la richiesta di credito del contratto di servizio.

## <a name="next-steps"></a>Passaggi successivi

- [Segnalare problemi per conto del cliente](report-problems-on-behalf-of-a-customer.md)
