---
title: Segnalare problemi per conto di un cliente
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Scopri quando inoltrare un problema al servizio clienti a Microsoft e come archiviare un ticket di supporto.
author: Kim-Davis
ms.author: kimnich
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7dda38680bd698ce04149ed8c1a9acf1cff0ba2f
ms.sourcegitcommit: 7a749e7130f903b2d94cfa44e14bde0adf7ee199
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/24/2020
ms.locfileid: "88781833"
---
# <a name="report-a-service-problem-on-behalf-of-a-customer---including-when-and-how-to-do-so"></a>Segnala un problema del servizio per conto di un cliente, incluse le attività e le modalità di esecuzione

**Si applica a**

- Centro per i partner
- Centro per i partner per Microsoft Cloud for US Government

**Ruoli appropriati**

- Provider indiretto

Se il cliente riscontra un problema del servizio che non è possibile risolvere e soddisfa i criteri descritti in [inoltrare i problemi a Microsoft](escalate-problems-to-microsoft.md), il provider indiretto può archiviare un ticket di supporto. Questo processo è utile anche per inoltrare problemi o controversie correlati alla fatturazione e segnalare possibili frodi.

## <a name="submit-a-service-request-for-a-customer"></a>Inviare una richiesta di servizio per un cliente

1. Dal menu **Centro per i partner** scegli **Richieste di servizio** e quindi **Richieste clienti**. 

2. Nella pagina Richieste clienti cerca il cliente desiderato.

3. Dal menu a discesa **Nuova richiesta** scegli **Azure** o **Office 365, Dynamics 365, Enterprise Mobility Suite**. Si verrà reindirizzati al portale di Microsoft Azure o all'interfaccia di amministrazione di Office 365.

>[!NOTE]
>I partner operativi di supporto per la transazione di Dynamics 365 in CSP sono necessari per mantenere un contratto di supporto del piano di supporto avanzato per i partner (ASfP) o superiore. Questo contratto di supporto è necessario per inviare eventi imprevisti di Dynamics 365 per conto di un cliente CSP. [Altre](https://partner.microsoft.com/support/partnersupport) informazioni sulle opzioni del contratto di supporto.

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

Se non si dispone delle autorizzazioni di amministratore per il cliente, potrebbe essere necessario creare una richiesta di supporto per un cliente. Ciò potrebbe verificarsi in questi due scenari:

- Non sono stati richiesti privilegi di amministratore quando la relazione è stata stabilita per la prima volta.
- È possibile gestire solo le sottoscrizioni di Azure di un cliente, in modo che non si disponga delle autorizzazioni amministrative.
 
In entrambi i casi, puoi usare la procedura seguente per creare una richiesta di supporto. 

1. Copiare il nome di dominio del cliente dalla pagina relativa all'account nel centro per i partner.

2. Passa a https://portal.azure.com/[nomedominiocliente]. 

3. Seleziona la sottoscrizione di Azure che richiede supporto.

4. Seleziona **Nuova richiesta di supporto** e quindi segui i prompt per creare la richiesta. 

 
### <a name="office-365-microsoft-dynamics-crm-online-enterprise-mobility-suite"></a>Office 365, Microsoft Dynamics CRM Online, Enterprise Mobility Suite

1. Nella sezione **creare una richiesta di servizio** scegliere la categoria di supporto appropriata. Per visualizzare altri articoli, potrebbe essere necessario selezionare **altro...** .

2. Compila il modulo della richiesta di servizio e seleziona **Invia**.

   > [!TIP]
   > Assicurati di includere le tue informazioni di contatto e non quelle del cliente.

3. In seguito, rivedere le richieste di assistenza del cliente accedendo all'interfaccia di amministrazione di Office 365 e selezionando **Visualizza tutti i ticket di supporto**.

### <a name="support-for-commercial-marketplace-products"></a>Supporto per prodotti del Marketplace commerciale

Microsoft non fornisce il supporto tecnico per i prodotti commerciali del Marketplace. È necessario contattare il fornitore di software indipendente (ISV) che ha pubblicato il prodotto per ottenere supporto.

Per trovare le informazioni di contatto dell'ISV:

1.  Nella pagina**Marketplace** seleziona il prodotto per cui è necessaria assistenza.

2.  Nella pagina del prodotto sono disponibili informazioni di contatto per il supporto. Può trattarsi di una o più delle opzioni seguenti:

    - Un collegamento a un punto di ingresso del supporto tecnico nel sito Web dell'ISV
    - Un indirizzo di posta elettronica del supporto tecnico
    - Un numero di telefono per contattare il supporto tecnico

## <a name="faq"></a>Domande frequenti

**Cosa include il diritto al supporto?**

Le richieste di servizio devono essere presentate tramite il centro per i partner. Sono disponibili per Azure, Microsoft Office 365, Microsoft Dynamics CRM online ed Enterprise Mobility Suite. Un partner che partecipa al programma Cloud Solution Provider avrà tempi di risposta prioritari per i problemi più gravi.

Il supporto per il proprio tenant partner non è incluso nell'ambito del vantaggio del supporto CSP. Tuttavia, Office 365, Microsoft Dynamics CRM online ed Enterprise Mobility Suite non addebitano una tariffa di sottoscrizione di supporto separata per partner o clienti. Azure applica una tariffa, ma se si ha diritto a firmare il supporto cloud o altri vantaggi di Microsoft Partner Network (MPN), è possibile usarli per pagare la tariffa.

Questo vantaggio si applica a tutti i partner che partecipano al programma Cloud Solution Provider, a pagamento o durante un periodo di valutazione. Il supporto per la gestione di fatturazione e sottoscrizioni è anch'esso incluso come componente gratuito di questo pacchetto.

**Quanto tempo serve per avere la risposta iniziale?**

I tempi per la risposta iniziale dipendono dalla gravità del problema. La gravità di un problema è determinata dall'impatto aziendale indicato quando invii una richiesta di servizio.

Tempi di risposta iniziali per gli **eventi imprevisti di correzione tecnico**:

- Impatto critico (gravità A): 2 ore (perdita o riduzione delle prestazioni dei servizi significativa. Servizi di produzione non funzionanti).
- Effetto moderato (gravità B): quattro ore (perdita moderata o riduzione dei servizi. Servizi di produzione interessati parzialmente.
- Effetto minimo (gravità C): otto ore (perdita minima o riduzione dei servizi. Servizi ancora disponibili o servizi non di produzione interessati.

I tempi per la risposta iniziale si riferiscono solo al supporto in lingua inglese. Il supporto nella lingua locale viene fornito durante l'orario di ufficio.
Per gli eventi imprevisti che rientrano nei limiti del diritto di supporto ma che non sono considerati interventi di correzione, il tempo di risposta iniziale potrebbe essere fino a un giorno lavorativo.

**Posso inviare telefonicamente una richiesta di servizio?**

No, il supporto telefonico non è disponibile per questo programma.

**Cosa succede se accedo al portale di Azure senza usare il Centro per i partner?**

Se si accede direttamente al portale di Microsoft Azure, si sta visualizzando il centro nel proprio contesto, non nel contesto di un cliente. Per questo motivo, è consigliabile accedere direttamente al portale di Microsoft Azure quando si crea una richiesta di servizio per le proprie sottoscrizioni.

Il diritto del supporto del programma CSP non fornisce supporto per la sottoscrizione del partner. Per questo motivo, è necessario fornire il diritto valido del piano di supporto quando si crea una richiesta di servizio che riguarda la sottoscrizione del partner. Gli esempi includono ID contratto MPN, Premier o un piano di supporto di Azure. Per ulteriori informazioni, vedere le [domande frequenti sul supporto tecnico di Azure](https://go.microsoft.com/fwlink/?LinkId=717532).

**Cosa accade se si accede al portale dell'interfaccia di amministrazione di Office 365 e si ignora il centro per i partner?**

Se si accede direttamente all'interfaccia di amministrazione di Office 365, si sta visualizzando il centro nel proprio contesto, non nel contesto di un cliente. Per questo motivo, è consigliabile accedere direttamente all'interfaccia di amministrazione di Office 365 quando si crea una richiesta di servizio per le proprie sottoscrizioni.

**Come posso ottenere ulteriore supporto per Dynamics 365?**

Se si verificano problemi relativi a: sottoscrizioni del piano Dynamics 365, licenze, fatturazione, operazioni di & finanza, licenze del prodotto Dynamics 365 oppure è necessario ulteriore supporto tecnico:
 
contatta il [supporto Dynamics](https://docs.microsoft.com/dynamics365/customer-engagement/admin/contact-technical-support)

leggi l'argomento relativo al [supporto di Microsoft Dynamics](https://support.microsoft.com/help/4052881/faq-microsoft-dynamics-365-for-unified-operations-iur)

## <a name="next-steps"></a>Passaggi successivi

- [Fornire supporto ai clienti](customer-support.md)
- [Controllare l'integrità del servizio](check-service-health.md)
