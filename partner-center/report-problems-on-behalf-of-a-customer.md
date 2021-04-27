---
title: Segnalare problemi per conto di un cliente
ms.topic: how-to
ms.date: 02/26/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su quando inoltrare un problema del servizio clienti a Microsoft e su come determinare un ticket di supporto per diversi tipi di servizi Microsoft.
author: Kim-Davis
ms.author: kimnich
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f67a3b6a403f09cb773a5ca663d6cf6db1b03e2e
ms.sourcegitcommit: efd711b0e65c55f24ce5b9636abd7b5a8cc719fe
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/27/2021
ms.locfileid: "108018119"
---
# <a name="report-a-service-problem-on-behalf-of-a-customer---including-when-and-how-to-do-so"></a>Segnalare un problema di servizio per conto di un cliente, incluso quando e come eseguire questa operazione

**Si applica a**

- Centro per i partner per Microsoft Cloud for US Government

**Ruoli appropriati**

- Amministratore globale

Se il cliente riscontra un problema di servizio che non è possibile risolvere e soddisfa i criteri descritti in Escalation dei problemi a [Microsoft,](escalate-problems-to-microsoft.md)il provider indiretto può determinare un ticket di supporto. Questo processo è utile anche per inoltrare problemi o controversie correlati alla fatturazione e segnalare possibili frodi.

## <a name="submit-a-service-request-for-a-customer"></a>Inviare una richiesta di servizio per un cliente

1. Nel menu Partner Center sotto CSP selezionare **Clienti**

2. Nella pagina Clienti selezionare o cercare il cliente desiderato
    
3. Dal menu del cliente selezionare **Richieste di servizio**

4. Dal menu a discesa **Nuova richiesta** scegli **Azure** o **Office 365, Dynamics 365, Enterprise Mobility Suite**. Si verrà reindirizzati all'interfaccia di portale di Microsoft Azure o all'interfaccia di amministrazione di Office 365.

>[!NOTE]
>Per mantenere un contratto di supporto con piano ASfP (Advanced Support for Partner) o versione successiva, è necessario che i partner delle operazioni di supporto eseere transazionali di Dynamics 365 in CSP. Questo contratto di supporto è necessario per inviare eventi imprevisti di Dynamics 365 per conto di un cliente CSP. [Altre informazioni sulle](https://partner.microsoft.com/support/partnersupport) opzioni del contratto di supporto.

### <a name="microsoft-azure"></a>Microsoft Azure

> [!IMPORTANT]
> Quando devi creare una richiesta di servizio per il cliente in Azure, tieni presente quanto segue:
>
>- Per consentire al rivenditore indiretto di creare richieste di servizio per il cliente in Azure, il provider indiretto deve concedere l'accesso all'account Azure del cliente. Questa operazione è diversa dall'amministrazione per conto dei clienti per Office 365.
>
>- Sebbene l'amministratore di supporto tecnico nel Centro per i partner non possa creare richieste di servizio nel portale dei servizi di Azure, può creare un gruppo di supporto nel portale e assegnare a tale gruppo le autorizzazioni per registrare le richieste di supporto.

1. Selezionare **Nuova richiesta di supporto**.

2. Compila la richiesta di supporto con le informazioni appropriate e quindi seleziona **Crea**:

   - Nella sezione **Nozioni di base** della richiesta di supporto assicurati di aver selezionato **Cloud Solution Provider** nel campo **Piano di supporto**.

   - Nella sezione informativa **Contatto** della richiesta di supporto immetti le tue informazioni e non quelle del cliente.

3. Successivamente, esaminare le richieste di servizio del cliente all'interno del portale di Microsoft Azure selezionando **Gestisci richieste di supporto**.

Potrebbe essere necessario creare una richiesta di supporto per un cliente quando non si dispone delle autorizzazioni di amministratore per tale cliente. Ciò potrebbe verificarsi in questi due scenari:

- Non sono stati necessari privilegi di amministratore quando è stata stabilita la relazione per la prima volta.
- Si gestiscono solo le sottoscrizioni di Azure di un cliente, quindi non si hanno autorizzazioni amministrative.
 
In entrambi i casi, puoi usare la procedura seguente per creare una richiesta di supporto. 

1. Copiare il nome di dominio del cliente dalla pagina dell'account in Partner Center.

2. Passa a https://portal.azure.com/[nomedominiocliente]. 

3. Seleziona la sottoscrizione di Azure che richiede supporto.

4. Seleziona **Nuova richiesta di supporto** e quindi segui i prompt per creare la richiesta. 

 
### <a name="office-365-microsoft-dynamics-crm-online-enterprise-mobility-suite"></a>Office 365, Microsoft Dynamics CRM Online, Enterprise Mobility Suite

1. Nella sezione **Crea una richiesta di servizio** scegliere la categoria di supporto appropriata. Potrebbe essere necessario selezionare **Altro...** per visualizzare altri articoli.

2. Compila il modulo della richiesta di servizio e seleziona **Invia**.

   > [!TIP]
   > Assicurati di includere le tue informazioni di contatto e non quelle del cliente.

3. Successivamente, esaminare le richieste di servizio del cliente andando all'interfaccia di amministrazione di Office 365 e selezionando **Visualizza tutti i ticket di supporto.**

### <a name="support-for-commercial-marketplace-products"></a>Supporto per prodotti del Marketplace commerciale

Microsoft non fornisce supporto tecnico per i prodotti del marketplace commerciale. Per ottenere supporto, è necessario contattare il fornitore di software indipendente (ISV) che ha pubblicato il prodotto.

Per trovare le informazioni di contatto dell'ISV:

1.  Nella pagina **Marketplace** seleziona il prodotto per cui è necessaria assistenza.

2.  Nella pagina del prodotto sono possibile trovare le informazioni di contatto del supporto tecnico. Può trattarsi di una o più delle opzioni seguenti:

    - Un collegamento a un punto di ingresso del supporto tecnico nel sito Web dell'ISV
    - Un indirizzo di posta elettronica del supporto tecnico
    - Un numero di telefono per contattare il supporto tecnico

## <a name="faq"></a>Domande frequenti

Vedere le domande frequenti seguenti sulle richieste di servizio che è possibile inviare per conto di un cliente. 

### <a name="what-is-included-as-part-of-the-support-entitlement"></a>Cosa include il diritto al supporto?

Le richieste di servizio devono essere inviate tramite Partner Center. Sono disponibili per Azure, Microsoft Office 365, Microsoft Dynamics CRM Online ed Enterprise Mobility Suite. Un partner che partecipa al programma Cloud Solution Provider avrà tempi di risposta prioritari per i problemi più gravi.

Il supporto per il tenant partner non è incluso come parte del vantaggio del supporto CSP. Tuttavia, Office 365, Microsoft Dynamics CRM Online ed Enterprise Mobility Suite non addebita una tariffa di sottoscrizione di supporto separata per partner o clienti. Azure addebita una tariffa, ma se si ha diritto a Signature Cloud Support o ad altri vantaggi di Microsoft Partner Network (MPN), è possibile usare questi vantaggi per pagare tale tariffa.

Questo vantaggio si applica a tutti i partner che partecipano al programma Cloud Solution Provider, a pagamento o durante un periodo di valutazione. Il supporto per la gestione di fatturazione e sottoscrizioni è anch'esso incluso come componente gratuito di questo pacchetto.

### <a name="how-quickly-will-i-get-an-initial-response"></a>Quanto tempo serve per avere la risposta iniziale?

I tempi per la risposta iniziale dipendono dalla gravità del problema. La gravità di un problema è determinata dall'impatto aziendale indicato quando invii una richiesta di servizio.

Tempi di risposta iniziali per **gli eventi imprevisti di interruzione tecnica:**

- Impatto critico (gravità A): due ore (perdita significativa o riduzione delle prestazioni dei servizi. Servizi di produzione non funzionanti).
- Impatto moderato (gravità B): quattro ore (perdita moderata o riduzione delle prestazioni dei servizi. Servizi di produzione parzialmente interessati.
- Impatto minimo (gravità C): otto ore (perdita minima o riduzione delle prestazioni dei servizi. Servizi ancora disponibili o non di produzione interessati.

I tempi per la risposta iniziale si riferiscono solo al supporto in lingua inglese. Il supporto nella lingua locale viene fornito durante l'orario di ufficio.
Per gli eventi imprevisti che rientrano nei limiti del diritto di supporto, ma non sono considerati eventi imprevisti di correzione, il tempo di risposta iniziale può essere fino a un giorno lavorativo.

### <a name="can-i-submit-a-service-request-by-phone"></a>Posso inviare una richiesta di servizio per telefono?

No, il supporto telefonico non è disponibile per questo programma.

### <a name="what-happens-if-i-sign-into-the-azure-portal-and-bypass-partner-center"></a>Cosa succede se accedo al portale di Azure senza usare il Centro per i partner?

Se si accede direttamente al portale di Microsoft Azure, si sta visualizzando il centro nel proprio contesto, non nel contesto di un cliente. Questo è il motivo per cui è consigliabile accedere direttamente al portale di Microsoft Azure quando si crea una richiesta di servizio per le proprie sottoscrizioni.

L'entitlement per il supporto del programma CSP non fornisce supporto per la sottoscrizione partner. Per questo problema, è necessario fornire l'entitlement valido per il piano di supporto quando si crea una richiesta di servizio che riguarda la propria sottoscrizione partner. Ad esempio, l'ID contratto MPN, premier o un supporto tecnico di Azure aziendale. Per altre informazioni, vedere le domande [supporto di Azure seguenti.](https://go.microsoft.com/fwlink/?LinkId=717532)

### <a name="what-happens-if-i-sign-into-the-office-365-admin-center-portal-and-bypass-partner-center"></a>Cosa accade se si accede al portale dell'interfaccia di amministrazione di Office 365 e si ignora Partner Center?

Se si accede direttamente all'interfaccia di amministrazione di Office 365, si sta visualizzando il centro nel proprio contesto, non nel contesto di un cliente. Per questo motivo è consigliabile accedere direttamente all'interfaccia di amministrazione di Office 365 solo quando si crea una richiesta di servizio per le proprie sottoscrizioni.

### <a name="how-do-i-get-additional-dynamics-365-support"></a>Come posso ottenere ulteriore supporto per Dynamics 365?

Se si verificano problemi relativi a: Sottoscrizioni del piano Dynamics 365, Licenze, Fatturazione, Finance & Operations, licenze del prodotto Dynamics 365 o se è necessario ulteriore supporto tecnico:
 
contatta il [supporto Dynamics](/dynamics365/customer-engagement/admin/contact-technical-support)

## <a name="next-steps"></a>Passaggi successivi

- [Fornire supporto ai clienti](customer-support.md)
- [Controllare l'integrità del servizio](check-service-health.md)
