---
title: Aggiungere un profilo di distribuzione automatica per semplificare la configurazione del dispositivo con Windows Autopilot | Centro per i partner
description: Aggiungere un profilo di distribuzione automatica nel Centro per i partner per semplificare la configurazione del dispositivo con Windows Autopilot
author: KPacquer
keywords: autopilot, windows autopilot, autopilot microsoft, distribuzione automatica, distribuzione automatica, configurazione guidata, schermate di accesso
robots: NOINDEX,NOFOLLOW
ms.openlocfilehash: c51d9204b352b548a4095e96944aacdbcde97fa2
ms.sourcegitcommit: c2a12d6a18b9631916f6dd8301a4752ecc03296b
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 06/19/2017
---
# <a name="add-a-zero-touch-deployment-profile-to-simplify-device-setup-with-windows-autopilot"></a>Aggiungere un profilo di distribuzione automatica per semplificare la configurazione del dispositivo con Windows Autopilot

Windows Autopilot può semplificare e proteggere la configurazione per i nuovi dispositivi Windows 10 Pro dal primo avvio, in soli pochi passaggi. 

## <a name="features"></a>Funzionalità

*  **Disabilitazione delle autorizzazioni di amministratore locale** per gli utenti finali che impostano i dispositivi
*  **Visualizzazione della pagina di accesso dell'organizzazione**. L'organizzazione può impostare una pagina di accesso che aggiunge il dispositivo come dispositivo di lavoro e lo aggiunge ad Azure Active Directory.
*  **Registrazione del dispositivo in un'istanza di MDM**, ad esempio Microsoft Intune, al termine della configurazione guidata.
*  **Semplificazione della configurazione guidata** in modo da utilizzare solo i passaggi e le decisioni necessari, mediante in profilo di distribuzione automatica. 

## <a name="requirements"></a>Requisiti

*  Dispositivi con Windows 10 Pro Creators Update (versione 1703 o versioni successive) preinstallato
*  Identificatore dispositivo noto come hash hardware (128 HWH o 4K HWH), che in genere viene fornito da un OEM. Gli identificatori verranno usati per assegnare i profili dell'organizzazione nel Centro per i partner.
*  I dispositivi devono avere accesso a Internet. Se il dispositivo non è in grado di connettersi, vengono mostrate le schermate della Configurazione guidata di Windows predefinite.
*  Per registrare un dispositivo in un'istanza di MDM è necessario Azure Active Directory Premium.

## <a name="add-organization-login-pages-to-oobe"></a>Aggiungere pagine di accesso dell'organizzazione alla Configurazione guidata

Per aggiungere pagine specifiche dell'organizzazione, aggiungi i dispositivi nella [directory di Azure AD](https://go.microsoft.com/fwlink/?linkid=848958) dell'organizzazione e crea le pagine di accesso.


## <a name="remove--windows-pages-from-oobe-with-a-zero-touch-deployment-ztd-profile"></a>Rimuovi le pagine di Windows dalla Configurazione guidata con un profilo di distribuzione automatica

### <a name="examples-of-settings-in-a-ztd-profile"></a>Esempi di impostazioni in un profilo di distribuzione automatica
*  Ignorare le impostazioni privacy durante la configurazione
*  Disabilitare l'account amministratore locale durante la configurazione
*  Ignorare automaticamente le pagine durante la configurazione
   *  Selezionare automaticamente la configurazione per l'azienda o l'istituto di istruzione
   *  Ignorare le pagine di configurazione per la registrazione di Cortana, OneDrive e OEM

### <a name="add-devices-and-apply-a-profile"></a>Aggiungere i dispositivi e applicare un profilo

Nel Centro per i partner puoi creare un profilo di distribuzione automatica e applicarlo a un elenco di dispositivi.

Per configurare i dispositivi, carica un elenco dei dispositivi nel Centro per i partner, crea un profilo valido per i dispositivi e applicalo.

1.  Aggiungi l'elenco dei dispositivi nel Centro per i partner. Agenti di vendita e agenti amministratore dispongono dell'accesso per aggiungere l'elenco dei dispositivi nel Centro per i partner.

    a.  Chiedi all'OEM un file CSV in cui sono elencati i nuovi dispositivi. Questo file contiene numero di serie, ID prodotto e identificatore dispositivo generati tramite lo strumento OEM Activation 3.0. 

    b.  Dal dashboard Centro per i partner, vai a **Clienti** > seleziona il cliente che riceve i dispositivi > **Dispositivi > Aggiungi dispositivi**.

    c.  Assegna un nome al batch di dispositivi, ad esempio, "PC reparto vendite Contoso, ordine aprile 2017". 

    d.  Fai clic su **Sfoglia** > seleziona il file di informazioni sui dispositivi > **Convalida**.

2.  Crea un profilo che è possibile applicare ai dispositivi. Solo gli agenti amministratore dispongono dell'accesso per creare e applicare i profili nel Centro per i partner.

    a.  Da **Dispositivi** fai clic su **Aggiungi nuovo profilo**.

    b.  Assegna un nome al profilo, ad esempio "Profilo desktop Contoso – Ignora Configurazione guidata".

    c.  Configura le impostazioni della Configurazione guidata. Ad esempio, seleziona **Skip Express Settings in setup**.

    d.  Fai clic su **Invia**.

3.  Applica il profilo.

    a.  In **Dispositivi** nel riquadro **Assign and delete devices**, seleziona i dispositivi che si desidera configurare. Per selezionare un intero batch, selezionare la casella di controllo accanto al nome del batch (ad esempio, "PC reparto vendite Contoso, ordine di marzo 2017").

    b.  Fai clic su **Apply profile**, seleziona il profilo (ad esempio, "Profilo desktop Contoso – Ignora Configurazione guidata"). Per i dispositivi, il profilo verrà mostrato nella colonna Profilo.

4.  Facoltativo: verifica il corretto funzionamento del profilo.

    a.  Connetti un dispositivo alla rete e accendilo.

    b.  Verifica che siano visualizzate le eventuali schermate appropriate della Configurazione guidata.

    c.  Per preparare il dispositivo per un nuovo utente, completa l'esperienza della Configurazione guidata, quindi ripristina le impostazioni predefinite di fabbrica del dispositivo.


## <a name="to-update-or-delete-a-profile"></a>Per aggiornare o eliminare un profilo 

Una volta assegnato un profilo a un dispositivo, è possibile aggiornarlo, anche se il dispositivo è già stato fornito al cliente. Quando il dispositivo si connette a Internet, scarica la versione più recente del profilo durante il processo della Configurazione guidata. Se il cliente ripristina le impostazioni predefinite di fabbrica del dispositivo, gli aggiornamenti più recenti apportati al tuo profilo verranno di nuovo scaricati dal dispositivo. 

###<a name="you-can-remove-a-profile-from-a-device"></a>È possibile rimuovere un profilo da un dispositivo
1. Seleziona il dispositivo o batch di dispositivi da cui si desidera rimuovere il profilo. 

2. Nel riquadro **Assign and delete devices** selezionare **Rimuovi profilo**.

3. Vai al profilo che desideri rimuovere ed eliminalo. Il profilo verrà eliminato da tutti i dispositivi.


In **Dispositivi** seleziona il profilo. Da qui è possibile modificare le impostazioni esistenti.

