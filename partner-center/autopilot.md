---
title: Semplificare la configurazione del dispositivo con Windows Autopilot | Centro per i partner
ms.topic: article
ms.date: 10/29/2018
description: Aggiungi un profilo di distribuzione di Windows Autopilot nel Centro per i partner per semplificare la configurazione del dispositivo con Windows Autopilot
author: KPacquer
ms.author: kenpacq
keywords: autopilot, windows autopilot, autopilot microsoft, distribuzione automatica, configurazione guidata, schermate di accesso
ms.localizationpriority: medium
ms.openlocfilehash: 3d6e6e015424eb8be83bae21b2e15bdc072e480b
ms.sourcegitcommit: 777225c8bf16e4a8811a9d88aceb45fcba1cd959
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/11/2018
ms.locfileid: "8917563"
---
<!--Maggie, 12/7/18 - removed line telling indirect resellers to go through their indirect providers for autopilot stuff as per Bhavya Chopra in bug 19841770.-->

# <a name="simplify-device-setup-with-windows-autopilot"></a>Semplifica la configurazione del dispositivo con Windows Autopilot 

Windows Autopilot semplifica e protegge la configurazione per i nuovi dispositivi Windows 10 Pro dal primo avvio, in soli pochi passaggi. Per ulteriori informazioni, consulta [Panoramica di Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot).

## <a name="features"></a>Funzionalità

- **Disabilitazione delle autorizzazioni di amministratore locale** per gli utenti finali che impostano i dispositivi
- **Visualizzazione della pagina di accesso dell'organizzazione**. L'organizzazione pre-definire una pagina di accesso che aggiunge il dispositivo come dispositivo di lavoro e aggiunge il dispositivo con Azure Active Directory.
- **Registrazione del dispositivo in una Gestione dispositivi mobili (MDM)**, ad esempio Microsoft Intune, al termine della configurazione guidata.
- **Semplificazione della configurazione guidata** in modo da utilizzare solo i passaggi e le decisioni necessari, mediante un profilo di distribuzione di Windows Autopilot.

## <a name="requirements"></a>Requisiti

- Dispositivi pre-installati con Windows 10 Pro Creators Update (versione 1703 o versione successiva) o Windows 10 Pro per i PC avanzati.
- Identificatore dispositivo noto come hash hardware (128 HWH o 4K HWH), che in genere viene fornito da un OEM. Gli identificatori verranno usati per assegnare i profili dell'organizzazione nel centro per i Partner.
- I dispositivi devono avere accesso a Internet. Se il dispositivo non è in grado di connettersi, vengono mostrate le schermate della Configurazione guidata di Windows predefinite.
- Per registrare un dispositivo in un'istanza di MDM è necessario Azure Active Directory Premium.

## <a name="add-company-branded-sign-in-pages-to-oobe"></a>Aggiungere pagine di marchio della società Accedi alla configurazione guidata

Per aggiungere pagine specifiche della società, aggiungere i dispositivi [directory di Azure AD della tua azienda](https://go.microsoft.com/fwlink/?linkid=848958) e crea le pagine di accesso.

## <a name="remove-windows-pages-from-oobe-with-a-windows-autopilot-deployment-profile"></a>Rimuovi le pagine di Windows dalla Configurazione guidata con un profilo di distribuzione di Windows Autopilot

### <a name="examples-of-settings-in-a-windows-autopilot-deployment-profile"></a>Esempi di impostazioni in un profilo di distribuzione di Windows Autopilot

- Ignora le impostazioni della privacy durante la configurazione
- Disabilitare l'account amministratore locale durante la configurazione
- Ignorare automaticamente le pagine durante la configurazione
  - Selezionare automaticamente la configurazione per l'azienda o l'istituto di istruzione
  - Ignorare le pagine di configurazione per la registrazione di Cortana, OneDrive e OEM

### <a name="add-devices-and-apply-a-profile"></a>Aggiungi i dispositivi e applica un profilo

Centro per i Partner, puoi creare un profilo Windows AutoPilot deployment e applicarlo a un elenco dei dispositivi.

Per configurare i dispositivi, caricane l'elenco, crea un profilo valido per i dispositivi e applicalo.

1.  Aggiungi l'elenco dei dispositivi.

    Agenti di vendita e agenti amministratore dispongono dell'accesso per aggiungere l'elenco dei dispositivi nel Centro per i partner.

    a. Creare un file con estensione csv usando lo script di PowerShell dall'argomento della [Panoramica di Windows AutoPilot](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot). Il file CSV contiene informazioni sul dispositivo, inclusi il numero di serie, il nome dell'OEM, il nome del modello, l'ID prodotto e l'identificatore del dispositivo. 

    b. Dal centro per i Partner, Vai a **clienti** > Seleziona il cliente che riceve i dispositivi > **dispositivi > Aggiungi dispositivi**.

    c. Assegna un nome al batch di dispositivi, ad esempio, "PC reparto vendite Contoso, ordine aprile 2017". 

    d. Selezionare **Sfoglia** > Seleziona il file di informazioni sui dispositivi > **convalida**.

    **Nota:** Se ricevi un messaggio di errore dopo aver tentato di caricare il file CSV, controlla il formato del file. Dopo agosto, puoi usare solo l'hash hardware o il nome dell'OEM, il numero di serie e il modello in tale ordine colonna oppure l'ID prodotto Windows. Puoi anche utilizzare il file CSV di esempio fornito dal collegamento accanto a **Aggiungi dispositivi**.

2.  Crea un profilo che è possibile applicare ai dispositivi. (Solo gli agenti amministratore hanno accesso a creare e applicare i profili nel centro per i Partner).

    a.  Dai **dispositivi**, selezionare **Aggiungi nuovo profilo**.

    b.  Assegna un nome al profilo, ad esempio "Profilo desktop Contoso – Ignora Configurazione guidata".

    c.  Configura le impostazioni della Configurazione guidata. Ad esempio, seleziona **Skip Express Settings in setup**.

    d.  Seleziona **Invia**.

3.  Applica il profilo.

    a.  In **Dispositivi** nel riquadro **Assign and delete devices**, seleziona i dispositivi che si desidera configurare. Per selezionare un intero batch, selezionare la casella di controllo accanto al nome del batch (ad esempio, "PC reparto vendite Contoso, ordine di marzo 2017").

    b.  Selezionare **Applica profilo**e seleziona il profilo (ad esempio, "Contoso Desktop profilo – Ignora configurazione guidata"). Per i dispositivi, il profilo verrà mostrato nella colonna Profilo.

4.  Facoltativo: verifica il corretto funzionamento del profilo.

    a.  Connettere un dispositivo alla rete e quindi accendilo.

    b.  Verifica che siano visualizzate le eventuali schermate appropriate della Configurazione guidata.

    c.  Per preparare il dispositivo per un nuovo utente, completa l'esperienza della Configurazione guidata, quindi ripristina le impostazioni predefinite di fabbrica del dispositivo.

## <a name="to-update-or-delete-a-profile"></a>Per aggiornare o eliminare un profilo 

Dopo aver assegnato un profilo a un dispositivo, è possibile aggiornare, anche se il dispositivo è già stato fornito al cliente. Quando il dispositivo si connette a Internet, scarica la versione più recente del profilo durante il processo della Configurazione guidata. Se il cliente ripristina le impostazioni predefinite di fabbrica del dispositivo, gli aggiornamenti più recenti apportati al tuo profilo verranno di nuovo scaricati dal dispositivo. 

### <a name="remove-a-profile-from-a-device"></a>Rimuovere un profilo da un dispositivo

1. Seleziona il dispositivo o batch di dispositivi da cui si desidera rimuovere il profilo. 

2. Nel riquadro **Assign and delete devices** selezionare **Rimuovi profilo**.

3. Vai al profilo che desideri rimuovere ed eliminalo. Il profilo verrà eliminato da tutti i dispositivi.

In **Dispositivi** seleziona il profilo. Da qui è possibile modificare le impostazioni esistenti.

## <a name="windows-autopilot-eula-dismissal--important-information"></a>Interruzione dell'EULA di Windows AutoPilot - Informazioni importanti

Questo strumento ti consente di configurare le singole installazioni di Windows nei dispositivi gestiti per i clienti. Se autorizzato dal cliente, puoi scegliere di non visualizzare o nascondere alcune schermate di installazione che normalmente vengono visualizzate agli utenti durante la configurazione di Windows, tra cui lo schermo di accettazione del contratto di licenza. 

Utilizzando questa funzione, accetti che eliminando o nascondendo le schermate progettate per offrire agli utenti l'avviso o l'accettazione delle condizioni confermi che hai ottenuto dal cliente il consenso e l'autorizzazione necessari per nascondere tali schermate e che, per conto del cliente (che si tratti di organizzazione o singolo utente), accetti gli avvisi e le condizioni applicabili per il cliente. Ciò include il contratto per le condizioni della licenza o dell'avviso che potrebbero essere presentati all'utente se non è stato scelto di non visualizzare o di nascondere usando questo strumento. Il cliente non può utilizzare il software Windows su tali dispositivi se non ha acquisito validamente una licenza per il software da Microsoft o dai distributori autorizzati.