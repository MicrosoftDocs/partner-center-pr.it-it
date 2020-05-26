---
title: Connettore di co-selling per Salesforce CRM Partner Center
ms.topic: article
ms.date: 05/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Uso del connettore Salesforce CRM, ottenere i riferimenti da Microsoft
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: ''
ms.localizationpriority: medium
ms.openlocfilehash: ad39bdde92611066d0dd0c56d8b9133f4d9dcaa9
ms.sourcegitcommit: 97f1ff7386562cbb945bdfbcf15c85bc8303cac2
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/25/2020
ms.locfileid: "83825698"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Co-selling Connector per Salesforce CRM-Panoramica

### <a name="appropriate-roles"></a>Ruoli appropriati

- Amministratore delle segnalazioni
- Amministratore di sistema o verbi di sistema in CRM

Il connettore di co-selling del centro partner consente ai venditori di co-selling con Microsoft all'interno dei sistemi CRM. Non dovranno essere sottoposti a training per usare il centro per i partner per gestire le offerte di co-selling. Utilizzando i connettori di co-selling, sarà possibile creare un nuovo riferimento di co-selling per coinvolgere un venditore Microsoft, ricevere i riferimenti da Microsoft seller, accettare o rifiutare i riferimenti, modificare i dati relativi alle trattative, ad esempio il valore dell'offerta, la data di chiusura e così via, nonché ricevere eventuali aggiornamenti dai venditori Microsoft per le offerte di co-selling. Questa operazione può essere eseguita all'interno del CRM scelto piuttosto che nel centro per i partner. 

La soluzione è basata sulla soluzione Microsoft Power automatizzate e usa le API del centro per i partner Microsoft.


## <a name="before-you-install---pre-requisites"></a>Prima di installare-prerequisiti

|**Argomenti**   |**Dettagli**   |**Collegamenti**   |
|--------------|--------------------|------|
|ID Microsoft Partner Network |È necessario un ID MPN valido|Per aggiungere [MPN](https://partner.microsoft.com/)|
|Co-selling pronto|La soluzione IP/servizi deve essere pronta per il co-selling.|[Vendi con Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Account del Centro per i partner|L'ID MPN associato al tenant del centro per i partner deve corrispondere all'ID MPN associato alla soluzione di co-selling. Prima di distribuire i connettori, verificare che sia possibile visualizzare i riferimenti di co-selling nel portale del centro per i partner.|[Gestire l'account](create-user-accounts-and-set-permissions.md)|
|Ruoli utente del Centro per i partner|Il dipendente che installerà e userà i connettori deve essere un amministratore dei riferimenti|[Assegnare autorizzazioni e ruoli utente](create-user-accounts-and-set-permissions.md)|
|CRM Salesforce|Il ruolo utente CRM è amministratore sistema o sistema verbi|[Assegnare i ruoli in Dynamics 365](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Power automatizzare l'account di flusso|Un account di [Power automatici](https://flow.microsoft.com) attivo per l'amministratore del sistema CRM o verbi di sistema. L'utente deve accedere a [Power Automate](https://flow.microsoft.com) almeno una volta prima dell'installazione.|

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>Installare la sincronizzazione dei riferimenti del centro per i partner per Salesforce CRM

1. Passare a [Power automatici](https://flow.microsoft.com) e selezionare **ambienti** nell'angolo superiore destro. Vengono visualizzate le istanze di CRM disponibili.

2. Selezionare l'istanza di CRM appropriata dall'elenco a discesa nell'angolo in alto a destra. 

3. Selezionare **soluzioni** sulla barra di spostamento a sinistra.

4. Fare clic sul collegamento **Apri AppSource** nel menu in alto.

![Apri AppSource](images/cosellconnectors/openappsource.png)

5. Cercare **connettori per i riferimenti del centro per i partner per Salesforce** nella schermata popup.  

6. Fai clic sul pulsante **Get it Now (Ottieni ora** ) e **continua**. 

7. Verrà visualizzata la pagina in cui è possibile selezionare l'ambiente CRM (Dynamics 365) per installare l'applicazione.  Accettare i termini e le condizioni. 

8. Si verrà quindi indirizzati alla pagina **Gestisci soluzioni** .  Passare a "centro per i partner" usando i pulsanti freccia nella parte inferiore della pagina. L' **installazione pianificata** verrà visualizzata accanto alla soluzione di riferimento del centro per i partner. L'installazione può richiedere 10-15 minuti. 

9. Al termine dell'installazione, tornare a [Power automatizzate](https://flow.microsoft.com) e selezionare **soluzioni** dall'area di spostamento a sinistra. Si noti che la **sincronizzazione dei riferimenti del centro per i partner per Salesforce** è disponibile nell'elenco soluzioni.

10. Selezionare **la sincronizzazione dei riferimenti del centro per i partner per Dynamics 365**. Sono disponibili i flussi e le entità seguenti per l'automazione dell'energia elettrica:

![DISPONGONO disponibili](images/cosellconnectors/dynamics-available-crms.png)

## <a name="best-practice-test-before-you-go-live"></a>Procedura consigliata: testare prima di iniziare

Prima di installare, configurare e personalizzare la soluzione Power automatizzate nell'ambiente di produzione, assicurarsi di testare la soluzione in un'istanza di CRM di staging.

- Installare la soluzione Microsoft Power automatizzate in un ambiente di gestione temporanea o in un'istanza di CRM.
- Creare una copia della soluzione ed eseguire la configurazione e Power automatizzare le personalizzazioni dei flussi nell'ambiente di gestione temporanea.
- Testare la soluzione in un'istanza di staging/CRM. 
- In caso di esito positivo, importare come soluzione gestita nell'istanza di produzione. 

## <a name="configure-the-solution"></a>Configurare la soluzione

1. Dopo aver installato la soluzione nell'istanza di CRM, tornare a [Power automatizzate](https://flow.microsoft.com/).

2. Dall'elenco a discesa **ambienti** nell'angolo superiore destro selezionare l'istanza di CRM in cui è stata installata la soluzione Power automatizzate.

3. Sarà necessario creare connessioni che associano i tre account utente: 

- Utente del centro per i partner con credenziali di amministratore per i riferimenti 
- Eventi del Centro per i partner
- L'amministratore di CRM con la funzionalità Power automatizza i flussi nella soluzione. 

    a. Selezionare **Connections (connessioni** ) dalla barra di spostamento a sinistra e selezionare la soluzione "Partner Center referrals" dall'elenco.
    b. Creare una connessione facendo clic su **Crea una connessione**. 

    ![Creare la connessione](images/cosellconnectors/createconnection.png)

    c. Cercare i riferimenti per il centro per i **partner (anteprima)** nella barra di ricerca nell'angolo superiore destro.
    d. Creare una connessione per l'utente del centro per i partner con il ruolo delle credenziali di amministratore dei riferimenti. e. Successivamente, creare una connessione per gli eventi del centro partner per l'utente del centro per i partner con le credenziali di amministratore dei riferimenti. f. Creare una connessione per Common Data Service (ambiente corrente) per l'utente amministratore CRM.

4. Per associare i flussi di automazione dell'alimentazione con le connessioni, modificare ognuno dei flussi di automazione dell'alimentazione per connettersi a Common Data Service e ai riferimenti del centro per i partner. Salvare le modifiche.

5. **Attivare** i flussi di automazione dell'alimentazione.

## <a name="next-steps"></a>Passaggi successivi

- [Usare i webhook per ottenere gli eventi di modifica delle risorse](referral-connector-webhooks.md)

- [Altre informazioni sulla piattaforma Microsoft Power automatizzate?](https://docs.microsoft.com/power-automate/)

- [Gestire lead](manage-leads.md)

- [Gestire opportunità di co-selling](manage-co-sell-opportunities.md)
