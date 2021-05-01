---
title: Gestire le licenze nelle offerte del marketplace
ms.topic: how-to
ms.date: 04/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come configurare e gestire le licenze per le offerte del marketplace commerciale ISV.
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3b2281696a2fe69253cd033eb2a7eef7fb3046f3
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284873"
---
# <a name="manage-licensing-in-marketplace-offers"></a>Gestire le licenze nelle offerte del marketplace

**Ruoli appropriati**

- Amministratore globale
- Amministratore degli account

Questo articolo illustra come configurare un'offerta in Partner Center, renderla disponibile in Microsoft AppSource e quindi gestire le licenze per tale offerta.  

>[!IMPORTANT]
>Le funzionalità di questo articolo sono attualmente disponibili in anteprima pubblica.

## <a name="before-you-begin"></a>Prima di iniziare

Prima di iniziare questo processo, è consigliabile acquisire familiarità con le informazioni seguenti.

### <a name="review-the-azure-marketplace-documentation"></a>Esaminare la documentazione Azure Marketplace

Gli articoli seguenti contengono informazioni che è necessario conoscere prima di continuare. 

- [Creare un'offerta Dynamics 365 for Customer Engagement & PowerApps](https://docs.microsoft.com/azure/marketplace/dynamics-365-customer-engage-offer-setup)
- [Creare un account del marketplace commerciale in Partner Center](https://docs.microsoft.com/azure/marketplace/create-account)

### <a name="create-your-offer-id"></a>Creare l'ID offerta

Nelle procedure seguenti verrà richiesto di immettere un ID offerta. A questo punto, è opportuno creare un ID offerta appropriato, tenendo presente quanto segue:

- Questo ID è visibile ai clienti nell'indirizzo Web per l'offerta del marketplace e nei modelli di Azure Resource Manager, se applicabile.
- L'ID offerta combinato con l'ID editore deve avere una lunghezza inferiore a 40 caratteri.
- Usare solo lettere minuscole e numeri. L'ID offerta può includere trattini e caratteri di sottolineatura, ma non spazi. Ad esempio, se l'ID editore è testpublisherid e si immette test-offer-1, l'indirizzo Web dell'offerta sarà https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1 .
- Questo ID non può essere modificato dopo aver selezionato **Crea.**

### <a name="create-your-offer-alias"></a>Creare l'alias dell'offerta

L'alias dell'offerta è il nome usato per l'offerta in Partner Center. È anche necessario un alias dell'offerta appropriato che segua le linee guida seguenti:

- Questo nome non viene usato nel marketplace ed è diverso dal nome dell'offerta e da altri valori visualizzati ai clienti.
- Questo nome non può essere modificato dopo aver selezionato Crea.

## <a name="create-your-offer"></a>Creare l'offerta

Il primo passaggio del processo di gestione delle licenze consiste nel creare l'offerta del marketplace commerciale. 

1. Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard/).
2. Nel menu di spostamento a sinistra selezionare **Marketplace commerciale/Panoramica.**
3. Nella parte superiore della pagina Panoramica selezionare Nuova offerta **e** quindi **Dynamics 365 for Customer Engagement & PowerApps.**
4. Immettere **l'ID offerta** e **l'alias** dell'offerta creati in precedenza.
5. Selezionare **Crea** per generare l'offerta e continuare.
6. Scegliere le opzioni di licenza.

    - Per abilitare la gestione delle licenze per l'offerta, selezionare Abilita gestione licenze **app tramite Microsoft**. Si tratta di un'impostazione una sola volta e non è possibile modificarla dopo la pubblicazione dell'offerta.

    - È anche possibile abilitare i clienti per eseguire le funzionalità di base dell'app senza una licenza ed eseguire le funzionalità Premium dopo aver acquistato una licenza. A tale scopo, selezionare **Consenti ai clienti di installare l'app anche se le licenze non sono assegnate.**

    - Se non si vuole che la gestione delle licenze dell'offerta sia abilitata, selezionare Scarica adesso **(gratuito),** Versione di valutazione gratuita o **Contattami.**

## <a name="create-your-plan"></a>Creare il piano

In questi passaggi si definiranno il piano o i piani da abilitare per l'offerta.

1. Nel menu di spostamento a sinistra selezionare **Panoramica del piano** e quindi Selezionare Crea nuovo **piano.**
2. Immettere un **ID piano** e un **nome di** piano e quindi selezionare **Crea**.
3. Nella pagina **Elenco piani** immettere la descrizione **del piano.**
4. Per salvare la descrizione e completare in un secondo momento, **selezionare Salva bozza.**

5. Al termine, selezionare Rivedi **e pubblica**. Le informazioni sul piano verranno ora visualizzate nel appsource.microsoft.com nell'inserzione dell'offerta (sezione piani).

6. Dopo aver creato tutti i piani per questa offerta, è necessario copiare l'ID servizio di ogni piano. Selezionare **Panoramica del** piano nella parte superiore della pagina Elenco piani. Copiare l'ID servizio per ogni piano in una posizione sicura.

## <a name="add-service-ids-to-your-solution"></a>Aggiungere GLI ID servizio alla soluzione

Il passaggio successivo consiste nell'aggiornare la soluzione aggiungendo gli ID servizio per ogni piano appena copiato. Per indicazioni, vedere [Creare un pacchetto AppSource per la soluzione.](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource)

## <a name="upload-your-package-and-publish-your-offer"></a>Caricare il pacchetto e pubblicare l'offerta

1. Nel riquadro di spostamento a sinistra selezionare **Marketplace commerciale** e quindi Selezionare **Configurazione tecnica.**
2. In **Base License Model (Modello di licenza** di base) selezionare User **(Utente).**
3. In **Crm Package (Pacchetto CRM)** immettere l'URL del percorso del pacchetto.
4. Usare le altre schede nel riquadro di spostamento a sinistra per immettere eventuali altre informazioni necessarie. Al termine, selezionare Rivedi **e pubblica.**

Dopo aver pubblicato l'offerta, verranno esaminate e verificate le informazioni. In caso di problemi con questo processo, l'utente verrà avvisato. Dopo aver risolto tutti i problemi, si otterrà una notifica che indica che l'offerta è disponibile in AppSource. A questo punto è possibile renderlo live.

## <a name="make-your-offer-live-in-partner-center"></a>Rendere l'offerta live in Partner Center

La procedura seguente illustra il processo per rendere l'offerta live in AppSource. Per altre informazioni su questo processo, vedere [Introduzione alle opzioni di elenco.](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type)

>[!NOTE]
>Dopo aver pubblicato l'offerta, la pubblicazione dell'offerta sarà di 4-6 ore.

1. Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard/).
2. Nel menu di spostamento a sinistra selezionare **Marketplace commerciale/Panoramica.**
3. Nella **pagina Panoramica** trovare l'offerta che si sta cercando. Lo stato delle offerte pronte per la pubblicazione sarà **Anteprima.** Selezionare l'offerta.
4. Nella pagina **Panoramica dell'offerta** selezionare **Vai al live.**
L'offerta sarà live in 4-6 ore.
5. Per visualizzare la presentazione dell'offerta in AppSource, selezionare il **collegamento AppSource** nella parte inferiore della **pagina panoramica dell'offerta.**

    - **Per le offerte abilitate** per le licenze: se l'offerta richiede un controllo della licenza, gli utenti potranno immettere un lead solo facendo clic su **Contattami,** in modo da poter comunicare con loro.

    - **Per le offerte abilitate** per le licenze con l'opzione di installazione  gratuita: se l'offerta non richiede un controllo della licenza, gli utenti amministratori visualizzano un pulsante Scarica adesso oltre a **Contattami.** Gli utenti che vogliono provare l'opzione di installazione gratuita dovrebbero fare clic su Scarica **adesso,** che li porterà a installare l'offerta Power Platform Admin Center. Gli utenti possono comunque usare **Contattami** se hanno domande o se vogliono eseguire l'aggiornamento a un piano a pagamento.

## <a name="register-isv-connect-deal-in-dealreg"></a>Registrare l'offerta ISV Connect in DealReg

Il passaggio successivo consiste nel registrare l'accordo. A tale scopo, vedere [Registrare le offerte.](https://docs.microsoft.com/partner-center/register-deals)

## <a name="invite-the-customer"></a>Invitare il cliente

Usare la procedura seguente per invitare il cliente a partecipare all'offerta.  

1. Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard/).
2. Nel menu di spostamento a sinistra selezionare **Marketplace commerciale/Panoramica.**
3. Filtrare **le offerte** inviate, selezionare la scheda **In** corso e quindi selezionare l'offerta desiderata.
4. Nella pagina di panoramica per questa operazione selezionare **Gestisci licenze**.
5. Nella finestra **Gestisci licenze** selezionare il cliente nell'elenco a discesa **Dettagli** cliente. Se la relazione con il cliente non esiste ancora, selezionare **+Invita un nuovo cliente a acconsentire.**
6. Copiare il collegamento visualizzato.
7. Inviare questo collegamento tramite posta elettronica all'amministratore della fatturazione o all'amministratore globale del cliente e fare in modo che usi questo collegamento per accedere admin.microsoft.com e accettare e autorizzare la relazione che si sta stabilendo.

    >[!NOTE]
    >La relazione non verrà stabilita fino a quando il cliente non esegue questo passaggio.

## <a name="activate-manage-and-remove-your-licenses"></a>Attivare, gestire e rimuovere le licenze

Dopo aver stabilito il cliente, è possibile iniziare ad aggiungere piani dall'offerta e assegnare licenze a ogni piano.

1. Nella finestra Gestisci licenze per questa trattativa selezionare **+Aggiungi un piano.**
2. Completare **i campi Piani per questa soluzione** e Numero **di** licenze e quindi selezionare **Aggiorna licenze.** Le licenze saranno disponibili a livello admin.microsoft.com che i clienti possono gestire e assegnare ai dipendenti.

    - Per modificare il numero di licenze per un piano esistente, immettere il nuovo numero nel campo **Numero** di licenze e quindi selezionare **Aggiorna licenze.**

    - Per disattivare o rimuovere le licenze per una trattativa, selezionare l'icona del cestino nel **campo Azioni** e quindi selezionare **Aggiorna licenze.**