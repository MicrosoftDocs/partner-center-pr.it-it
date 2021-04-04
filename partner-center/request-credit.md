---
title: Richiedere crediti del contratto di servizio a Microsoft
ms.topic: article
ms.date: 03/31/2021
description: Scopri i vantaggi, le restrizioni e le procedure per richiedere un credito di contratto di servizio (SLA) a Microsoft qualora i clienti dovessero riscontrare un'interruzione del servizio.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: d33188510b127873864260199ff92018e1a4d995
ms.sourcegitcommit: 766b2bb46dffd29e532b42106359f83e51b96700
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/31/2021
ms.locfileid: "106103826"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a>Come e quando richiedere un contratto di servizio (SLA) a livello di servizio da Microsoft

È possibile richiedere crediti con **contratto di servizio (SLA)** di Microsoft se un servizio fornito per i clienti presenta un'interruzione.

## <a name="sla-credit-calculation"></a>Calcolo del credito SLA

I crediti del contratto di servizio di Microsoft vengono determinati in base ai servizi interessati. Se ad esempio il cliente ha una suite Office 365 ma si è verificata un'interruzione di SharePoint, il credito del contratto di servizio viene approvato solo per SharePoint e non per l'intero piano del cliente.

*I crediti sono pro-rated in base al servizio interessato e alla durata dell'interruzione.* Per visualizzare i tipi di scenari idonei per i crediti del contratto di servizio, vedere il [documento contratto di servizio consolidato per i servizi online](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37). Queste informazioni si applicano anche ai servizi venduti tramite il programma Cloud Solution Provider.


## <a name="request-an-sla-credit"></a>Richiedi un credito del contratto di contratto

*Il partner Cloud Solution Provider (CSP) deve inviare l'attestazione e tutte le informazioni necessarie entro la fine del mese di calendario dopo il mese in cui si è verificato l'evento imprevisto.* Se, ad esempio, l'evento imprevisto si è verificato il 15 febbraio, Microsoft deve ricevere l'attestazione e tutte le informazioni necessarie entro il 31 marzo. I clienti finali e i rivenditori indiretti non possono inviare attestazioni di credito del contratto di contratto; il provider indiretto o il partner Direct Bill deve inviare attestazioni per loro conto.

>[!NOTE]
>Gli eventi imprevisti consultivi ([come controllare Microsoft 365 integrità del servizio](https://docs.microsoft.com/microsoft-365/enterprise/view-service-health?&preserve-view=trueo365-worldwide#incidents-and-advisories)) non sono idonei per i crediti del contratto di servizio.

### <a name="required-information"></a>Informazioni necessarie

Il nome del cliente, l'identificatore del tenant, il ticket del partner n e l'indicatore di data e ora creati dal ticket non sono sufficienti per l'elaborazione di un'attestazione.

Prima di [inviare una richiesta di credito del contratto](#submit-sla-credit-request) di servizio a Microsoft, è necessario raccogliere **tutte** le informazioni seguenti da includere nel ticket di supporto:

- GUID del tenant del cliente
- [Identificatore dell'evento imprevisto di interruzione](#outage-incident-identifier)?
- Prova che il cliente è stato influenzato dall'interruzione e ha richiesto un credito del contratto di servizio.
- Le sottoscrizioni interessate sono state acquistate tramite CSP? (*Sì* o *No*)

#### <a name="evidence-that-proves-customer-impact"></a>Prove che dimostrano l'effetto del cliente

- Informazioni riguardanti l'ora e la durata del tempo di inattività
- Il numero e la posizione degli utenti interessati (se applicabile)
- Descrizioni dei tentativi di risoluzione dell'evento imprevisto al momento dell'occorrenza
- Un messaggio di posta elettronica dal cliente interessato che richiede supporto e successivamente credito
- Il numero di ticket di supporto e i dettagli del contatto del cliente in merito alla risoluzione dell'effetto sul servizio


#### <a name="outage-incident-identifier"></a>ID evento di interruzione

È possibile trovare l'identificatore per l'evento imprevisto di interruzione nella pagina **integrità del servizio** nell'interfaccia di amministrazione di Microsoft 365. L' **ID evento imprevisto di interruzione** è un numero preceduto da un'abbreviazione di due lettere che indica il servizio interessato (ad esempio, *EX25194* per un'interruzione di Exchange Online). La tabella seguente descrive le abbreviazioni di servizio comuni:

| Abbreviazione di due lettere | Servizio Microsoft |
| ----------------------- | ----------------- |
| EX | Exchange Online |
| FO | Protezione di Exchange Online |
| SB | Skype for business online (in precedenza Lync Online) |
| OS | Sottoscrizione a Office |
| PB | Power BI per Office 365 |
| SP | SharePoint Online |
| YA | Yammer Enterprise |
| MO | Errore del portale |

### <a name="submit-sla-credit-request"></a>Invia richiesta di credito del contratto di contratto

Per inviare la richiesta di credito del contratto di lavoro a Microsoft tramite il dashboard del centro per i partner:

1. Accedere al dashboard Centro per i partner.
2. Nel menu a sinistra scegliere **richieste di servizio**, quindi selezionare richieste di **supporto** per i partner.
3. Nella pagina **richiesta partner** scegliere **nuova richiesta**.
4. Nella pagina **Avvia richiesta** trovare la sezione **CSP-Customers, Orders and subscriptions**. In questa sezione scegliere **selezionare un tipo di problema**, quindi selezionare **Customer Services requests Credit requests**.
5. Nella pagina **soluzioni consigliate** , in sono **necessarie altre informazioni?**, scegliere **Sì**.
6. Nella pagina **Dettagli** compilare la sezione **Dettagli problema** . Nella casella di testo **Dettagli** assicurarsi di immettere le [informazioni necessarie](#required-information) raccolte in precedenza.
7. Scegliere **Invia** per inviare la richiesta di credito del contratto di contratto.

## <a name="next-steps"></a>Passaggi successivi

- [Segnala i problemi per conto del cliente](report-problems-on-behalf-of-a-customer.md)
