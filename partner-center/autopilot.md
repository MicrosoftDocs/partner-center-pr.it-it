---
title: Personalizzare l'esperienza di un dispositivo
ms.topic: how-to
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Prima di distribuire il nuovo dispositivo di un cliente, è possibile usare i profili Windows Autopilot per personalizzare o pre-configurare l'esperienza predefinita del dispositivo.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 5294495403be729adecb5a7814ade4f9d454a0f6
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149826"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a>Usare i profili di Windows Autopilot nei nuovi dispositivi per personalizzare l'esperienza predefinita di un cliente

**Ruoli appropriati:** amministrazione dell'agente | Amministratore globale | Agente di vendita | Amministratore di gestione utenti

Se si gestiscono i dispositivi dei clienti, potrebbe essere necessario personalizzare l'esperienza predefinita (OOBE) per gli utenti del cliente. È possibile pre-configurare nuovi dispositivi con Windows Autopilot prima di recapitare i dispositivi ai clienti e applicare nuovi profili ai dispositivi che i clienti hanno già acquistato. 

Si noti che gli OEM hanno iniziato a includere un'etichetta di spedizione all'esterno della casella del dispositivo Autopilot che mostra l'ID del codice **Product Key (PKID) del dispositivo.**  Questo codice a barre leggibile unidimensionale offre ai partner downstream un modo per registrare i dispositivi per Autopilot senza dover disappiare i dispositivi e raccogliere l'ID dispositivo con mezzi alternativi.

Questo articolo illustra come creare e applicare profili Autopilot ai dispositivi in Partner Center.

Se non si ha già familiarità con Autopilot, vedere le informazioni in questi articoli:

- [Panoramica di Windows Autopilot](/windows/deployment/windows-10-auto-pilot)
- [Guida di riferimento alla distribuzione di Autopilot](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>Panoramica

Con la Windows Autopilot funzionalità in Partner Center, è possibile creare profili personalizzati da applicare ai dispositivi dei clienti. Al momento della pubblicazione di questo articolo erano disponibili le impostazioni del profilo seguenti:

- Ignorare le impostazioni di privacy. Questa impostazione del profilo Autopilot facoltativa consente alle organizzazioni di non chiedere informazioni sulle impostazioni di privacy durante il processo di configurazione guidata.

- Disabilitare la creazione dell'account amministratore locale nel dispositivo. Le organizzazioni possono decidere se l'utente che configura il dispositivo deve avere accesso come amministratore al termine del processo.

- Configurare automaticamente il dispositivo per l'istituto di istruzione o l'istituto di istruzione. Tutti i dispositivi registrati con Autopilot verranno automaticamente considerati dispositivi aziendali o dell'istituto di istruzione, quindi questa domanda non verrà posta durante il processo di configurazione.

- Ignorare le pagine di configurazione della registrazione di Cortana, OneDrive e OEM. Tutti i dispositivi registrati con Autopilot ignorano automaticamente queste pagine durante il processo di configurazione della configurazione automatica.

- Ignorare il Contratto di licenza con l'utente finale . A partire Windows 10 versione 1709, le organizzazioni possono decidere di ignorare la pagina EULA presentata durante il processo di configurazione. Per informazioni importanti su come ignorare la pagina [EULA durante](#windows-autopilot-eula-dismissal) l'installazione di Windows, vedere Windows Autopilot chiusura dell'EULA di seguito.

Si applicano le limitazioni e le autorizzazioni seguenti di gestione dei profili e dei dispositivi:

- I partner CSP possono continuare a gestire i profili di Autopilot per i clienti esistenti di cui sono rivenditori, anche se i clienti hanno rimosso i privilegi di amministrazione delegata del partner.

- È possibile gestire i dispositivi esistenti per i clienti aggiunti.

- Non è possibile gestire i dispositivi caricati dal cliente in Microsoft Store per le aziende o nel portale di Microsoft Intune.

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>Creare e gestire profili Autopilot in Partner Center

In Partner Center, è possibile creare Windows Autopilot di distribuzione e applicarli ai dispositivi.

>[!NOTE]
>Solo gli agenti amministratore possono creare e applicare profili.

### <a name="create-a-new-autopilot-profile"></a>Creare un nuovo profilo Autopilot

1. Selezionare **Clienti** dal menu Partner Center e quindi selezionare il cliente per cui si sta creando il profilo Autopilot.

2. Nella pagina dei dettagli del cliente selezionare **Dispositivi**.

3. In **Windows Autopilot profili selezionare** Aggiungi nuovo **profilo**.

4. Immettere il nome e la descrizione del profilo e quindi configurare le impostazioni di Configurazione guidata. Scegliere tra:  

   - Ignorare le impostazioni di privacy nella configurazione

   - Disabilitare l'account amministratore locale durante l'installazione
  
   - Ignorare automaticamente le pagine nella configurazione<br>
        (Include *la selezione automatica della configurazione per l'ambiente di lavoro o dell'istituto di* istruzione e ignora le pagine di configurazione della registrazione di *Cortana, OneDrive e OEM)*
  
   - Ignorare il contratto di licenza con l'utente finale (EULA)<br> 
       >[!IMPORTANT] 
       >Per informazioni importanti su come ignorare la pagina [EULA durante](#windows-autopilot-eula-dismissal) l'installazione di Windows, vedere Windows Autopilot chiusura dell'EULA di seguito.

5. Al **termine, selezionare** Invia.

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>Applicare un profilo Autopilot ai dispositivi dei clienti

>[!NOTE]
>Le istruzioni seguenti presuppongono che i dispositivi del cliente siano già stati aggiunti a Partner Center e che sia possibile accedere al relativo elenco di dispositivi. Se i dispositivi del cliente non sono ancora stati aggiunti, seguire le istruzioni riportate in Aggiungere dispositivi [all'account](#add-devices-to-a-customers-account) di un cliente e quindi seguire questa procedura.

Dopo aver creato un profilo autopilot per un cliente, è possibile applicarlo ai dispositivi del cliente.

1. Selezionare **Clienti** dal menu Partner Center e quindi selezionare il cliente per cui è stato creato il profilo autopilot.

2. Nella pagina dei dettagli del cliente selezionare **Dispositivi.**

3. In **Applica profili ai dispositivi** selezionare i dispositivi o i gruppi di dispositivi a cui si vogliono aggiungere profili e quindi selezionare Applica **profilo.** Il profilo appena applicato viene visualizzato nella **colonna** Profilo.

4. Seguire questa procedura per verificare che il profilo verrà applicato correttamente al dispositivo.

    a.  Connettere un dispositivo alla rete e attivarlo.

    b.  Verificare che vengano visualizzate le eventuali schermate appropriate della Configurazione guidata.

    c.  Quando il processo di Configurazione guidata si arresta, ripristinare le impostazioni predefinite del dispositivo per prepararlo per un nuovo utente.

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>Rimuovere un profilo di Autopilot dal dispositivo di un cliente

1. Selezionare **Clienti** dal menu Partner Center e quindi selezionare il cliente per cui è stato creato il profilo autopilot.

2. Nella pagina dei dettagli del cliente selezionare **Dispositivi.**

3. In **Applica profili ai dispositivi** selezionare i dispositivi da cui si vuole rimuovere il profilo e quindi selezionare Rimuovi **profilo.**

   >[!NOTE]
   >La rimozione di un profilo da un dispositivo non elimina il profilo dall'elenco. Se si vuole eliminare un profilo, seguire le istruzioni in [Aggiornare o eliminare un profilo di Autopilot.](#update-or-delete-an-autopilot-profile)

### <a name="update-or-delete-an-autopilot-profile"></a>Aggiornare o eliminare un profilo di Autopilot

Se un cliente vuole modificare l'esperienza predefinita dopo aver inviato i dispositivi, è possibile modificare il profilo in Partner Center.

Quando il dispositivo del cliente si connette a Internet, scarica la versione più recente del profilo durante il processo di Configurazione guidata. Inoltre, ogni volta che un cliente ripristina le impostazioni predefinite predefinite di un dispositivo, il dispositivo scaricherà di nuovo la versione più recente del profilo durante il processo di configurazione guidata.

1. Selezionare **Clienti** dal menu Partner Center e quindi selezionare il cliente che vuole modificare un profilo autopilot.

2. Nella pagina dei dettagli del cliente selezionare **Dispositivi**.

3. In **Windows Autopilot profili** selezionare il profilo da aggiornare. Apportare le modifiche necessarie e quindi selezionare **Invia**.

Per eliminare questo profilo, selezionare **Elimina profilo** nell'angolo superiore destro della pagina.

### <a name="add-devices-to-a-customers-account"></a>Aggiungere dispositivi all'account di un cliente

>[!NOTE]
>Gli agenti di vendita e gli agenti di amministrazione possono aggiungere dispositivi all'account di un cliente.

Prima di poter applicare profili Autopilot personalizzati ai dispositivi dei clienti, è necessario poter accedere all'elenco dei dispositivi del cliente.

Se si prevede di usare la combinazione di nome, numero di serie e modello OEM, tenere presenti queste limitazioni:

- Questa tupla funziona solo per i dispositivi più nuovi (hash 4k, ad esempio) e non è supportata per gli hash da 128b (RS2 e dispositivi precedenti).

- La registrazione della tupla fa distinzione tra maiuscole e  minuscole, quindi i dati nel file devono corrispondere ai nomi del modello e del produttore esattamente come fornito dal provider OEM (provider hardware).

Seguire le istruzioni seguenti per aggiungere dispositivi all'account di un cliente in Partner Center.

1. Selezionare **Clienti** dal menu Partner Center e quindi selezionare il cliente di cui si vuole gestire i dispositivi.

2. Nella pagina dei dettagli del cliente selezionare **Dispositivi**.

3. In **Applica profili ai dispositivi** selezionare Aggiungi **dispositivi**.

4. Immettere un nome per l'elenco di dispositivi e quindi selezionare Sfoglia per caricare l'elenco del cliente (in formato di file CSV) in Partner Center. 

    >[!NOTE]
    >Questo file CSV dovrebbe essere stato ricevuto con l'acquisto del dispositivo. Se non si riceve un file CSV, è possibile crearne uno manualmente seguendo la procedura [descritta](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)in Aggiunta di dispositivi a Windows Autopilot .  

5. Caricare il file CSV e quindi selezionare **Salva**.

Se si riceve un messaggio di errore mentre si tenta di caricare il file CSV, controllare il formato del file. È possibile usare solo l'hash hardware oppure il nome OEM, il numero di serie e il modello (nell'ordine di tale colonna) o l'ID del prodotto Windows. È anche possibile usare il file CSV di esempio fornito dal collegamento accanto ad **Aggiungi dispositivi** per creare un elenco di dispositivi.

Il file CSV dovrebbe essere simile al seguente:

> **Device Serial Number,Windows Product ID,Hardware Hash,Manufacturer name,Device model**

> **{serialNumber},,,Microsoft Corporation,Surface Laptop**

>[!NOTE]
> Per "Nome produttore" e "Modello di dispositivo" viene fatto distinzione tra maiuscole e minuscole.

Se non si conosce il valore da inserire per Nome produttore e Modello di dispositivo, è possibile eseguire questa operazione nel dispositivo per raccogliere i valori corretti:

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a>Windows Autopilot EULA dismissal

### <a name="important-information"></a>INFORMAZIONI IMPORTANTI

Windows Autopilot consente di configurare installazioni personalizzate di Windows nei dispositivi gestiti per i clienti. Se autorizzato dal cliente, è possibile eliminare o nascondere determinate schermate di configurazione che vengono normalmente presentate agli utenti durante la configurazione di Windows, inclusa la schermata di accettazione del contratto di licenza con l'utente finale.

Usando questa funzione, l'utente accetta di eliminare o nascondere eventuali schermate progettate per fornire agli utenti la comunicazione o l'accettazione delle condizioni significa che il cliente ha ottenuto un consenso e un'autorizzazione sufficienti per nascondere le condizioni e che, per conto del cliente (che possa trattarsi di un'organizzazione o di un singolo utente), acconsentire a eventuali comunicazioni e accettare le condizioni applicabili al cliente. Ciò include il contratto ai termini e alle condizioni della licenza o all'avviso che verrebbe presentato all'utente se non fosse stato eliminato o nascosto con questo strumento. Il cliente non può usare il software Windows su tali dispositivi se il cliente non ha acquistato in modo valido una licenza per il software da Microsoft o dai suoi distributori con licenza.