---
title: Gestire le licenze nelle offerte del Marketplace
ms.topic: how-to
ms.date: 04/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come configurare e gestire le licenze per le offerte del marketplace commerciale ISV.
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f049ffda4c3d9476c09257fc814e5acac393cb54
ms.sourcegitcommit: 6c20c3cc4a226cada70c56df295966696affcec8
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/30/2021
ms.locfileid: "108328016"
---
# <a name="manage-licensing-in-marketplace-offers"></a>Gestire le licenze nelle offerte del Marketplace

**Ruoli appropriati**

- Amministratore globale
- Amministratore degli account

Questo articolo illustra il processo di configurazione di un'offerta in Partner Center, rendendola disponibile in Microsoft AppSource e quindi gestione delle licenze per tale offerta.  

>[!IMPORTANT]
>Le funzionalità di questo articolo sono attualmente in anteprima pubblica.

## <a name="before-you-begin"></a>Prima di iniziare

### <a name="commercial-marketplace-basics"></a>Nozioni di base sul marketplace commerciale

Prima di iniziare questo processo, è necessario acquisire familiarità con le nozioni di base del marketplace commerciale. Gli articoli nella tabella seguente consentono di iniziare. 

| Argomento  | Articolo  |
|-------|--------|
|Piani del marketplace commerciale | [Piani e prezzi per le offerte del marketplace commerciale](/azure/marketplace/plans-pricing)    |
|Offerte del marketplace commerciale  | [Tipi di elenco](/azure/marketplace/determine-your-listing-type)    |
|Account del marketplace commerciale |  [Creare un account del marketplace commerciale in Partner Center](/azure/marketplace/create-account) |

### <a name="determine-your-offer-id"></a>Determinare l'ID offerta

Nelle procedure seguenti verrà richiesto di immettere un ID offerta. Prendere ora tempo per creare un ID offerta appropriato, tenendo presenti i punti seguenti:

- Questo ID è visibile ai clienti nell'indirizzo Web per l'offerta del marketplace e nei modelli di Azure Resource Manager, se applicabile.
- L'ID offerta combinato con l'ID editore deve avere una lunghezza inferiore a 40 caratteri.
- Usare solo lettere minuscole e numeri. L'ID offerta può includere trattini e caratteri di sottolineatura, ma non spazi. Ad esempio, se l'ID editore è `testpublisherid` e si immette , `test-offer-1` l'indirizzo Web dell'offerta sarà `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1` .
- Questo ID non può essere modificato dopo aver selezionato **Crea.**

### <a name="determine-your-offer-alias"></a>Determinare l'alias dell'offerta

L'alias dell'offerta è il nome usato per l'offerta in Partner Center. È anche necessario un alias dell'offerta appropriato che segua le linee guida seguenti:

- Questo nome non viene usato nel marketplace ed è diverso dal nome dell'offerta e da altri valori visualizzati ai clienti.
- Questo nome non può essere modificato dopo aver selezionato Crea.

## <a name="create-your-offer"></a>Creare l'offerta

Il primo passaggio del processo di gestione delle licenze consiste nel creare l'offerta del marketplace commerciale. 

1. Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard/).
2. Nel menu di spostamento a sinistra selezionare **Marketplace commerciale/Panoramica.**
3. Nella parte superiore della pagina Panoramica selezionare Nuova offerta **e** quindi **Dynamics 365 for Customer Engagement & PowerApps.**
4. Immettere **l'ID offerta** e **l'alias dell'offerta** creati in precedenza.
5. Selezionare **Crea** per generare l'offerta e continuare.
6. Scegliere le opzioni di licenza.

    - Per abilitare la gestione delle licenze per l'offerta, selezionare **Abilita la gestione delle licenze delle app tramite Microsoft.** Si tratta di un'impostazione una sola volta e non è possibile modificarla dopo la pubblicazione dell'offerta.

    - È anche possibile consentire ai clienti di eseguire le funzionalità di base dell'app senza una licenza ed eseguire le funzionalità Premium dopo aver acquistato una licenza. A tale scopo, selezionare **Consenti ai clienti di installare l'app anche se le licenze non sono assegnate.**

    - Se non si vuole che la gestione delle licenze dell'offerta sia abilitata, selezionare Scarica adesso **(gratuito),** Versione di valutazione gratuita o **Contattami.**

## <a name="create-your-plan"></a>Creare il piano

In questi passaggi si definiranno il piano o i piani da abilitare per l'offerta.

1. Nel menu di spostamento a sinistra selezionare **Panoramica del piano** e quindi Selezionare Crea nuovo **piano.**
2. Immettere un **ID piano** e un **nome di** piano e quindi selezionare **Crea.**
3. Nella pagina **Elenco piani** immettere la **descrizione del piano.**
4. Per salvare la descrizione e completare l'operazione in un secondo momento, **selezionare Salva bozza.**

5. Al termine, selezionare Rivedi **e pubblica**. Le informazioni sul piano verranno ora visualizzate nel appsource.microsoft.com nell'inserzione dell'offerta (sezione piani).

6. Dopo aver creato tutti i piani per questa offerta, è necessario copiare l'ID servizio di ogni piano. Selezionare **Panoramica del** piano nella parte superiore della pagina Elenco piani. Copiare l'ID servizio per ogni piano in una posizione sicura.

## <a name="add-service-ids-to-your-solution"></a>Aggiungere gli ID servizio alla soluzione

Il passaggio successivo consiste nell'aggiornare la soluzione aggiungendo gli ID servizio per ogni piano appena copiato. Per istruzioni su questo argomento, vedere [Creare un pacchetto AppSource per la soluzione.](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource)

## <a name="upload-your-package-and-publish-your-offer"></a>Caricare il pacchetto e pubblicare l'offerta

1. Nel riquadro di spostamento sinistro selezionare **Marketplace commerciale** e quindi **Configurazione tecnica.**
2. In **Modello di licenza di base** selezionare **Utente**.
3. In **Pacchetto CRM** immettere l'URL del percorso del pacchetto.
4. Usare le altre schede nel riquadro di spostamento sinistro per immettere eventuali altre informazioni necessarie. Al termine, selezionare Rivedi **e pubblica**.

Dopo aver pubblicato l'offerta, verranno esaminate e verificate le informazioni. In caso di problemi con questo processo, l'utente verrà avvisato. Quando tutti i problemi sono stati risolti, si otterrà una notifica che l'offerta è disponibile in AppSource. A questo punto è possibile renderlo live.

## <a name="make-your-offer-live-in-partner-center"></a>Rendere l'offerta live Partner Center

La procedura seguente illustra il processo di rendere l'offerta live in AppSource. Per altre informazioni su questo processo, vedere [Introduzione alle opzioni di elenco.](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type)

>[!NOTE]
>Dopo aver pubblicato l'offerta, la pubblicazione dell'offerta sarà di 4-6 ore.

1. Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard/).
2. Nel menu di spostamento a sinistra selezionare **Marketplace commerciale/Panoramica.**
3. Nella **pagina Panoramica** trovare l'offerta che si sta cercando. Lo stato delle offerte pronte per la pubblicazione sarà **Anteprima.** Selezionare l'offerta.
4. Nella pagina **Panoramica dell'offerta** selezionare **Vai in tempo reale.**
L'offerta sarà live in 4-6 ore.
5. Per visualizzare la presentazione dell'offerta in AppSource, selezionare il **collegamento AppSource** nella parte inferiore della pagina **Panoramica dell'offerta.**

    - **Per le offerte abilitate** per le licenze: se l'offerta richiede un controllo della licenza, gli utenti potranno immettere un lead solo facendo clic su **Contattami,** in modo da poter comunicare con loro.

    - **Per le offerte abilitate** per le licenze con l'opzione di installazione  gratuita: se l'offerta non richiede un controllo della licenza, gli utenti amministratori visualizzano un pulsante Scarica adesso oltre a **Contattami.** Gli utenti che vogliono provare l'opzione di installazione gratuita devono fare clic su Scarica adesso per installare l'offerta nell Power Platform di amministrazione.  Gli utenti possono comunque usare **Contattami** in caso di domande o se vogliono eseguire l'aggiornamento a un piano a pagamento.

## <a name="register-isv-connect-deal-in-deal-registration"></a>Registrare la trattativa ISV Connect nella registrazione della trattativa

Prima di poter assegnare licenze a un cliente, ogni vendita deve essere registrata in Partner Center. A tale scopo, vedere [Registrare le trattative.](register-deals.md)

## <a name="invite-the-customer"></a>Invitare il cliente

Usare la procedura seguente per invitare il cliente a partecipare a questa trattativa.  

1. Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard/).
2. Nel menu di spostamento a sinistra selezionare **Marketplace commerciale/Panoramica.**
3. Nel menu di spostamento a sinistra selezionare **Segnalazioni** e quindi selezionare **Deal Registration (Registrazione trattativa).**
4. Filtrare **le offerte** inviate, selezionare la scheda **In** corso e quindi selezionare l'offerta desiderata.
5. Nella pagina di panoramica per questa operazione selezionare **Gestisci licenze**.
6. Nella finestra **Gestisci licenze** selezionare il cliente nell'elenco a discesa **Dettagli** cliente. Se la relazione con il cliente non esiste ancora, selezionare **+Invita un nuovo cliente a acconsentire.**
7. Copiare il collegamento visualizzato.
8. Inviare questo collegamento tramite posta elettronica all'amministratore della fatturazione o all'amministratore globale del cliente e fare in modo che usi questo collegamento per accedere admin.microsoft.com e accettare e autorizzare la relazione che si sta stabilendo.

    >[!NOTE]
    >La relazione non verrà stabilita fino a quando il cliente non esegue questo passaggio.

## <a name="activate-manage-and-remove-your-licenses"></a>Attivare, gestire e rimuovere le licenze

Dopo che il cliente ha autorizzato la relazione con l'utente, è possibile iniziare ad aggiungere piani dall'offerta e assegnare licenze a ogni piano.

1. Nella finestra Manage licenses for this deal (Gestisci licenze) selezionare **+Add a plan (Aggiungi un piano).**
2. Completare **i campi Plans for this solution** (Piani per questa soluzione) e Number of licenses **(Numero di** licenze) e quindi selezionare Update licenses **(Aggiorna licenze).** Le licenze saranno disponibili in admin.microsoft.com che i clienti possono gestire e assegnare ai dipendenti.

    - Per modificare il numero di licenze per un piano esistente, immettere il nuovo numero nel campo **Numero** di licenze e quindi **selezionare Aggiorna licenze**.

    - Per disattivare o rimuovere licenze per un accordo, selezionare l'icona del cestino nel **campo Azioni** e quindi **selezionare Aggiorna licenze**.

## <a name="next-steps"></a>Passaggi successivi

[Risorse relative alle licenze](support-resources-licensing.md)
