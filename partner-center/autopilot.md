---
title: Personalizzare l'esperienza out-of-box di un dispositivo con i profili di Windows Autopilot | Centro per i partner
description: Preconfigurare esperienza out-of-box di un dispositivo con i profili Autopilot.
ms.topic: article
ms.date: 2/6/19
author: maggiepuccievans
ms.author: evansma
keywords: AutoPilot, autopilot windows, autopilot microsoft, distribuzione automatica, configurazione guidata, schermate di accesso, out-of-box
ms.localizationpriority: medium
ms.openlocfilehash: 62e83c63bb10c041549f5a09bc32bdae979d462d
ms.sourcegitcommit: 5251779c33378f9ef4735fcb7c91877339462b1e
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/07/2019
ms.locfileid: "9062279"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a>Personalizzare l'esperienza out-of-box di un dispositivo con i profili di Windows Autopilot

**Si applica a**

- I partner direct-fattura CSP, i provider indiretti e i rivenditori indiretti

Se si gestiscono i dispositivi dei clienti, devi personalizzare l'esperienza di out-of-box (OOBE) per gli utenti del cliente. Puoi pre-configurare nuovi dispositivi con i profili di Windows Autopilot prima della consegna i dispositivi per i clienti e applicare i profili di nuovo ai dispositivi i clienti hanno già acquistato. Questo articolo spiega come creare e applicare i profili Autopilot ai dispositivi nel centro per i Partner.

Se non sei già familiarità con Autopilot, controlla le informazioni in questi articoli:

- [Panoramica di Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [Guida di riferimento di distribuzione AutoPilot](http://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>Panoramica

Con la funzionalità di Windows Autopilot nel centro per i Partner, puoi creare profili personalizzati da applicare ai dispositivi dei clienti. Le seguenti impostazioni del profilo erano disponibili al momento della che pubblicazione di questo articolo:

- Ignorare le impostazioni di privacy. Questa impostazione facoltativa di profilo Autopilot consente alle organizzazioni di non chiedere informazioni sulle impostazioni di privacy durante il processo di configurazione guidata.

- Disabilitare la creazione di un account amministratore locale nel dispositivo. Le organizzazioni possono decidere se l'utente di configurare il dispositivo deve avere accesso come amministratore, una volta completato il processo.

- Configura automaticamente dispositivo per l'azienda o all'istituto di istruzione. Tutti i dispositivi registrati con Autopilot verranno automaticamente considerati aziendale o dell'istituto di istruzione dispositivi, in modo che questa domanda non verrà richiesto durante il processo di configurazione guidata.

- Ignorare le pagine di configurazione registrazione OEM, OneDrive e Cortana. Tutti i dispositivi registrati con Autopilot salterà automaticamente queste pagine durante il processo di out-of-box experience (OOBE).

- Ignora il contratto di licenza utente finale (EULA). A partire da Windows 10 versione 1709, le organizzazioni possono decidere di saltare la pagina di condizioni di licenza presentata durante il processo di configurazione guidata. Vedi l' [interruzione dell'EULA di Windows Autopilot](#windows-autopilot-eula-dismissal) seguito per informazioni importanti da prendere in considerazione su ignorare la pagina di condizioni di licenza durante l'installazione di Windows.

Applicano le autorizzazioni di gestione di profilo e del dispositivo e limitazioni seguenti:

- I partner CSP possono continuare a gestire i profili Autopilot per i clienti esistenti con cui hanno relazioni come rivenditore, anche se i clienti hanno rimosso i privilegi di privilegi di amministratore delegato del partner.

- È possibile gestire i dispositivi esistenti per i clienti che sono stati aggiunti da te o da un altro partner CSP.

- Non puoi gestire i dispositivi che caricati dal tuo cliente a Microsoft Store per le aziende o il portale di Microsoft Intune.

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>Creare e gestire i profili Autopilot nel centro per i Partner

Nel centro per i Partner, puoi creare profili di distribuzione Windows Autopilot e applicarli ai dispositivi.

>[!NOTE]
>Solo gli agenti amministratore possono creare e applicare i profili.

### <a name="create-a-new-autopilot-profile"></a>Creare un nuovo profilo Autopilot

1. Seleziona **clienti** dal menu di Centro per i Partner e quindi seleziona il cliente per che quando crei il profilo Autopilot.

2. Nella pagina dei dettagli del cliente, seleziona **i dispositivi**.

3. Selezionare **Aggiungi nuovo profilo** **Windows Autopilot profili** .

4. Immetti nome e una descrizione del profilo e quindi Configura le impostazioni di configurazione guidata. Scegliere tra:  

   - Ignora impostazioni di privacy durante l'installazione

   - Disabilitare l'account amministratore locale durante la configurazione
  
   - Ignorare automaticamente le pagine durante la configurazione<br>
        (Include *Seleziona automaticamente la configurazione per l'azienda o all'istituto di istruzione* e *le pagine di configurazione registrazione OEM, OneDrive e Ignora Cortana*)
  
   - Ignora il contratto di licenza utente finale (EULA)<br> 
       >[!IMPORTANT] 
       >Vedi l' [interruzione dell'EULA di Windows Autopilot](#windows-autopilot-eula-dismissal) seguito per informazioni importanti da prendere in considerazione su ignorare la pagina di condizioni di licenza durante l'installazione di Windows.

5. Al termine seleziona **Invia**.

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>Applicare un profilo Autopilot ai dispositivi dei clienti

>[!NOTE]
>Le istruzioni seguenti presuppongono che hai già aggiunto i dispositivi del cliente nel centro per i Partner e che sia possibile accedere l'elenco di dispositivi. Se non lo hai già aggiunto i dispositivi del cliente, segui le istruzioni in [dispositivi Aggiungi all'account del cliente](#add-devices-to-a-customers-account) e quindi seguire i passaggi seguenti.

Dopo aver creato un profilo Autopilot per un cliente, puoi applicare ai dispositivi del cliente.

1. Seleziona **clienti** dal menu di Centro per i Partner e quindi seleziona il cliente per che è stato creato il profilo Autopilot.

2. Nella pagina dei dettagli del cliente, seleziona **i dispositivi**.

3. Selezionare i dispositivi o gruppi di dispositivi che vuoi aggiungere i profili e quindi selezionare **Applica profilo** **Applica profili ai dispositivi** . Il profilo che è stato applicato solo verrà visualizzato nella colonna **profilo** .

4. Segui i passaggi seguenti per verificare che il profilo verrà applicato correttamente nel dispositivo.

    a.  Connettere un dispositivo alla rete e accendilo.

    b.  Verifica che siano visualizzate le eventuali schermate appropriate della Configurazione guidata.

    c.  Quando si interrompe il processo di configurazione guidata, reimpostare il dispositivo per impostazioni predefinite di fabbrica per prepararla per un nuovo utente.

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>Rimuovere un profilo Autopilot dal dispositivo del cliente

1. Seleziona **clienti** dal menu di Centro per i Partner e quindi seleziona il cliente per che è stato creato il profilo Autopilot.

2. Nella pagina dei dettagli del cliente, seleziona **i dispositivi**.

3. Selezionare i dispositivi che vuoi rimuovere il profilo e quindi seleziona **rimuovere profilo** **Applica profili ai dispositivi** .

   >[!NOTE]
   >Rimozione di un profilo da un dispositivo non eliminare il profilo dall'elenco. Se si desidera eliminare un profilo, segui le istruzioni in [aggiornamento o eliminare un profilo Autopilot](#update-or-delete-an-autopilot-profile).

### <a name="update-or-delete-an-autopilot-profile"></a>Aggiornare o eliminare un profilo Autopilot

Se un cliente desidera modificare l'esperienza out-of-box dopo che hai fornito i dispositivi su di essi, è possibile modificare il profilo nel centro per i Partner.

Quando il dispositivo del cliente si connette a internet, verranno scaricati la versione più recente del profilo durante il processo di configurazione guidata. Inoltre, ogni volta che un cliente Ripristina impostazioni predefinite di fabbrica, un dispositivo il dispositivo verrà nuovamente scaricare la versione più recente del profilo durante il processo di configurazione guidata.

1. Seleziona **clienti** dal menu di Centro per i Partner e quindi seleziona il cliente che desidera modificare un profilo Autopilot.

2. Nella pagina dei dettagli del cliente, seleziona **i dispositivi**.

3. Selezionare il profilo che è necessario aggiornare **i profili di Windows Autopilot** . Apporta le modifiche necessarie e quindi seleziona **Invia**.

Per eliminare il profilo, seleziona **eliminare il profilo** nell'angolo superiore destro della pagina.

### <a name="add-devices-to-a-customers-account"></a>Aggiungere i dispositivi all'account del cliente

>[!NOTE]
>Gli agenti di vendita e agenti amministratore possono aggiungere i dispositivi per conto del cliente.

Prima di poter applicare i profili Autopilot personalizzati per i dispositivi dei clienti, è necessario essere in grado di accedere all'elenco di dispositivo del cliente.

Se si prevede di usare il nome OEM, il numero di serie e combinazione di modello, tieni presente queste limitazioni:

- Questa versione tupla funziona solo per i dispositivi più recente (4 k hash, ad esempio) e non è supportato per 128b hash (RS2 e dispositivi precedenti).

- La registrazione tupla è tra maiuscole e minuscole, in modo che i dati nel file devono corrispondere il modello e produttore nomi ***esattamente*** come specificato dal provider di OEM (provider hardware).

Segui le istruzioni seguenti per aggiungere i dispositivi per conto del cliente nel centro per i Partner.

1. Seleziona **clienti** dal menu di Centro per i Partner e quindi seleziona il cliente di cui desideri gestire i dispositivi.

2. Nella pagina dei dettagli del cliente, seleziona **i dispositivi**.

3. Selezionare **Aggiungi dispositivi** **Applica profili ai dispositivi** .

4. Immetti un nome per l'elenco dei dispositivi e quindi seleziona **Sfoglia** per caricare l'elenco del cliente (in formato di file con estensione csv) al centro per i Partner.

    >[!NOTE]
    >Dovrebbe aver ricevuto il file CSV con l'acquisto di dispositivo. Se non ricevi un file con estensione csv, è possibile creare una personalizzata seguendo i passaggi descritti in [aggiunta i dispositivi Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).  

5. Caricare il file CSV e quindi seleziona **salvare**.

Se ricevi un messaggio di errore durante il tentativo di caricare il file con estensione csv, controlla il formato del file. È possibile utilizzare, solo l'hash hardware o il nome dell'OEM, il numero di serie e modello (in questo ordine colonna) o l'ID prodotto Windows. È inoltre possibile utilizzare il file CSV di esempio fornito dal collegamento accanto **Aggiungi dispositivi** per creare un elenco dei dispositivi.

## <a name="windows-autopilot-eula-dismissal"></a>Interruzione dell'EULA di Windows Autopilot

### <a name="important-information"></a>INFORMAZIONI IMPORTANTI

Windows Autopilot consente di configurare le installazioni personalizzate di Windows nei dispositivi gestiti per i tuoi clienti. Se disponi dell'autorizzazione per eseguire questa operazione dal cliente, puoi eliminare o nascondere alcune schermate di installazione che normalmente vengono visualizzate agli utenti durante la configurazione di Windows, tra cui lo schermo di accettazione del contratto di licenza (contratto di licenza utente finale).

Utilizzando questa funzione, accetti che eliminando o nascondendo le schermate progettate per fornire agli utenti avviso o l'accettazione delle condizioni indica di avere ricevuto il consenso sufficiente e l'autorizzazione dal cliente per nascondere i termini e che si, per conto di il cliente (se un'organizzazione o singolo utente nel caso potrebbe essere), gli avvisi e accettare le condizioni applicabili al cliente. Ciò include il contratto per le condizioni della licenza o dell'avviso che potrebbero essere presentati all'utente se non è stato scelto di non visualizzare o di nascondere usando questo strumento. Il cliente non può utilizzare il software Windows su tali dispositivi se non ha acquisito validamente una licenza per il software da Microsoft o dai distributori autorizzati.