---
title: Registrazione degli incentivi
ms.topic: how-to
ms.date: 04/15/2021
description: Iscriversi al programma incentivi e assegnare i ruoli necessari per la gestione degli utenti. Questo articolo descrive il processo di registrazione.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.openlocfilehash: c4e24c22790edddef02e7936eaef9ed788489a37
ms.sourcegitcommit: 9f6be9bc8d9a065422d1ec8388bd770eb6cd9f33
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/16/2021
ms.locfileid: "107528527"
---
# <a name="enrollment-and-user-management-in-the-incentives-program"></a>Registrazione e gestione utenti nel programma incentivi

**Ruoli appropriati**

- Amministratore degli incentivi

>[!NOTE]
>Prima di poter eseguire la registrazione al programma di incentivi, è necessario aver completato il Partner Membership Center per Partner Center [migrazione.](prepare-pmc-pc-migration.md)

Il processo di registrazione è costituito da due passaggi.

**Passaggio 1. Gestione utenti:** questo passaggio comporta la definizione dell'amministratore incentivi in Partner Center.

**Passaggio 2. Registrazione:** Microsoft invia un invito a registrarsi nel programma di incentivi.

## <a name="user-management"></a>User Management

Per registrarsi in un Partner Center di incentivi, l'amministratore globale o l'amministratore dell'account deve configurare gli utenti aziendali come amministratori degli incentivi. Per informazioni su account, ruoli e autorizzazioni partner, vedere [Gestire l'account Partner Center partner.](partner-center-account-setup.md) Il amministratore globale può anche configurare gli utenti aziendali tramite il Azure Active Directory (Azure AD).

>[!NOTE]
>Solo l'amministratore incentivo può registrarsi nei programmi di incentivi. Se non è presente alcun amministratore incentivi per la località, il amministratore globale e l'amministratore account devono assegnarne uno. L'amministratore dell'incentivo deve essere assegnato per gli ID MPN della posizione. L amministratore globale amministratore dell'account o dell'account può anche essere assegnato come amministratore incentivo. Per altre informazioni sui diversi ruoli, vedere [Gestire gli incentivi.](permissions-overview.md#manage-incentives)

## <a name="enrollment-process"></a>Processo di registrazione

Una volta che l'organizzazione è idonea per gli incentivi, Microsoft invierà un invito all'amministratore incentivi di MPNLocationID idoneo per iniziare il processo di registrazione. Questo messaggio di posta elettronica verrà inviato da **Microsoft Partner Center** e avrà l'oggetto **Partner Incentive Enrollment Invitation**. Aprire l'invito e selezionare **Introduzione.**

Verrà visualizzato anche un invito nella Partner Center home page. Dopo aver selezionato il messaggio, non sarà più possibile visualizzare il messaggio. Tuttavia, l'amministratore incentivi può comunque completare il processo accedendo al [dashboard](https://partner.microsoft.com/dashboard/) Partner Center e selezionando Panoramica in **Incentivi** nel riquadro di spostamento a sinistra.  Selezionare **Registra** e quindi completare il profilo di pagamento e fiscale per il programma.

Se è già stata impostata una configurazione del profilo bancario predefinito per una località MPN e si sta tentando di registrarsi per la stessa località MPN in un programma di incentivi, quando si seleziona **Registra** e si accetta l'invito, verrà visualizzato il profilo bancario predefinito. Verrà visualizzato anche qualsiasi profilo fiscale disponibile se è stato creato per tale località MPN. Se Microsoft dispone di tutti i dettagli richiesti per il profilo bancario e fiscale, verrà richiesto di selezionare **Invia** per completare la registrazione. Vedere [Configurare un profilo bancario predefinito.](incentives-create-and-manage-your-payout-and-tax-profiles.md#set-up-a-default-bank-profile)

È anche possibile scegliere un profilo bancario diverso da quello predefinito. Se Microsoft richiede dettagli aggiuntivi per i profili di pagamento  o fiscali o la  valuta, verrà richiesto di continuare e verrà reindirizzato alla pagina del profilo Pagamento e imposta per fornire i dettagli mancanti. 

Una registrazione viene considerata completa solo quando il profilo di pagamento e fiscale fornito per la registrazione viene convalidato da Microsoft.

Alcuni programmi di incentivi non hanno criteri di idoneità e sono aperti a tutti i partner. L'amministratore degli incentivi visualizza gli inviti per questi programmi nella pagina di panoramica degli incentivi, purché abbia le autorizzazioni per il programma di incentivi pertinente e MPN. Microsoft non invia inviti tramite posta elettronica per questi programmi.

Per altre informazioni sul processo di registrazione, scaricare la [Guida all'iscrizione agli](https://partner.microsoft.com/resources/detail/partner-center-incentives-enrollment-pdf) incentivi (è necessario l'accesso).

## <a name="expiration-and-renewal"></a>Scadenza e rinnovo

L'iscrizione agli incentivi scade alla fine dell'anno fiscale. Tuttavia, finché si rimane un partner idoneo con un contratto attivo, Microsoft esegue il roll forward della registrazione degli incentivi nel prossimo anno fiscale. Non è necessario intraprendere alcuna azione, purché le informazioni sui pagamenti e sulle imposte necessarie per il programma di incentivi sono complete in base alle regole del programma di incentivi.

## <a name="next-steps"></a>Passaggi successivi

- [Determinare l'idoneità al programma](incentives-determined-your-program-eligibility.md)
- [Creare e gestire i profili di pagamento e fiscali](incentives-create-and-manage-your-payout-and-tax-profiles.md)
