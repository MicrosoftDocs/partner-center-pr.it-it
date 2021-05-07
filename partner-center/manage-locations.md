---
title: Gestire le posizioni nell'account partner
ms.topic: how-to
ms.date: 05/01/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Informazioni su come aggiungere una nuova sede e come usare l'ID MNP di sede in programmi di incentivi, transazioni aziendali CSP, sottoscrizioni e altre transazioni.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8a2b4fa8b204b10d5d45c0e1409ab4bc463e272f
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702893"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a>Gestire le posizioni dell'account MPN e aggiungere (eliminare) una località


**Ruoli appropriati**

- Amministratore globale
- Amministratore degli account

L'ID MPN di sede identifica ogni specifica sede della società. L'ID MPN di sede viene usato per l'iscrizione a programmi di incentivi, per transazioni CSP e per altre transazioni aziendali. L'ID MPN globale viene usato per attività non transazionali, ad esempio richieste di supporto.

## <a name="the-following-scenario-is-typical"></a>Lo scenario seguente è tipico:

Contoso ha registrato il proprio account globale partner nel Regno Unito. Il PGA è l'azienda legale registrata e l'ID MPN globale viene usato per la gestione di tutte le attività non transazionali. Contoso ha anche account di sede partner, corrispondenti a filiali o divisioni in un'altra località del Regno Unito, della Francia o degli Stati Uniti. Nella struttura degli account MPN gli account di sede partner sono rappresentati come ID MPN di sede univoci. Gli account di sede partner vengono usati per attività transazionali, ad esempio programmi di incentivi o CSP. I pagamenti sono collegati a posizioni specifiche. 

>[!NOTE]
>Tra un tenant CSP e un ID MPN di sede esiste una relazione 1 a 1.

:::image type="content" source="images/locations/locations1.png" alt-text="Struttura delle sedi MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a>Prerequisiti per aggiungere un nuovo account per un'azienda CSP

Per aggiungere un nuovo account aziendale CSP, iniziare verificando di aver soddisfatto i prerequisiti.

1. È necessario avere un ID MPN della posizione nel paese in cui si vuole eseguire l'attività CSP. Per creare una nuova posizione MPN, leggere "Aggiungere una posizione MPN" di seguito.
  
1. Per creare una nuova registrazione CSP Indirect Reseller, vedere [Usare i provider indiretti](indirect-reseller-tasks-in-partner-center.md#get-started) 

>[!NOTE] 
 >Ricordarsi di accedere con le **nuove** credenziali per il **nuovo** account CSP. Non usare le credenziali esistenti perché il Centro per i partner riconoscerà l'utente che ha già un account.

2. Accettare il Contratto Microsoft Partner e attivare l'account.

1. Per registrarsi come partner con fatturazione diretta, vedere [Requisiti per i partner con fatturazione diretta](direct-partner-new-requirements.md)

## <a name="view-and-update-your-mpn-locations"></a>Visualizzare e aggiornare le località MPN

1. Accedere al dashboard Partner Center [con](https://partner.microsoft.com/dashboard/home) le credenziali dell'account MPN. Le credenziali MPN potrebbero essere diverse dalle credenziali CSP. 
 
1. **Dall'icona Impostazioni** selezionare **Impostazioni account,** **Profilo organizzazione,** **Note legali.** 

1. Nella scheda **Partner** verificare che non sia presente un messaggio di errore banner in cui viene chiesto di correggere i percorsi migrati da PMC.  Se le posizioni non sono state configurate correttamente in PMC e non sono ancora state aggiornate al PC, è necessario aggiornare tali posizioni.

:::image type="content" source="images/locations/location-two.png" alt-text="Screencap mostra come aggiornare la posizione.":::
 
4.  Nella schermata **Review PMC locations (Verifica posizioni PMC)** selezionare Update **(Aggiorna).**
Aggiornare i campi seguenti:

- **Campo Nome:** assicurarsi che il nome della località aziendale sia corretto. Se viene visualizzato un errore duplicato, provare a cambiare, ad esempio, da Contoso a Contoso, Inc.

- **Campo Persona giuridica:** assicurarsi di aver scelto la persona giuridica a cui è associata la località

- **Riga indirizzo 1 & 2 campi**: assicurarsi che l'indirizzo sia corretto

- **City & State/Province :** assicurarsi che la combinazione tra la città e lo stato/provincia sia corretta. In alcuni paesi verrà applicato il menu a discesa per la scelta dello stato/provincia e in altri paesi il campo dovrà essere inserito manualmente.

- **Campo CAP:** assicurarsi che il campo CAP sia corrispondente al paese, all'area geografica, alla città o all'indirizzo indicato.

- **Campi** relativi alle informazioni di contatto primarie: assicurarsi che i campi nome e cognome siano compilati e che l'indirizzo di posta elettronica indicato sia un indirizzo di posta elettronica dell'lavoro e non personale (ad esempio, , e così @outlook.com @live.com via).

- **Campo Numero di telefono:** assicurarsi che il numero di telefono NON includa caratteri speciali, spazi o codice paese. Il valore immesso nel campo Numero di telefono conterrà sempre un massimo di 10 caratteri.

5. Se non viene visualizzato un messaggio di errore, in  **Impostazioni** selezionare  **Impostazioni account**, **Profilo organizzazione**, **Identificatori**.

6. Trovare l'ID MPN con tipo "Location" corrispondente al paese di questo account CSP e usarlo per completare l'associazione.

7. Se non è possibile trovare l'ID MPN della posizione corrispondente all'account CSP che si vuole usare, è possibile aggiungere una nuova posizione, che creerà un nuovo ID MPN. Vedere **Aggiungere un percorso MPN di** seguito.

## <a name="add-an-mpn-location"></a>Aggiungere una sede MPN

1. Accedere usando l'account MPN in Partner Center. Le credenziali MPN potrebbero essere diverse dalle credenziali CSP. L'account MPN deve avere i privilegi di amministratore globale o amministratore account. 

1. **Dall'icona Impostazioni** selezionare Impostazioni **account e** quindi Profilo **organizzazione.**

2. Selezionare **Legale** e quindi nella **scheda Partner** selezionare Località aziendali e **fare** clic su Aggiungi **una località.**

3. Specificare i dettagli necessari, inclusi il nome dell'azienda, l'indirizzo e il contatto per la località che si vuole aggiungere all'azienda.
 
1. Fare clic **su Aggiungi percorso**. Verrà creato un nuovo ID MPN per la nuova località che è possibile usare per le transazioni e gli incentivi CSP.

:::image type="content" source="images/legal-biz.png" alt-text="Aggiungere una nuova azienda legale":::

> [!NOTE]
> Dopo aver aggiunto un percorso in Partner Center, non è possibile rimuoverlo. Se l'accesso è stato effettuato con l'account corretto, verrà visualizzato **MPN** nel menu a sinistra del Centro per i partner.

## <a name="add-the-registration-number-id"></a>Aggiungere l'ID del numero di registrazione

Se si è un provider indiretto, un partner con fatturazione diretta o un rivenditore indiretto e si collabora con clienti nuovi o esistenti nei paesi seguenti, è necessario fornire i numeri ID di registrazione per l'azienda. Se il paese in cui si sta effettuando la società non è elencato di seguito, l'ID registrazione è facoltativo.

- Armenia 
- Azerbaigian 
- Bielorussia 
- Brasile 
- Ungheria 
- India 
- Iraq 
- Kazakhstan 
- Kirghizistan 
- Moldova 
- Myanmar 
- Polonia 
- Russia 
- Arabia Saudita 
- Sudafrica 
- Sud Sudan  
- Tagikistan 
- Thailandia
- Turchia 
- Ucraina 
- Emirati Arabi Uniti 
- Uzbekistan 
- Venezuela
- Vietnam 


Per altre informazioni, vedere Informazioni [sul numero ID registrazione](reg-number-id.md)

## <a name="delete-a-location"></a>Eliminare una località

Per eliminare una località dall'account, è necessario contattare il [supporto per i partner.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b) Assicurarsi di comprendere l'impatto di questa azione. Le posizioni eliminate non possono essere recuperate e qualsiasi elemento associato a tale ID MPN specifico non verrà più riconosciuto o sarà attivo per l'azienda.

## <a name="change-country-of-partner-global-account"></a>Cambiare il paese dell'account globale del partner 

1. Accedere con l'account MPN Partner Center. Le credenziali MPN potrebbero essere diverse dalle credenziali CSP. L'account MPN deve avere i privilegi di amministratore globale o amministratore account. 

2. Nella scheda **Partner** passare a **Località aziendali** e controllare l'elenco delle località per assicurarsi che sia elencata la località desiderata come persona legale. 
 
1. Per aggiungere una località, fare clic su Aggiungi una località e, nel riquadro a comparsa, specificare i dettagli necessari, inclusi il nome dell'azienda, l'indirizzo e il contatto principale per la località che si vuole aggiungere all'azienda. 
 
1. Selezionare **Cambia paese accanto** all'elenco a discesa **Paese/area** geografica e seguire la procedura. 

:::image type="content" source="images/lbp.png" alt-text="Riquadro a comparsa dei dati del profilo di business legale":::

5. Fare clic su **Salva**.

6. Il paese dell'account globale MPN verrà modificato nel nuovo paese legale.
  
## <a name="next-steps"></a>Passaggi successivi

- Vedere le informazioni sul [processo di verifica](verification-responses.md).
