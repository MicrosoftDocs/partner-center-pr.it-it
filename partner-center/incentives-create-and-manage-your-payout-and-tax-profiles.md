---
title: Creare e gestire i profili di pagamento e fiscali nel centro per i partner
ms.topic: article
ms.date: 06/29/2020
description: Prima di poter pagare il lavoro per gli incentivi, è necessario creare i profili di pagamento e di imposta.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: b7f99ff64b6cdabe8b59607e5820daf0909050f1
ms.sourcegitcommit: bea864212edc90c5f851566505deef6623f79723
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/01/2020
ms.locfileid: "85719399"
---
# <a name="payout-and-tax-profiles-in-partner-center"></a>Profili di pagamento e fiscali nel centro per i partner

Si applica a:

- Centro per i partner

Prima di poter ricevere il pagamento per i programmi Incentivi per una particolare posizione MPN, è necessario completare la registrazione associando un profilo di pagamento e fiscale valido al programma e alla posizione MPN. Microsoft userà il profilo di pagamento e fiscale per emettere i pagamenti. È possibile che l'utente sia autorizzato a usare il trasferimento bancario elettronico o una nota di accredito per il pagamento, a seconda delle regole del programma Incentivi. 

Ruoli appropriati:

- Amministratore degli incentivi
- Amministratore fatturazione
- Amministratore globale

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a>Creare e gestire i profili di pagamento e fiscali nel centro per i partner

Le sezioni seguenti illustrano il processo di creazione e gestione dei profili di pagamento e di imposta nel centro per i partner.

>[!IMPORTANT]
>È necessario essere un amministratore di incentivi per creare o gestire i profili di pagamento nel centro per i partner. I ruoli incentivo devono essere assegnati a ogni località MPN in ogni programma di incentivi. Per altre informazioni su come aggiungere gli amministratori di incentivi in Partner Center, vedere [come aggiungere utenti o amministratori di incentivi nel centro per i partner](https://support.microsoft.com/help/3011450/how-to-add-incentive-users-or-admins-in-partner-center).

## <a name="access-the-payout-and-tax-section-in-partner-center"></a>Accedere alla sezione relativa ai pagamenti e alle imposte nel centro per i partner

1. Accedere al centro per i partner usando il proprio account AAD (account aziendale) o l'indirizzo di posta elettronica appropriato se ne è stato assegnato uno. 

   - È possibile registrare più domini all'interno di un account di AAD. Contattare l'amministratore globale per determinare quali domini sono associati.
   - Se è possibile eseguire l'accesso solo con **@onmicrosoft.com** il dominio, contattare l'amministratore dell'account per aggiungere altri domini all'account AAD.
   - Se viene richiesto di selezionare un account aziendale o dell' **Istituto di istruzione** o un account **personale**, selezionare account aziendale o dell'Istituto di **istruzione**.

2. Selezionare l'icona a forma di ingranaggio per aprire il menu **Impostazioni** , quindi selezionare **Impostazioni partner**.

3. Nel menu **Impostazioni account** selezionare **pagamenti e imposte**. 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a>Assegnare i profili di pagamento e di imposta a singoli programmi

1. In centro per i partner selezionare l'icona a forma di ingranaggio per aprire il menu **Impostazioni** . 

2. Selezionare **Impostazioni partner**, espandere la **sezione pagamenti e imposte**, quindi selezionare **assegnazione del profilo di pagamento e di imposta**. 
   
   Verrà visualizzato un elenco dei programmi. Selezionare la freccia accanto a un programma per visualizzare i dettagli del profilo. 

3. Nel menu a discesa **profilo fiscale** selezionare il profilo fiscale desiderato oppure selezionare l'opzione per creare un nuovo profilo. Quando si seleziona l'opzione per creare un nuovo profilo, si verrà reindirizzati in modo appropriato.  Selezionare continua nella finestra popup. Il processo per la creazione di un nuovo profilo fiscale è stato fornito di seguito.

4. Selezionare il **metodo di pagamento**.

   - Se si è scelto **Electronic Bank Transfer** come metodo di pagamento, selezionare il profilo di pagamento desiderato nell'elenco a discesa Profilo di pagamento oppure selezionare l'opzione per la creazione di un nuovo profilo. Quando si seleziona l'opzione per creare un nuovo profilo, si verrà reindirizzati in modo appropriato.  Selezionare continua nella finestra popup. Di seguito è riportato il processo per la creazione di un nuovo profilo di pagamento.

   - Se è stata selezionata l'opzione **Nota credito** come metodo di pagamento, completare la verifica per verificare che il numero SAP a cui si fa riferimento appartenga all'organizzazione.

    >[!NOTE]
    >Se sono elencate più entità aziendali Microsoft, è necessario selezionare un profilo di pagamento per ogni entità.

    >[!NOTE]
    >La disponibilità dei metodi di pagamento dipende dalle regole del programma di incentivi.
    
5. Selezionare la **valuta**.

6. Una volta completati tutti i campi di pagamento, selezionare **Invia**.

## <a name="create-your-bank-profile"></a>Creare il profilo bancario

I profili bancari vengono creati a livello di organizzazione, che consente di assegnare lo stesso profilo bancario tra più ID MPN e programmi incentive all'interno di un'organizzazione. È possibile che si verifichino eccezioni durante l'applicazione del profilo bancario a paesi diversi, in quanto possono essere applicate diverse regole fiscali e bancarie.

>[!NOTE]
>Nelle pagine seguenti sono necessari campi con un asterisco. Se non si conosce il campo, selezionare l'icona informazioni. 

1. Nella pagina **Dettagli** completare i campi seguenti: **nome profilo:** immettere un nome univoco per identificare il profilo di pagamento.
    **Posizione conto bancario:** Il paese in cui si trova la banca della società.
    **Metodo di pagamento:** Il metodo di pagamento preferito per il centro per i partner è il trasferimento bancario elettronico.

2. Selezionare **Avanti**.

3. Nella pagina **conto bancario** immettere le informazioni. I campi visualizzati in questa pagina variano in base al paese. 

4. Selezionare **Avanti**.

5. Nella pagina **beneficiari** immettere le informazioni appropriate. Il beneficiario è la persona dell'azienda a cui la banca potrebbe rivolgersi se deve discutere l'account.

6. Una volta completati i campi, selezionare **fine**, quindi selezionare **conferma** per creare il profilo bancario.

Si verrà reindirizzati alla pagina dei **profili di pagamento e fiscali** . Lo stato del nuovo profilo rifletterà la **convalida Microsoft in sospeso** fino a quando non sarà stata completata la convalida. Questa operazione può richiedere fino a 48 ore. Al termine della convalida, lo stato del profilo rifletterà l' **approvazione** o l' **azione richiesta**. Se è **richiesta l'azione**, ripetere i passaggi precedenti fornendo le informazioni necessarie. 

## <a name="create-your-tax-profile"></a>Creare il profilo fiscale

Utilizzare la seguente procedura per fornire a Microsoft le informazioni fiscali necessarie per l'organizzazione. Le pagine di questa sezione sono dinamiche e variano in base al paese o all'area geografica. Se è necessario assistenza per identificare le informazioni fiscali corrette, contattare le fonti governative appropriate nel proprio paese.

Per le società partner in America, se sono necessarie informazioni sul completamento dei moduli W8 o W9, i seguenti indirizzi indirizzano al sito di IRS:

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> Immettere solo i dettagli della società. Non immettere mai i dettagli personali.

1. Nella pagina **profilo business** completare i campi obbligatori e quindi fare clic su **Avanti**. 

2. Nella pagina di **installazione** selezionare l'opzione che si applica alla società.

   - Selezionare l'opzione a sinistra se la società è incorporata solo nel Stati Uniti o se il profilo è per un singolo utente. 
   - Selezionare l'opzione a destra se la società è incorporata all'esterno del Stati Uniti, quindi selezionare il paese dall'elenco.

3. Selezionare **Avanti**. 

4. Nella pagina **Tax status** immettere le informazioni necessarie e quindi fare clic su **Next (avanti**). I campi in questa pagina variano in base al paese. dettagli. 

5. Nella pagina **documentazione aggiuntiva** , i campi obbligatori e selezionare **Avanti**. 

6. Selezionare **Browse (Sfoglia** ) per caricare i documenti richiesti dal paese o dall'area geografica. Quando viene visualizzato il nome del documento, selezionare **carica**. 

7. Se è necessario rimuovere il documento, selezionare **Rimuovi**.

8. Per salvare e continuare, selezionare **fine**.

9. Selezionare **conferma** nel messaggio popup. Verrà ripristinata la pagina di **configurazione dei pagamenti e delle imposte** .

## <a name="payout-and-tax-profile-faqs"></a>Domande frequenti sul profilo fiscale e sui pagamenti

### <a name="why-do-i-need-to-provide-my-payout-andor-tax-details"></a>Perché è necessario fornire il pagamento e/o le informazioni fiscali?

Per ricevere i pagamenti per i programmi per gli incentivi Microsoft, è necessario completare la registrazione fornendo i dettagli validi per i pagamenti e le imposte. Una registrazione viene considerata completa solo quando i pagamenti e i profili fiscali forniti vengono convalidati da Microsoft.

### <a name="how-do-i-know-that-i-need-to-provideupdate-my-payout-andor-tax-details"></a>Ricerca per categorie sa che è necessario fornire/aggiornare i dettagli relativi a pagamenti e/o imposte?

Per completare la registrazione, tutti i partner che eseguono la registrazione in un nuovo programma incentive devono fornire i dettagli validi per i pagamenti e le imposte.

Potrebbe anche essere necessario fornire informazioni aggiornate se le regole per il programma incentive cambiano o se gli aspetti del profilo scadono o diventano obsoleti. In tal caso, nella pagina di panoramica verrà visualizzato lo stato **azione richiesta: Aggiorna banca e/o profilo fiscale**.

### <a name="how-do-i-provide-update-my-payout-and-or-tax-details"></a>In che modo inserisco o aggiorno i dettagli di pagamento e/o fiscali?

Per informazioni dettagliate su come aggiornare i dettagli relativi ai pagamenti e alle imposte nel centro per i partner, vedere [How to create and Manage Bank and Tax Profiles in Partner Center](https://support.microsoft.com/help/4524534/how-to-create-and-manage-bank-and-tax-profiles-in-partner-center)

### <a name="why-dont-i-see-my-enrollments-when-i-go-to-assign-my-payout-and-tax-profile"></a>Perché non vedo le registrazioni quando assegno i profili di pagamento e fiscali?

Solo gli amministratori di Incentivi per la posizione MPN possono creare o gestire i profili di pagamento e fiscali. È possibile che l'utente non disponga delle autorizzazioni appropriate o che sia connesso con un account che non dispone di tali autorizzazioni. Contattare l'amministratore dell'organizzazione per gestire le autorizzazioni bancarie e fiscali.

### <a name="where-can-i-see-the-payout-and-tax-profiles-for-my-organization-that-i-can-use"></a>Dove posso vedere i profili di pagamento e fiscali da usare per l'organizzazione?

Usare la procedura seguente per visualizzare i profili di pagamento e fiscali:

1. Accedere al Centro per i partner.

2. Selezionare l'icona a forma di ingranaggi per aprire il menu **Impostazioni**.

3. Selezionare **Impostazioni partner**.

4. In **Impostazioni account** selezionare **Proventi e imposte**, quindi selezionare **Profilo di pagamento e fiscale**. Verranno visualizzati tutti i profili di pagamento e fiscali esistenti, oltre allo stato e alla possibilità di modifica.

### <a name="my-organization-is-participating-in-multiple-incentive-programs-do-i-need-to-provide-my-payment-and-tax-profile-multiple-times"></a>L'organizzazione partecipa a più programmi incentive. È necessario specificare più volte il mio profilo di pagamento e di imposta?

Per i profili di pagamento dipende, in genere, dall'utente. I profili di pagamento vengono creati a livello di organizzazione e questo consente di assegnare lo stesso profilo bancario a più ID MPN e programmi Incentivi all'interno di un'organizzazione. Nella maggior parte dei casi, è possibile riutilizzare un profilo esistente o crearne uno nuovo.

Tuttavia, quando si applica il profilo bancario a paesi o aree geografiche diverse, è possibile che ci siano delle eccezioni.

I profili fiscali creati per una posizione MPN vengono riutilizzati e popolati automaticamente quando la stessa posizione MPN partecipa a un altro programma Incentivi. Ma possono esserci delle eccezioni. Ad esempio, per le regole di pagamento di un nuovo programma Incentivi potrebbero essere necessari altri dettagli per il profilo fiscale.  

### <a name="i-am-only-able-to-log-in-with-my-onmicrosoftcom-domain-what-should-i-do"></a>Sono in grado di accedere solo con il mio @onmicrosoft.com dominio. Cosa devo fare?

Contattare l'amministratore account per aggiungere altri domini all'account AAD.
