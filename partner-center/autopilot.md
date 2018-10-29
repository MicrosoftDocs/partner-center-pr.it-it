---
title: Semplificare la configurazione del dispositivo con Windows Autopilot | Centro per i partner
ms.topic: article
ms.date: 10/29/2018
description: Aggiungi un profilo di distribuzione di Windows Autopilot nel Centro per i partner per semplificare la configurazione del dispositivo con Windows Autopilot
author: KPacquer
ms.author: kenpacq
keywords: autopilot, windows autopilot, autopilot microsoft, distribuzione automatica, configurazione guidata, schermate di accesso
ms.localizationpriority: medium
ms.openlocfilehash: 2c8e8953fbb79493a3704c9c8ea6982928c3fe92
ms.sourcegitcommit: ed22f6825d3af1d19385198b4d511e4b39d5e353
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/29/2018
ms.locfileid: "5796654"
---
# <a name="simplify-device-setup-with-windows-autopilot"></a>Semplifica la configurazione del dispositivo con Windows Autopilot 

Windows Autopilot semplifica e protegge la configurazione per i nuovi dispositivi Windows 10 Pro dal primo avvio, in soli pochi passaggi. Per ulteriori informazioni, consulta [Panoramica di Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot).

## <a name="features"></a>Funzionalità

*  **Disabilitazione delle autorizzazioni di amministratore locale** per gli utenti finali che impostano i dispositivi
*  **Visualizzazione della pagina di accesso dell'organizzazione**. L'organizzazione può impostare una pagina di accesso che aggiunga il dispositivo come dispositivo di lavoro e lo aggiunga ad Azure Active Directory.
*  **Registrazione del dispositivo in una Gestione dispositivi mobili (MDM)**, ad esempio Microsoft Intune, al termine della configurazione guidata.
*  **Semplificazione della configurazione guidata** in modo da utilizzare solo i passaggi e le decisioni necessari, mediante un profilo di distribuzione di Windows Autopilot. 

## <a name="requirements"></a>Requisiti

*  Dispositivi pre-installati con Windows 10 Pro Creators Update (versione 1703 o versione successiva) o Windows 10 Pro per i PC avanzati.
*  Identificatore dispositivo noto come hash hardware (128 HWH o 4K HWH), che in genere viene fornito da un OEM. Gli identificatori verranno usati per assegnare i profili dell'organizzazione nel centro per i Partner. 
*  I dispositivi devono avere accesso a Internet. Se il dispositivo non è in grado di connettersi, vengono mostrate le schermate della Configurazione guidata di Windows predefinite.
*  Per registrare un dispositivo in un'istanza di MDM è necessario Azure Active Directory Premium.

## <a name="add-organization-login-pages-to-oobe"></a>Aggiungere pagine di accesso dell'organizzazione alla Configurazione guidata

Per aggiungere pagine specifiche dell'organizzazione, aggiungi i dispositivi nella [directory di Azure AD](https://go.microsoft.com/fwlink/?linkid=848958) dell'organizzazione e crea le pagine di accesso.


## <a name="remove-windows-pages-from-oobe-with-a-windows-autopilot-deployment-profile"></a>Rimuovi le pagine di Windows dalla Configurazione guidata con un profilo di distribuzione di Windows Autopilot

**Esempi di impostazioni in un profilo di distribuzione di Windows Autopilot**
*  Ignora le impostazioni della privacy durante la configurazione
*  Disabilitare l'account amministratore locale durante la configurazione
*  Ignorare automaticamente le pagine durante la configurazione
   *  Selezionare automaticamente la configurazione per l'azienda o l'istituto di istruzione
   *  Ignorare le pagine di configurazione per la registrazione di Cortana, OneDrive e OEM

### <a name="add-devices-and-apply-a-profile"></a>Aggiungi i dispositivi e applica un profilo

Centro per i Partner, puoi creare un profilo Windows AutoPilot deployment e applicarlo a un elenco dei dispositivi.

Per configurare i dispositivi, caricane l'elenco, crea un profilo valido per i dispositivi e applicalo.

1.  Aggiungi l'elenco dei dispositivi.

    Agenti di vendita e agenti amministratore dispongono dell'accesso per aggiungere l'elenco dei dispositivi nel Centro per i partner.
    
    I rivenditori indiretti possono collaborare con il provider indiretto per aggiungere l'elenco.

    a.  Crea un file CSV utilizzando lo script di PowerShell dall'argomento: [Panoramica di Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot). Il file CSV contiene informazioni sul dispositivo, inclusi il numero di serie, il nome dell'OEM, il nome del modello, l'ID prodotto e l'identificatore del dispositivo. 

    b.  Dal centro per i Partner, Vai a **clienti** > Seleziona il cliente che riceve i dispositivi > **dispositivi > Aggiungi dispositivi**.

    c.  Assegna un nome al batch di dispositivi, ad esempio, "PC reparto vendite Contoso, ordine aprile 2017". 

    d.  Fai clic su **Sfoglia** > seleziona il file di informazioni sui dispositivi > **Convalida**.

    **Nota:** Se ricevi un messaggio di errore dopo aver tentato di caricare il file CSV, controlla il formato del file. Dopo agosto, puoi usare solo l'hash hardware o il nome dell'OEM, il numero di serie e il modello in tale ordine colonna oppure l'ID prodotto Windows. Puoi anche utilizzare il file CSV di esempio fornito dal collegamento accanto a **Aggiungi dispositivi**.

2.  Crea un profilo che è possibile applicare ai dispositivi. (Solo gli agenti amministratore hanno accesso a creare e applicare i profili nel centro per i Partner).

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

### <a name="you-can-remove-a-profile-from-a-device"></a>È possibile rimuovere un profilo da un dispositivo
1. Seleziona il dispositivo o batch di dispositivi da cui si desidera rimuovere il profilo. 

2. Nel riquadro **Assign and delete devices** selezionare **Rimuovi profilo**.

3. Vai al profilo che desideri rimuovere ed eliminalo. Il profilo verrà eliminato da tutti i dispositivi.

In **Dispositivi** seleziona il profilo. Da qui è possibile modificare le impostazioni esistenti.

## <a name="windows-autopilot-eula-dismissal--important-information"></a>Interruzione dell'EULA di Windows AutoPilot - Informazioni importanti

Questo strumento ti consente di configurare le singole installazioni di Windows nei dispositivi gestiti per i clienti. Se autorizzato dal cliente, puoi scegliere di non visualizzare o nascondere alcune schermate di installazione che normalmente vengono visualizzate agli utenti durante la configurazione di Windows, tra cui lo schermo di accettazione del contratto di licenza. 

Utilizzando questa funzione, accetti che eliminando o nascondendo le schermate progettate per offrire agli utenti l'avviso o l'accettazione delle condizioni confermi che hai ottenuto dal cliente il consenso e l'autorizzazione necessari per nascondere tali schermate e che, per conto del cliente (che si tratti di organizzazione o singolo utente), accetti gli avvisi e le condizioni applicabili per il cliente. Ciò include il contratto per le condizioni della licenza o dell'avviso che potrebbero essere presentati all'utente se non è stato scelto di non visualizzare o di nascondere usando questo strumento. Il cliente non può utilizzare il software Windows su tali dispositivi se non ha acquisito validamente una licenza per il software da Microsoft o dai distributori autorizzati.


