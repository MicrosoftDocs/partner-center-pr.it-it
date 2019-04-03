---
title: Personalizzare l'esperienza out-of-box del dispositivo con i profili di Autopilot di Windows | Centro per i partner
description: Preconfigurare esperienza out-of-box del dispositivo con i profili di Autopilot.
ms.topic: article
ms.date: 03/18/19
author: maggiepuccievans
ms.author: evansma
keywords: AutoPilot, autopilot di windows, autopilot microsoft, distribuzione zero touch, la configurazione guidata, le schermate di accesso, out-of-box
ms.localizationpriority: medium
ms.openlocfilehash: e940a7ccf79f6b43d3712a2f3ae2f9b150e1473e
ms.sourcegitcommit: f5dbd07185059aa5faddf1c5daa556f634ce97ee
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/19/2019
ms.locfileid: "58162221"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a>Personalizzare l'esperienza out-of-box del dispositivo con i profili Windows Autopilot

**Si applica a**

- I partner CSP diretti fattura e i provider indiretti i rivenditori indiretti

Se si gestiscono i dispositivi dei clienti, si potrebbe essere necessario personalizzare l'esperienza di out-of-box (OOBE) per gli utenti del cliente. È possibile preconfigurare nuovi dispositivi con profili di Autopilot di Windows prima di recapitare i dispositivi per i clienti e si applicano nuovi profili nei dispositivi, i clienti hanno già acquistato. Questo articolo illustra come creare e applicare i profili di Autopilot per i dispositivi nel centro per i Partner.

Se non si ha già familiarità con Autopilot, consultare le informazioni contenute in questi articoli:

- [Panoramica di Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [Guida di riferimento di distribuzione AutoPilot](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>Panoramica

Con la funzionalità di Windows Autopilot nel centro per i Partner, è possibile creare profili personalizzati da applicare ai dispositivi dei clienti. Le impostazioni del profilo sono state disponibili al momento che della pubblicazione dell'articolo:

- Ignorare le impostazioni di privacy. Questa impostazione del profilo di Autopilot facoltativa consente alle organizzazioni di non porre sulle impostazioni di privacy durante il processo di configurazione guidata.

- Disabilitare la creazione dell'account amministratore locale nel dispositivo. Le organizzazioni possono decidere se l'utente di configurazione del dispositivo deve avere accesso come amministratore, una volta completato il processo.

- Configurare automaticamente i dispositivi per lavoro o dell'istituto di istruzione. Tutti i dispositivi registrati con Autopilot verranno automaticamente considerati lavoro o dell'istituto di istruzione, i dispositivi in modo che durante il processo di configurazione guidata non verrà chiesto di questa domanda.

- Ignorare Cortana, OneDrive e OEM pagine di configurazione di registrazione. Tutti i dispositivi registrati con Autopilot ignorerà automaticamente queste pagine durante il processo di out-of-box configurazione guidata.

- Ignorare il contratto di licenza utente finale (EULA). A partire da Windows 10 versione 1709, le organizzazioni possono decidere di ignorare la pagina Contratto di licenza presentata durante il processo di configurazione guidata. Visualizzare [licenziamento condizioni di licenza di Windows Autopilot](#windows-autopilot-eula-dismissal) seguito per informazioni importanti da considerare su come ignorare la pagina Contratto di licenza Windows durante l'installazione.

Si applicano le autorizzazioni di gestione profilo e dispositivo e le limitazioni seguenti:

- I partner CSP possono continuare a gestire i profili di Autopilot per i clienti esistenti con cui hanno relazioni reseller, anche se i clienti hanno rimosso i privilegi di amministrazione delegata del partner.

- È possibile gestire i dispositivi esistenti per i clienti che sono stati aggiunti.

- Non è possibile gestire i dispositivi che del cliente è caricata in Microsoft Store per le aziende o il portale di Microsoft Intune.

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>Creare e gestire i profili di Autopilot nel centro per i Partner

Nel centro per i Partner, è possibile creare profili di distribuzione Windows Autopilot e applicarle ai dispositivi.

>[!NOTE]
>Solo gli agenti di amministrazione è possono creare e applicare i profili.

### <a name="create-a-new-autopilot-profile"></a>Creare un nuovo profilo di Autopilot

1. Selezionare **clienti** dal centro per i Partner menu e quindi selezionare il cliente crei il profilo di Autopilot per.

2. Nella pagina dei dettagli del cliente, selezionare **dispositivi**.

3. Sotto **profili Windows Autopilot** selezionate **aggiungere nuovo profilo**.

4. Immettere nome e una descrizione del profilo e quindi configurare le impostazioni di configurazione guidata. Scegliere tra:  

   - Ignorare le impostazioni di privacy nel programma di installazione

   - Disabilitare l'account amministratore locale durante la configurazione
  
   - Ignorare automaticamente le pagine durante la configurazione<br>
        (Include *automaticamente seleziona il programma di installazione per l'azienda o dell'istituto di istruzione* e *pagine di configurazione di registrazione OEM, OneDrive e Skip Cortana*)
  
   - Ignorare il contratto di licenza utente finale (EULA)<br> 
       >[!IMPORTANT] 
       >Visualizzare [licenziamento condizioni di licenza di Windows Autopilot](#windows-autopilot-eula-dismissal) seguito per informazioni importanti da considerare su come ignorare la pagina Contratto di licenza Windows durante l'installazione.

5. Al termine seleziona **Invia**.

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>Applicare un profilo di Autopilot per i dispositivi dei clienti

>[!NOTE]
>Le istruzioni seguenti presuppongono che i dispositivi del cliente è già stato aggiunto al centro per i Partner e che sia possibile accedere proprio elenco di dispositivi. Se è già stato aggiunto i dispositivi del cliente, seguire le istruzioni in [aggiungere i dispositivi a un account del cliente](#add-devices-to-a-customers-account) e quindi seguire la procedura seguente.

Dopo aver creato un profilo di Autopilot per un cliente, è possibile applicarlo ai dispositivi del cliente.

1. Selezionare **clienti** dal centro per i Partner menu e quindi selezionare il cliente creato per il profilo di Autopilot.

2. Nella pagina dei dettagli del cliente, selezionare **dispositivi**.

3. Sotto **applicare i profili nei dispositivi** selezionare i dispositivi o gruppi di dispositivi che si desidera aggiungere i profili e quindi selezionare **applicare profilo**. Il profilo appena applicati viene visualizzato nei **profilo** colonna.

4. Attenersi alla procedura seguente per verificare che il profilo verrà applicato correttamente al dispositivo.

    a.  Connettere un dispositivo alla rete e attivarlo.

    b.  Verifica che siano visualizzate le eventuali schermate appropriate della Configurazione guidata.

    c.  Quando si arresta il processo di configurazione guidata, reimpostare il dispositivo per le impostazioni predefinite per prepararlo per un nuovo utente.

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>Rimuovere un profilo di Autopilot da dispositivo del cliente

1. Selezionare **clienti** dal centro per i Partner menu e quindi selezionare il cliente creato per il profilo di Autopilot.

2. Nella pagina dei dettagli del cliente, selezionare **dispositivi**.

3. Sotto **applicare i profili nei dispositivi** selezionare i dispositivi che si desidera rimuovere il profilo e quindi selezionare **rimuovere il profilo**.

   >[!NOTE]
   >Rimozione di un profilo da un dispositivo non elimina il profilo dall'elenco. Se si desidera eliminare un profilo, seguire le istruzioni in [Update o delete un profilo di Autopilot](#update-or-delete-an-autopilot-profile).

### <a name="update-or-delete-an-autopilot-profile"></a>Aggiornare o eliminare un profilo di Autopilot

Se un cliente vuole modificare l'esperienza di out-of-box dopo che è stato spedito i loro dispositivi, è possibile modificare il profilo nel centro per i Partner.

Quando il dispositivo del cliente si connette a internet, verrà scaricato la versione più recente del profilo durante il processo di configurazione guidata. Inoltre, ogni volta che un cliente consente di ripristinare un dispositivo per le impostazioni predefinite, il dispositivo nuovamente scaricherà l'ultima versione del profilo durante il processo di configurazione guidata.

1. Selezionare **clienti** dal centro per i Partner menu e quindi selezionare il cliente che si desidera modificare un profilo di Autopilot.

2. Nella pagina dei dettagli del cliente, selezionare **dispositivi**.

3. Sotto **profili Windows Autopilot** selezionare il profilo è necessario aggiornare. Apportare le modifiche necessarie e quindi selezionare **Submit**.

Per eliminare questo profilo, selezionare **eliminare il profilo** dall'angolo superiore destro della pagina.

### <a name="add-devices-to-a-customers-account"></a>Aggiungere i dispositivi a un account del cliente

>[!NOTE]
>Gli agenti di vendita e amministratore possono aggiungere dispositivi all'account del cliente.

Prima di poter applicare i profili di Autopilot personalizzati per i dispositivi dei clienti, è necessario essere in grado di accedere all'elenco dispositivi del cliente.

Se si prevede di usare il nome OEM, numero di serie e combinazione di modello, tenere presente queste limitazioni:

- Questa tupla funziona solo per i dispositivi più recenti (4 k gli hash, ad esempio) e non è supportata per gli hash 128b (RS2 e dispositivi precedenti).

- La registrazione di tupla viene fatta distinzione tra maiuscole e minuscole, in modo che i dati nel file devono corrispondere ai nomi di produttore e modello ***esattamente*** fornito dal provider OEM (provider hardware).

Seguire le istruzioni seguenti per aggiungere i dispositivi per conto del cliente nel centro per i Partner.

1. Selezionare **clienti** dal centro per i Partner menu e quindi selezionare il cliente con i dispositivi da gestire.

2. Nella pagina dei dettagli del cliente, selezionare **dispositivi**.

3. Sotto **applicare i profili nei dispositivi** selezionate **aggiungere dispositivi**.

4. Immettere un nome per l'elenco dei dispositivi e quindi selezionare **esplorare** per caricare l'elenco del cliente (nel formato di file con estensione csv) in Partner Center.

    >[!NOTE]
    >Dovrebbe avere inviato questo file con estensione csv con l'acquisto di dispositivo. Se non è stato ricevuto un file con estensione csv, è possibile creare uno manualmente seguendo la procedura descritta in [aggiunta di dispositivi a Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).  

5. Caricare il file con estensione csv e quindi selezionare **salvare**.

Se viene visualizzato un messaggio di errore durante il tentativo di caricare il file con estensione csv, controllare il formato del file. È possibile usare solo l'hash hardware o il nome OEM, il numero di serie e modello (in tale ordine delle colonne) o l'ID prodotto Windows. È anche possibile usare il file CSV di esempio fornito dal collegamento accanto a **aggiungere i dispositivi** per creare un elenco dei dispositivi.

## <a name="windows-autopilot-eula-dismissal"></a>Licenziamento condizioni di licenza di Windows Autopilot

### <a name="important-information"></a>INFORMAZIONI IMPORTANTI

Windows Autopilot consente di configurare installazioni personalizzate di Windows nei dispositivi gestiti per i clienti. Se autorizzato a eseguire questa operazione dal cliente, è possibile eliminare o nascondere alcune schermate di configurazione che normalmente vengono presentate all'utente durante la configurazione di Windows, tra cui la schermata di accettazione di condizioni di licenza (End User License Agreement).

Tramite questa funzione, si accetta che l'eliminazione o nascondere tutte le schermate che sono progettate per offrire agli utenti con avviso o l'accettazione di mezzi di termini di avere ottenuto il consenso sufficiente e l'autorizzazione dal cliente per nascondere i termini e, per conto di il cliente (se un'organizzazione o un singolo utente come nel caso può essere), fornire il consenso a eventuali comunicazioni e accettare le condizioni applicabili al cliente. Ciò include il contratto per le condizioni della licenza o dell'avviso che potrebbero essere presentati all'utente se non è stato scelto di non visualizzare o di nascondere usando questo strumento. Il cliente non può utilizzare il software Windows su tali dispositivi se non ha acquisito validamente una licenza per il software da Microsoft o dai distributori autorizzati.