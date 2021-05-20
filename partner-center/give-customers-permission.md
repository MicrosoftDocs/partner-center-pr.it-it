---
title: Consentire ai clienti di acquistare i propri servizi in CSP
description: Informazioni su come i partner del programma CSP possono consentire ai clienti di acquistare i propri servizi, ad esempio le prenotazioni di Azure, per una sottoscrizione acquistata in Partner Center.
ms.topic: how-to
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9fabd6bd188c9d596128672d9fce3321db9b5432
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150761"
---
# <a name="give-customers-permission-in-partner-center-to-buy-their-own-products-or-services"></a>Concedere ai clienti l'autorizzazione Partner Center acquistare i propri prodotti o servizi

**Ruoli appropriati:** Agente di amministrazione | Agente di vendita

Questo articolo illustra in che modo un partner del programma Cloud Solution Provider (CSP) può concedere a un cliente l'autorizzazione per acquistare alcuni dei propri servizi o risorse.

I partner del programma CSP spesso usano Partner Center e il relativo marketplace commerciale per acquistare soluzioni e servizi per i clienti. I partner consentono quindi ad alcuni clienti di effettuare il provisioning di questi servizi direttamente dal portale di Azure.

Ecco un esempio. Si supponiamo di acquistare una sottoscrizione del piano di Azure per un cliente in Partner Center. Si decide quindi di aggiungere altre risorse o servizi a tale sottoscrizione per conto del cliente. In questo caso, è possibile aggiungere prenotazioni di Azure alla sottoscrizione del cliente, ad esempio aggiungendo istanze di macchine virtuali riservate. È quindi possibile consentire al cliente di effettuare il provisioning delle risorse di prenotazione di Azure nel portale di Azure.

Ora, con la **funzionalità Autorizzazioni del** cliente, si offrono ai clienti più opzioni self-service con le risorse di Azure. Attivando le autorizzazioni per il cliente, si consente ai clienti di acquistare le proprie risorse( ad esempio, acquistare le proprie prenotazioni di Azure).  

## <a name="overview-of-customer-permissions-in-partner-center"></a>Panoramica delle autorizzazioni dei clienti in Partner Center

Usare la pagina **Account cliente** per attivare o disattivare le autorizzazioni dei clienti. Attualmente, questa funzionalità supporta:

- **Prenotazioni di Azure:** L'attivazione di questa autorizzazione consente al cliente di acquistare le proprie prenotazioni di Azure per una sottoscrizione di Azure specifica acquistata per loro.

Prima di attivare le autorizzazioni dei clienti, tenere presente questi punti importanti:

- Per impostazione predefinita, le autorizzazioni dei clienti vengono disabilitate (disattivate) automaticamente in Partner Center.

- Prima di poter attivare (o disattivare) le autorizzazioni per un cliente, è necessario avere il ruolo di agente amministratore in Partner Center.

  I partner a cui è assegnato il ruolo di agente di vendita o di help desk hanno accesso in sola lettura e non possono attivare o disattivare le autorizzazioni dei clienti.

- È possibile attivare (abilitare) le autorizzazioni per qualsiasi cliente scelto.

- È possibile attivare (o disattivare) le autorizzazioni dei clienti usando il dashboard Partner Center o [Partner Center API](/partner-center/develop/manage-customers).

- Dopo aver attivato (abilitato) le autorizzazioni per un cliente specifico, si sarà responsabili del pagamento per eventuali acquisti successivi effettuati da tale cliente. Se i clienti vogliono scambiare, annullare o rinnovare un acquisto effettuato (o se vogliono modificare l'ambito iniziale di una prenotazione), non potranno farlo da soli. Il partner deve chiedere all'utente di scambiare, annullare e rinnovare gli acquisti o apportare modifiche successive all'ambito di una prenotazione.  

- Dopo l'attivazione delle autorizzazioni per  un cliente specifico, non si riceverà notifica di eventuali acquisti successivi effettuati dal cliente.

- Gli acquisti successivi effettuati dal cliente verranno visualizzati Partner Center insieme agli acquisti effettuati dall'utente. È possibile trovare questi acquisti nella  pagina Cronologia  ordini del cliente, nella pagina Prenotazioni o nel [**log attività**](activity-logs.md).

>[!NOTE]
> Per informazioni sui prezzi che il cliente paga e su come aiutare i clienti a gestire gli acquisti, vedere Aiutare i clienti a gestire le prenotazioni [acquistate.](give-customers-permission.md#help-customers-manage-reservations-they-purchase)

## <a name="give-customers-permission-to-buy-their-own-azure-reservations"></a>Concedere ai clienti l'autorizzazione per acquistare le proprie prenotazioni di Azure

Le prenotazioni di Azure sono un modo eccellente per acquistare i servizi di Azure a una tariffa scontata. Per altre informazioni sui vantaggi delle prenotazioni di Azure, vedere [Che cosa sono le prenotazioni di Azure?](/azure/cost-management-billing/reservations/save-compute-costs-reservations)

A questo punto è possibile scegliere di acquistare prenotazioni di Azure per conto dei clienti, come già fatto. In caso contrario, è possibile concedere ai clienti l'autorizzazione per acquistare le proprie prenotazioni di Azure.

>[!NOTE]
> Dopo aver autorizzato i clienti ad acquistare le proprie prenotazioni di Azure, è possibile gestirne le prenotazioni. Per altre informazioni, vedere [Aiutare i clienti a gestire le prenotazioni acquistate.](give-customers-permission.md#help-customers-manage-reservations-they-purchase)

### <a name="to-enable-customers-to-buy-their-own-azure-reservations"></a>Per consentire ai clienti di acquistare le proprie prenotazioni di Azure

1. Verificare che il cliente abbia un piano di Azure esistente o una sottoscrizione globale di Azure acquistata per loro conto.

2. Verificare che al cliente sia stato assegnato **il ruolo Proprietario** per questa sottoscrizione.

3. Abilitare le autorizzazioni dei clienti (attivare **questa** funzionalità) per acquistare le proprie prenotazioni di Azure.

Ogni passaggio viene visualizzato di seguito.

### <a name="verify-the-customer-has-an-existing-azure-subscription"></a>Verificare che il cliente abbia una sottoscrizione di Azure esistente

Prima di concedere ai clienti l'autorizzazione per acquistare le proprie prenotazioni di Azure, è necessario verificare che il cliente abbia un piano di Azure o una sottoscrizione globale di Azure esistente. Se il cliente non visualizza alcuna sottoscrizione di Azure Partner Center, è necessario acquistarne una prima di attivare le autorizzazioni del cliente.

- Per verificare se un cliente ha già una sottoscrizione di Azure, accedere al dashboard di Partner Center, quindi selezionare **CSP** seguito da **Clienti**. Selezionare il cliente specifico nell'elenco. Selezionare quindi **Sottoscrizioni** e cercare eventuali sottoscrizioni basate sull'utilizzo per Piano di Azure o Globale di Azure.

- Se un cliente non ha una sottoscrizione di Azure esistente, è possibile acquistarne una. Vedere [Acquistare il piano di Azure.](purchase-azure-plan.md)

### <a name="verify-the-customer-has-been-assigned-the-correct-role-in-azure"></a>Verificare che al cliente sia stato assegnato il ruolo corretto in Azure

Dopo aver verificato che il cliente abbia una sottoscrizione di Azure esistente, è anche necessario verificare che agli utenti chiave associati al cliente sia stato assegnato il ruolo **Proprietario** corretto per tale sottoscrizione di Azure. Si tratta dell'accesso in base al ruolo necessario al cliente per acquistare prenotazioni di Azure per una sottoscrizione di Azure acquistata.

Alcuni partner potrebbero aver già assegnato il **ruolo Proprietario** ai clienti che vogliono gestire ed eseguire attivamente il provisioning delle proprie risorse di Azure. Se è già stato assegnato **lo stato** Proprietario a un cliente per gestire le sottoscrizioni precedenti acquistate, è possibile ignorare questo passaggio.  

> [!IMPORTANT]
> Se a un cliente  non è stato assegnato il ruolo Proprietario, riceverà un errore nell'portale di Azure impedendo l'acquisto di prenotazioni di Azure.

Per verificare che al cliente sia stato assegnato il **ruolo Proprietario** per una sottoscrizione di Azure:

1. Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.

2. Selezionare **CSP,** quindi **Clienti** e selezionare il cliente specifico.

3. Selezionare **Sottoscrizioni** per il cliente e individuare la sottoscrizione di Azure specifica.

4. Selezionare il **pulsante** Gestisci accanto alla sottoscrizione del cliente. In questo modo viene aperto [il portale di Azure](https://portal.azure.com/).

5. Per assegnare **il ruolo** Proprietario a un utente specifico, seguire questa procedura [Per assegnare un utente come amministratore](/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator).

### <a name="turn-on-or-turn-off-customer-permissions-to-purchase-their-own-azure-reservations"></a>Attivare o disattivare le autorizzazioni dei clienti per acquistare le proprie prenotazioni di Azure

Dopo aver verificato che il cliente abbia una  sottoscrizione di Azure esistente e che agli utenti sia assegnato il ruolo Proprietario per tale sottoscrizione, si è pronti per attivare (abilitare) le autorizzazioni del cliente. È anche possibile usare questi passaggi per disattivare (disabilitare) le autorizzazioni dei clienti. È possibile abilitare o disabilitare le autorizzazioni dei clienti usando il dashboard Partner Center o [Partner Center API](/partner-center/develop/manage-customers).

Per attivare o disattivare le autorizzazioni dei clienti in Partner Center:

1. Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.

2. Nel menu di spostamento a sinistra selezionare **CSP** e quindi **Clienti.** Viene visualizzato un elenco di clienti.

3. Selezionare un nome di cliente specifico.

4. Selezionare **Account** dal menu del cliente. Viene visualizzata la **pagina Account** del cliente.

5. Individuare **l'area Autorizzazioni** cliente nella parte inferiore della pagina.

   :::image type="content" source="images/give-customers-permission-reservations.png" alt-text="Autorizzazioni del cliente nella pagina Account." border="true":::

6. In **Prenotazioni di Azure** individuare l'opzione Consenti al cliente di **acquistare.**

7. Per attivare le autorizzazioni dei clienti, spostare l'interruttore accanto a questa opzione in **Posizione** attiva. Per disattivare le autorizzazioni dei clienti, spostare l'interruttore sulla **posizione Off.**

>[!NOTE]
> Per informazioni su cosa accade quando si attivano le autorizzazioni di un cliente per acquistare le proprie prenotazioni di Azure, vedere Panoramica delle autorizzazioni dei clienti [in Partner Center](give-customers-permission.md#overview-of-customer-permissions-in-partner-center).
>
>Quando si attivano (o disattivano) le autorizzazioni dei clienti, il log attività registra ogni azione. Questo log è accessibile quando si seleziona l'icona Ingranaggio nella parte superiore Partner Center dashboard. Quando si attivano o disattivano le autorizzazioni per i clienti, l'azione verrà visualizzata come **Crea** autorizzazioni di acquisto cliente o Elimina autorizzazioni di acquisto **cliente** nel log attività.

## <a name="help-customers-manage-reservations-they-purchase"></a>Aiutare i clienti a gestire le prenotazioni acquistate

Dopo aver dato ai clienti l'autorizzazione per acquistare le proprie prenotazioni di Azure, è possibile aiutarli a gestire meglio le risorse acquistate. I clienti possono gestire molti aspetti delle prenotazioni di Azure direttamente [dall'portale di Azure](https://portal.azure.com/). Sarà necessario il supporto dell'utente per la gestione di alcuni altri aspetti delle prenotazioni di Azure acquistate all'interno della sottoscrizione CSP.  

Aiutare i clienti a comprendere di più sulla gestione di questi aspetti delle prenotazioni di Azure:

- Prezzi che i clienti pagano per le prenotazioni di Azure
- Come i clienti possono ottimizzare l'uso delle prenotazioni di Azure
- Cosa accade quando i clienti acquistano prenotazioni con un ambito condiviso?
- Cosa accade se i clienti vogliono modificare, annullare e rinnovare una prenotazione o modificarne l'ambito?

**Prezzi che i clienti pagano per le prenotazioni.** Il cliente acquisterà prenotazioni di Azure in base a una sottoscrizione acquistata in precedenza nell'account di fatturazione del partner CSP. Anche il prezzo del cliente per le prenotazioni di Azure acquistate in base a questa sottoscrizione viene impostato dall'utente. Questo prezzo può essere diverso dal prezzo di Web Direct visualizzato dal cliente nel portale di Azure.

**Come i clienti possono ottimizzare l'uso di una prenotazione.** Alcuni clienti potrebbero trarre vantaggio da altre informazioni su come ottimizzare l'uso di una prenotazione o su come assegnare l'ambito iniziale di una prenotazione durante l'acquisto. Per altre informazioni, chiedere ai clienti di leggere [Gestire le prenotazioni per le risorse di Azure.](/azure/cost-management-billing/reservations/manage-reserved-vm-instance)

**Cosa accade quando un cliente acquista una prenotazione con un ambito condiviso?** Quando i clienti acquistano una prenotazione basata su una sottoscrizione CSP precedente e assegnano un ambito condiviso a tale prenotazione, tutti gli sconti che il cliente ha acquistato verranno applicati all'utilizzo corrispondente per tutte le sottoscrizioni acquistate dal partner CSP per tale cliente.

**Cosa devono fare i clienti se vogliono scambiare, annullare o rinnovare un acquisto effettuato o modificare l'ambito iniziale di una prenotazione?** I clienti devono chiedere al partner di aiutare a modificare l'ambito iniziale di una prenotazione. È anche necessario l'aiuto di un partner per lo scambio, l'annullamento o il rinnovo di una prenotazione. Non possono eseguire queste attività con prenotazioni basate sulle sottoscrizioni acquistate da un partner CSP.

## <a name="next-steps"></a>Passaggi successivi

- [Acquistare prenotazioni di Azure per conto dei clienti](azure-reservations-buying.md)

- [Partner Center - Vendere prenotazioni Microsoft](azure-reservations.md)

- [Gestire le prenotazioni di Azure per conto dei clienti](azure-reservations-manage.md)