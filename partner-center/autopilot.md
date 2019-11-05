---
title: Personalizzare l'esperienza predefinita di un dispositivo con i profili di Windows Autopilot | Centro per i partner
description: Preconfigurare l'esperienza predefinita di un dispositivo con i profili Autopilot.
ms.topic: article
ms.date: 03/18/2019
author: maggiepuccievans
ms.author: evansma
keywords: Autopilot, Windows Autopilot, Microsoft Autopilot, distribuzione Zero-Touch, OOBE, schermate di accesso, predefinite
ms.localizationpriority: medium
ms.openlocfilehash: 7861efa8c0fd7e03488ba3f222fcb3a476c06cc2
ms.sourcegitcommit: 76c34fd8dc544cea93496079df68759a1da9098c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/04/2019
ms.locfileid: "73544049"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a>Personalizzare l'esperienza predefinita di un dispositivo con i profili di Windows Autopilot

**Si applica a**

- CSP Direct-fatturazione partner, provider indiretti e rivenditori indiretti

Se si gestiscono i dispositivi dei clienti, potrebbe essere necessario personalizzare l'esperienza predefinita per gli utenti del cliente. È possibile preconfigurare nuovi dispositivi con i profili di Windows Autopilot prima di consegnare i dispositivi ai clienti e applicare nuovi profili ai dispositivi che i clienti hanno già acquistato. 

Si noti che gli OEM hanno iniziato ad includere un'etichetta di spedizione all'esterno della casella dispositivo Autopilot che mostra l' **ID del codice Product Key (pkID)** del dispositivo.  Questo codice a barre leggibile e unidimensionale fornisce ai partner downstream un modo per registrare i dispositivi per Autopilot senza dover sottoporre a unboxing i dispositivi e raccogliere l'ID del dispositivo in modo alternativo.

Questo articolo illustra come creare e applicare i profili di Autopilot ai dispositivi nel centro per i partner.

Se non si ha già familiarità con Autopilot, rivedere le informazioni contenute in questi articoli:

- [Panoramica di Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [Guida di riferimento per la distribuzione di Autopilot](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>Panoramica

Con la funzionalità Windows Autopilot in centro per i partner, è possibile creare profili personalizzati da applicare ai dispositivi dei clienti. Al momento della pubblicazione di questo articolo sono disponibili le impostazioni di profilo seguenti:

- Ignora le impostazioni di privacy. Questa impostazione facoltativa del profilo di Autopilot consente alle organizzazioni di non richiedere informazioni sulle impostazioni della privacy durante il processo di configurazione guidata.

- Disabilitare la creazione dell'account amministratore locale nel dispositivo. Le organizzazioni possono decidere se l'utente che configura il dispositivo deve avere l'accesso come amministratore al termine del processo.

- Configurare automaticamente il dispositivo per l'ufficio o l'Istituto di istruzione. Tutti i dispositivi registrati con Autopilot verranno considerati automaticamente dispositivi aziendali o dell'Istituto di istruzione, pertanto questa domanda non verrà richiesta durante il processo di configurazione guidata.

- Ignorare le pagine di configurazione per la registrazione di Cortana, OneDrive e OEM. Tutti i dispositivi registrati con Autopilot ignoreranno automaticamente queste pagine durante il processo di configurazione guidata.

- Ignora il contratto di licenza con l'utente finale (EULA). A partire da Windows 10 versione 1709, le organizzazioni possono decidere di ignorare la pagina EULA visualizzata durante il processo di configurazione guidata. Per informazioni importanti su come ignorare la pagina di EULA durante l'installazione di Windows, vedere la pagina relativa al [contratto di licenza di Windows Autopilot](#windows-autopilot-eula-dismissal) .

Si applicano le limitazioni e le autorizzazioni di gestione dei profili e dei dispositivi seguenti:

- I partner CSP possono continuare a gestire i profili di Autopilot per i clienti esistenti con le relazioni rivenditore, anche se i clienti hanno rimosso i privilegi di amministrazione delegata del partner.

- È possibile gestire i dispositivi esistenti per i clienti aggiunti.

- Non è possibile gestire i dispositivi caricati dal cliente in Microsoft Store for business o nel portale di Microsoft Intune.

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>Creare e gestire i profili di Autopilot nel centro per i partner

Nel centro per i partner è possibile creare profili di distribuzione di Windows Autopilot e applicarli ai dispositivi.

>[!NOTE]
>Solo gli agenti amministratori possono creare e applicare profili.

### <a name="create-a-new-autopilot-profile"></a>Crea un nuovo profilo di Autopilot

1. Selezionare **Customers (clienti** ) dal menu centro partner e quindi selezionare il cliente per il quale si sta creando il profilo di Autopilot.

2. Nella pagina dei dettagli del cliente selezionare **Devices (dispositivi**).

3. In **profili di Windows Autopilot** selezionare **Aggiungi nuovo profilo**.

4. Immettere il nome e la descrizione del profilo e quindi configurare le impostazioni della configurazione guidata. Scegliere tra:  

   - Ignora le impostazioni di privacy nel programma di installazione

   - Disabilitare l'account amministratore locale durante la configurazione
  
   - Ignorare automaticamente le pagine durante la configurazione<br>
        (Include *automaticamente seleziona configurazione per lavoro o scuola* e *Ignora le pagine di configurazione per la registrazione di Cortana, OneDrive e OEM*)
  
   - Ignora il contratto di licenza con l'utente finale (EULA)<br> 
       >[!IMPORTANT] 
       >Per informazioni importanti su come ignorare la pagina di EULA durante l'installazione di Windows, vedere la pagina relativa al [contratto di licenza di Windows Autopilot](#windows-autopilot-eula-dismissal) .

5. Al termine seleziona **Invia**.

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>Applicare un profilo di Autopilot ai dispositivi dei clienti

>[!NOTE]
>Le istruzioni seguenti presuppongono che siano già stati aggiunti i dispositivi del cliente al centro per i partner e che sia possibile accedere all'elenco di dispositivi. Se non sono stati ancora aggiunti i dispositivi del cliente, seguire le istruzioni riportate in [aggiungere dispositivi a un account del cliente](#add-devices-to-a-customers-account) e quindi seguire questa procedura.

Dopo aver creato un profilo di Autopilot per un cliente, è possibile applicarlo ai dispositivi del cliente.

1. Selezionare **Customers** dal menu centro partner e quindi selezionare il cliente per cui è stato creato il profilo Autopilot.

2. Nella pagina dei dettagli del cliente selezionare **Devices (dispositivi**).

3. In **applica profili ai dispositivi** selezionare i dispositivi o i gruppi di dispositivi a cui si vogliono aggiungere i profili e quindi selezionare **Applica profilo**. Il profilo appena applicato viene visualizzato nella colonna **profilo** .

4. Attenersi alla procedura seguente per verificare che il profilo venga applicato correttamente al dispositivo.

    a.  Connettere un dispositivo alla rete e attivarlo.

    b.  Verifica che siano visualizzate le eventuali schermate appropriate della Configurazione guidata.

    c.  Quando il processo OOBE si interrompe, ripristinare le impostazioni predefinite del dispositivo per prepararlo per un nuovo utente.

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>Rimuovere un profilo di Autopilot dal dispositivo di un cliente

1. Selezionare **Customers** dal menu centro partner e quindi selezionare il cliente per cui è stato creato il profilo Autopilot.

2. Nella pagina dei dettagli del cliente selezionare **Devices (dispositivi**).

3. In **applica profili ai dispositivi** selezionare i dispositivi da cui si desidera rimuovere il profilo, quindi selezionare **Rimuovi profilo**.

   >[!NOTE]
   >La rimozione di un profilo da un dispositivo non comporta l'eliminazione del profilo dall'elenco. Per eliminare un profilo, seguire le istruzioni riportate in [aggiornare o eliminare un profilo di Autopilot](#update-or-delete-an-autopilot-profile).

### <a name="update-or-delete-an-autopilot-profile"></a>Aggiornare o eliminare un profilo di Autopilot

Se un cliente vuole modificare l'esperienza predefinita dopo aver spedito i dispositivi, è possibile modificare il profilo nel centro per i partner.

Quando il dispositivo del cliente si connette a Internet, verrà scaricata la versione più recente del profilo durante il processo di configurazione guidata. Inoltre, ogni volta che un cliente Ripristina le impostazioni predefinite di un dispositivo, il dispositivo Scarica di nuovo la versione più recente del profilo durante il processo OOBE.

1. Selezionare **Customers** dal menu centro per i partner e quindi selezionare il cliente che desidera modificare un profilo di Autopilot.

2. Nella pagina dei dettagli del cliente selezionare **Devices (dispositivi**).

3. In **profili di Windows Autopilot** selezionare il profilo che si desidera aggiornare. Apportare le modifiche necessarie e quindi selezionare **Invia**.

Per eliminare questo profilo, selezionare **Elimina profilo** nell'angolo superiore destro della pagina.

### <a name="add-devices-to-a-customers-account"></a>Aggiungere dispositivi all'account di un cliente

>[!NOTE]
>Gli agenti di vendita e gli agenti di amministrazione possono aggiungere dispositivi a un account del cliente.

Prima di poter applicare profili Autopilot personalizzati ai dispositivi dei clienti, è necessario essere in grado di accedere all'elenco di dispositivi del cliente.

Se si prevede di utilizzare il nome OEM, il numero di serie e la combinazione di modelli, tenere presente queste limitazioni:

- Questa tupla funziona solo per i dispositivi più recenti (ad esempio, gli hash 4K) e non è supportata per gli hash 128B (RS2 e i dispositivi precedenti).

- Per la registrazione della tupla viene fatta distinzione tra maiuscole e minuscole, pertanto i dati nel file devono corrispondere ai nomi del modello e del produttore ***esattamente*** come fornito dal provider OEM (provider hardware).

Seguire le istruzioni riportate di seguito per aggiungere i dispositivi all'account di un cliente nel centro per i partner.

1. Selezionare **Customers (clienti** ) dal menu centro partner e quindi selezionare il cliente di cui si vogliono gestire i dispositivi.

2. Nella pagina dei dettagli del cliente selezionare **Devices (dispositivi**).

3. In **applica profili ai dispositivi** selezionare **Aggiungi dispositivi**.

4. Immettere un nome per l'elenco dei dispositivi e quindi selezionare **Sfoglia** per caricare l'elenco del cliente (in formato file CSV) nel centro per i partner.

    >[!NOTE]
    >Il file con estensione CSV è stato ricevuto con l'acquisto del dispositivo. Se non si riceve un file con estensione CSV, è possibile crearne uno seguendo i passaggi descritti in [aggiunta di dispositivi a Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).  

5. Caricare il file con estensione CSV e quindi selezionare **Save (Salva**).

Se viene ricevuto un messaggio di errore durante il tentativo di caricare il file CSV, controllare il formato del file. È possibile utilizzare solo l'hash hardware oppure il nome OEM, il numero di serie e il modello (nell'ordine di tale colonna) o l'ID del prodotto Windows. È anche possibile usare il file CSV di esempio fornito dal collegamento accanto a **Aggiungi dispositivi** per creare un elenco di dispositivi.

Il file CSV avrà un aspetto simile al seguente:

> **Numero di serie del dispositivo, ID prodotto Windows, hash hardware, nome produttore, modello di dispositivo**

> **{serialNumber},,, Microsoft Corporation, Surface laptop**

Si noti che "nome produttore" e "modello dispositivo" fanno distinzione tra maiuscole e minuscole.

Se non si conosce il valore da inserire per il nome del produttore e il modello di dispositivo, è possibile eseguire questa operazione sul dispositivo per raccogliere i valori corretti:

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a>Dismissing EULA di Windows Autopilot

### <a name="important-information"></a>INFORMAZIONI IMPORTANTI

Windows Autopilot consente di configurare installazioni personalizzate di Windows nei dispositivi gestiti per i clienti. Se il cliente è autorizzato a eseguire questa operazione, è possibile disattivare o nascondere alcune schermate di configurazione che in genere vengono presentate agli utenti durante la configurazione di Windows, inclusa la schermata di accettazione del contratto di licenza con l'utente finale (EULA).

Utilizzando questa funzione, l'utente accetta che l'eliminazione o la disattivazione delle schermate progettate per fornire agli utenti la comunicazione o l'accettazione delle condizioni significa che l'utente ha ottenuto il consenso e l'autorizzazione sufficienti per nascondere i termini e che l'utente, per conto di il cliente (indipendentemente dal fatto che si tratti di un'organizzazione o di un singolo utente come caso), acconsente a qualsiasi comunicazione e accetti le condizioni applicabili al cliente. Ciò include il contratto per le condizioni della licenza o dell'avviso che potrebbero essere presentati all'utente se non è stato scelto di non visualizzare o di nascondere usando questo strumento. Il cliente non può utilizzare il software Windows su tali dispositivi se non ha acquisito validamente una licenza per il software da Microsoft o dai distributori autorizzati.
