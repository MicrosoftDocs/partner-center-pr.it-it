---
title: Concedi ai clienti l'autorizzazione per acquistare i propri servizi
ms.topic: article
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Scopri in che modo i partner del programma CSP possono consentire ai clienti di acquistare i propri servizi, ad esempio le prenotazioni di Azure, per una sottoscrizione acquistata per loro.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
Keywords: sottoscrizione, acquisto self-service, riservatezza self-service, abilitazione di ri, disabilitazione di RI, self-service, acquisto di clienti, autorizzazioni dei clienti, istanza riservata di acquisto del cliente, prenotazione dei clienti di Azure, attivare la funzionalità self-service, disattivare la funzionalità self-service
ms.localizationpriority: medium
ms.openlocfilehash: ee8f1221344ce2375aff63c52bbfd42350a29839
ms.sourcegitcommit: 8359f618426e341180b0380367dd9d16dfd6623c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/29/2020
ms.locfileid: "82255465"
---
# <a name="learn-how-to-give-customers-permission-to-buy-their-own-products-or-services"></a>Informazioni su come concedere ai clienti l'autorizzazione per acquistare prodotti o servizi propri

**Si applica a**

- Centro per i partner
- Partner aderenti al programma CSP

**Ruoli appropriati**

- Agente amministratore
- Agente di vendita

Questo articolo illustra in che modo un partner nel programma Cloud Solution Provider (CSP) può concedere a un cliente l'autorizzazione per acquistare alcuni dei propri servizi o risorse.

I partner del programma CSP spesso usano il centro per i partner e il suo Marketplace commerciale per acquistare soluzioni e servizi per i clienti. I partner consentono quindi ad alcuni clienti di effettuare il provisioning di questi servizi direttamente dalla portale di Azure.

Di seguito è riportato un esempio. Supponiamo di acquistare una sottoscrizione di piano di Azure per un cliente nel centro per i partner. Si decide quindi di aggiungere altre risorse o servizi alla sottoscrizione per conto dell'utente. In questo caso, è possibile aggiungere prenotazioni di Azure alla sottoscrizione del cliente, ad esempio aggiungendo istanze di macchine virtuali riservate. È quindi possibile consentire al cliente di eseguire ulteriormente il provisioning delle risorse di prenotazione di Azure nel portale di Azure.

Con la funzionalità per le **autorizzazioni** dei clienti, ora è possibile offrire ai clienti più opzioni self-service con le risorse di Azure. Attivando le autorizzazioni per il cliente, si consente ai clienti di acquistare le proprie risorse (ad esempio, acquistando le proprie prenotazioni di Azure).  

## <a name="overview-of-customer-permissions-in-partner-center"></a>Panoramica delle autorizzazioni dei clienti nel centro per i partner

Utilizzare la pagina **account** cliente per attivare o disattivare le autorizzazioni del cliente. Attualmente questa funzionalità supporta:

- **Prenotazioni di Azure:** L'attivazione di questa autorizzazione consente al cliente di acquistare le proprie prenotazioni di Azure per una sottoscrizione di Azure specifica acquistata per loro.

Prima di attivare le autorizzazioni dei clienti, tenere presenti i seguenti punti importanti:

- Per impostazione predefinita, le autorizzazioni dei clienti vengono disabilitate automaticamente (disattivate) nel centro per i partner.
- Prima di poter attivare o disattivare le autorizzazioni per un cliente, è necessario disporre del ruolo di agente di amministrazione nel centro per i partner.
  I partner a cui è stato assegnato il ruolo di agente di vendita o di supporto tecnico hanno accesso in sola lettura e non possono attivare o disattivare le autorizzazioni dei clienti.
- È possibile attivare le autorizzazioni (Abilita) per qualsiasi cliente scelto.
- È possibile attivare o disattivare le autorizzazioni dei clienti usando il dashboard del centro per i partner o le [API del centro](https://docs.microsoft.com/partner-center/develop/manage-customers)per i partner.
- Dopo aver attivato (abilitato) le autorizzazioni per un cliente specifico, si sarà responsabili del pagamento di eventuali acquisti successivi effettuati dal cliente. Se i clienti vogliono scambiare, annullare o rinnovare un acquisto effettuato, non saranno in grado di eseguire questa operazione. È necessario chiedere all'utente, come partner, di aiutarli a scambiare, annullare o rinnovare questi acquisti.
- Dopo aver immesso le autorizzazioni per un cliente specifico, l'utente **non** riceverà alcuna notifica per eventuali acquisti successivi effettuati dal cliente.
- Gli acquisti successivi effettuati dal cliente verranno visualizzati nel centro per i partner insieme a eventuali acquisti effettuati dall'utente. È possibile trovare questi acquisti nella pagina della **cronologia dell'ordine** del cliente, nella relativa pagina **prenotazioni** o nel [**log attività**](activity-logs.md).

## <a name="give-customers-permission-to-buy-their-own-azure-reservations"></a>Concedi ai clienti l'autorizzazione per acquistare le proprie prenotazioni di Azure

Le prenotazioni di Azure sono un ottimo modo per acquistare i servizi di Azure a una tariffa scontata. Per altre informazioni sui vantaggi delle prenotazioni di Azure, vedere [che cosa sono le prenotazioni di Azure?](https://docs.microsoft.com/azure/cost-management-billing/reservations/save-compute-costs-reservations)

È ora possibile scegliere di acquistare prenotazioni di Azure per conto dei clienti, come è già stato fatto. In alternativa, è possibile concedere ai clienti l'autorizzazione per acquistare le proprie prenotazioni di Azure.

>[!NOTE]
> Dopo aver fornito ai clienti l'autorizzazione per acquistare le proprie prenotazioni di Azure, è possibile aiutarli a comprendere come gestire le prenotazioni acquistate. È ad esempio possibile che i clienti desiderino ottenere informazioni su come ottimizzare l'uso di una prenotazione o su come modificare l'ambito di una prenotazione. Per altre informazioni su questi argomenti, chiedere ai clienti di leggere [gestire le prenotazioni per le risorse di Azure]( https://docs.microsoft.com/azure/cost-management-billing/reservations/manage-reserved-vm-instance).

### <a name="to-enable-customers-to-buy-their-own-azure-reservations"></a>Per consentire ai clienti di acquistare le proprie prenotazioni di Azure

1. Verificare che il cliente disponga di un piano di Azure esistente o di una sottoscrizione globale di Azure acquistata per loro conto.

2. Verificare che al cliente sia stato assegnato il ruolo **proprietario** per questa sottoscrizione.

3. Abilitare le autorizzazioni dei clienti (attivare **questa funzionalità)** per acquistare le proprie prenotazioni di Azure.

Ogni passaggio viene visualizzato di seguito.

### <a name="verify-the-customer-has-an-existing-azure-subscription"></a>Verificare che il cliente disponga di una sottoscrizione di Azure esistente

Prima di concedere ai clienti l'autorizzazione per acquistare le proprie prenotazioni di Azure, è necessario verificare che il cliente disponga di un piano di Azure o di una sottoscrizione globale di Azure esistente. Se il cliente non visualizza alcuna sottoscrizione di Azure corrente nel centro per i partner, è necessario acquistare una sottoscrizione prima di attivare le autorizzazioni del cliente.

- Per verificare se un cliente dispone già di una sottoscrizione di Azure, accedere al dashboard del centro per i partner, quindi selezionare **CSP** seguito dai **clienti**. Selezionare il cliente specifico dall'elenco. Selezionare quindi **sottoscrizioni** e cercare eventuali sottoscrizioni basate sull'utilizzo per piano Azure o Azure globale.

- Se un cliente non ha una sottoscrizione di Azure esistente, è possibile acquistarne una sottoscrizione. Vedere [acquistare il piano di Azure](purchase-azure-plan.md).

### <a name="verify-the-customer-has-been-assigned-the-correct-role-in-azure"></a>Verificare che al cliente sia stato assegnato il ruolo corretto in Azure

Dopo aver verificato che il cliente disponga di una sottoscrizione di Azure esistente, è necessario verificare anche che agli utenti chiave associati al cliente sia stato assegnato il ruolo di **proprietario** corretto per la sottoscrizione di Azure. Questo è l'accesso in base al ruolo (RBAC) a cui il cliente deve acquistare le prenotazioni di Azure per una sottoscrizione di Azure acquistata.

Alcuni partner potrebbero avere già assegnato il ruolo di **proprietario** ai clienti che desiderano gestire attivamente ed effettuare il provisioning delle proprie risorse di Azure. Se lo stato del **proprietario** è già stato assegnato a un cliente per gestire le sottoscrizioni acquistate in precedenza, è possibile ignorare questo passaggio.  

> [!IMPORTANT]
> Se a un cliente non è stato assegnato il ruolo di **proprietario** , riceverà un errore nel portale di Azure impedendo loro di acquistare prenotazioni di Azure.

Per verificare che al cliente sia stato assegnato il ruolo **proprietario** per una sottoscrizione di Azure:

1. Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.

2. Selezionare **CSP**, **Customers** e selezionare il cliente specifico.

3. Selezionare le **sottoscrizioni** per il cliente e individuare la sottoscrizione di Azure specifica.

4. Selezionare il pulsante **Gestisci** accanto alla sottoscrizione del cliente. In questo modo si apre il [portale di Azure](https://portal.azure.com/).

5. Per assegnare il ruolo **proprietario** a un utente specifico, attenersi alla procedura seguente [per assegnare un utente come amministratore](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator).

### <a name="turn-on-or-turn-off-customer-permissions-to-purchase-their-own-azure-reservations"></a>Attivare o disattivare le autorizzazioni del cliente per acquistare le proprie prenotazioni di Azure

Dopo aver verificato che il cliente dispone di una sottoscrizione di Azure esistente e che agli utenti viene assegnato il ruolo di **proprietario** per la sottoscrizione, è possibile attivare le autorizzazioni del cliente. È anche possibile usare questi passaggi per disattivare (disabilitare) le autorizzazioni del cliente. È possibile abilitare o disabilitare le autorizzazioni dei clienti usando il dashboard del centro per i partner o le [API del centro](https://docs.microsoft.com/partner-center/develop/manage-customers)per i partner.

Per attivare o disattivare le autorizzazioni dei clienti nel centro per i partner:

1. Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.

2. Nel menu di spostamento a sinistra selezionare **CSP**e quindi **Customers**. Verrà visualizzato un elenco di clienti.

3. Selezionare un nome di cliente specifico.

4. Selezionare **account** dal menu Customer. Viene visualizzata la pagina **account** cliente.

5. Individuare l'area **autorizzazioni del cliente** nella parte inferiore della pagina.

   ![Autorizzazioni del cliente nella pagina dell'account](images/give-customers-permission-reservations.png)

6. In **prenotazioni di Azure**individuare l'opzione **Consenti al cliente di acquistare** .

7. Per attivare le autorizzazioni del cliente, spostare il commutatore accanto a questa opzione in posizione **on** . Per disattivare le autorizzazioni del cliente, spostare il commutatore nella posizione **off** .

>[!NOTE]
> Per altre informazioni su ciò che accade quando si attivano le autorizzazioni di un cliente per acquistare le proprie prenotazioni di Azure, vedere [Panoramica delle autorizzazioni dei clienti nel centro per i partner](give-customers-permission.md#overview-of-customer-permissions-in-partner-center). Quando si attivano o disattivano le autorizzazioni del cliente, il log attività registra ciascuna azione. (Questo log è accessibile quando si seleziona l'icona a forma di ingranaggio nella parte superiore del dashboard del centro per i partner). Quando si attivano o disattivano le autorizzazioni del cliente, l'azione verrà visualizzata come **creare autorizzazioni di acquisto del cliente** o **eliminare le autorizzazioni di acquisto del cliente** nel log attività.

## <a name="see-also"></a>Vedere anche

- [Acquista prenotazioni di Azure per conto dei tuoi clienti](azure-reservations-buying.md)
- [Centro per i partner-vendere prenotazioni Microsoft](azure-reservations.md)
- [Gestisci prenotazioni di Azure per conto dei tuoi clienti](azure-reservations-manage.md) 