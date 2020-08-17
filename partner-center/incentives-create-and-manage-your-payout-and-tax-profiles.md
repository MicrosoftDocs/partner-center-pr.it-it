---
title: Creare e gestire il profilo di pagamento e il profilo fiscale nel Centro per i partner
ms.topic: how-to
ms.date: 08/13/2020
description: Prima di poter pagare il lavoro per gli incentivi, è necessario creare i profili di pagamento e di imposta.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: 6bf2f70bac6cbabcc0e4267585a23e1b74916c06
ms.sourcegitcommit: 9d3f88f7008a2771b02cb4af860c6ca00eb50e42
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/17/2020
ms.locfileid: "88303277"
---
# <a name="payout-and-tax-profiles-in-partner-center"></a>Profili di pagamento e fiscali nel Centro per i partner

Si applica a:

- Centro per i partner

Prima di poter ricevere il pagamento per i programmi Incentivi per una particolare posizione MPN, è necessario completare la registrazione associando un profilo di pagamento e fiscale valido al programma e alla posizione MPN. Microsoft userà il profilo di pagamento e fiscale per emettere i pagamenti. È possibile che l'utente sia autorizzato a usare il trasferimento bancario elettronico o una nota di accredito per il pagamento, a seconda delle regole del programma Incentivi. 

Ruoli appropriati:

- Amministratore degli incentivi
- Amministratore fatturazione
- Amministratore globale

## <a name="roles-currencies-and-other-microsoft-programs"></a>Ruoli, valute e altri programmi Microsoft

È importante comprendere le informazioni riportate di seguito prima di iniziare con il profilo di pagamento e di imposta.

### <a name="roles-and-permissions"></a>Ruoli e autorizzazioni

È necessario essere un amministratore di incentivi per immettere le informazioni fiscali e bancarie per i pagamenti di incentivi. Se si è un amministratore MPN/account, è possibile assegnare se stessi e/o un collega come amministratore di incentivi.

Se è necessario richiedere le autorizzazioni di amministratore per gli incentivi, contattare l'amministratore MPN o l'amministratore globale. È possibile scoprire chi ha questi ruoli nell'azienda nel [Dashboard del centro](https://partner.microsoft.com/dashboard/)per i partner. Dall'icona **Impostazioni** in alto a destra selezionare **Gestione utenti** , quindi filtrare in base a amministratore globale.

Gli incentivi consentono agli utenti di visualizzare i guadagni e i dettagli di pagamento e i report, ma non possono modificare i dettagli di banca e fiscali.

### <a name="choose-your-disbursement-currency"></a>Scegliere la valuta per il pagamento

Per impostazione predefinita, i pagamenti per gli incentivi vengono effettuati nella valuta locale di ogni entità corrispondente. È possibile specificare una valuta diversa durante la configurazione del profilo. I pagamenti verranno calcolati usando un tasso di cambio impostato su base mensile da Microsoft. L'utente sarà responsabile di tutte le modifiche apportate al valore a causa della valuta selezionata.

### <a name="bank-and-tax-information-and-other-programs"></a>Informazioni bancarie e fiscali e altri programmi

Fornire le informazioni descritte di seguito anche se Microsoft utilizza già i dati bancari per i pagamenti. Ciò consente di garantire la privacy e la sicurezza dei dati aziendali, perché la copia del profilo nel nuovo strumento potrebbe esporre informazioni riservate. L'esecuzione di questo processo è anche un'opportunità ideale per garantire che i dati siano completi e accurati.

### <a name="using-different-profiles-for-different-microsoft-programs"></a>Uso di profili diversi per programmi Microsoft diversi

All'interno del dettaglio, i pagamenti per ognuno dei cinque programmi per incentivi al dettaglio possono essere inviati allo stesso account bancario. In alternativa, è possibile scegliere di fare in modo che i pagamenti per la vendita al dettaglio vengano inseriti in un conto bancario mentre l'ufficio vendite al dettaglio viene pagato per un conto bancario diverso.

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a>Creare e gestire il profilo di pagamento e il profilo fiscale nel Centro per i partner

Le sezioni seguenti illustrano il processo di creazione e gestione dei profili di pagamento e di imposta nel centro per i partner.

>[!IMPORTANT]
>È necessario essere un amministratore di incentivi per creare o gestire i profili di pagamento nel centro per i partner. I ruoli incentivo devono essere assegnati a ogni località MPN in ogni programma di incentivi. Per altre informazioni su come aggiungere gli amministratori di incentivi in Partner Center, vedere [come aggiungere utenti o amministratori di incentivi nel centro per i partner](https://support.microsoft.com/help/3011450/how-to-add-incentive-users-or-admins-in-partner-center).

## <a name="access-the-payout-and-tax-section-in-partner-center"></a>Accedere alla sezione relativa ai pagamenti e alle imposte nel centro per i partner

1. Accedere al centro per i partner usando l'account Azure Active Directory (Azure AD) (account aziendale) o l'indirizzo di posta elettronica appropriato se ne è stato assegnato uno. 

   - È possibile registrare più domini all'interno di un account Azure AD. Contattare l'amministratore globale per determinare quali domini sono associati.
   - Se si è in grado di accedere solo con il @onmicrosoft.com dominio, contattare l'amministratore dell'account per aggiungere ulteriori domini all'account Azure ad.
   - Se viene richiesto di selezionare un account aziendale o dell' **Istituto di istruzione** o un account **personale**, selezionare account aziendale o dell'Istituto di **istruzione**.

2. Selezionare l'icona a forma di ingranaggio per aprire il menu **Impostazioni** , quindi selezionare **Impostazioni partner**.

3. Nel menu **Impostazioni account** selezionare **pagamenti e imposte**. 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a>Assegnare i profili di pagamento e di imposta a singoli programmi

1. In centro per i partner selezionare l'icona a forma di ingranaggio per aprire il menu **Impostazioni** . 

2. Selezionare **Impostazioni partner**, espandere la **sezione pagamenti e imposte**, quindi selezionare **assegnazione del profilo di pagamento e di imposta**. 
   
   Verrà visualizzato un elenco dei programmi. Selezionare la freccia accanto a un programma per visualizzare i dettagli del profilo. 

3. Nel menu a discesa **profilo fiscale** selezionare il profilo fiscale desiderato oppure selezionare l'opzione per creare un nuovo profilo. Quando si seleziona l'opzione per creare un nuovo profilo, si verrà reindirizzati in modo appropriato.  Selezionare continua nella finestra popup. Il processo per la creazione di un nuovo profilo fiscale è stato fornito di seguito.

4. Selezionare il **metodo di pagamento**.

   - Se è stato selezionato **Electronic Bank Transfer** come metodo di pagamento, selezionare il profilo di pagamento desiderato oppure selezionare l'opzione per creare un nuovo profilo. Quando si seleziona l'opzione per creare un nuovo profilo, si verrà reindirizzati in modo appropriato. Selezionare continua nella finestra popup. Di seguito è riportato il processo per la creazione di un nuovo profilo di pagamento.

   - Se è stata selezionata la **Nota di credito** come metodo di pagamento, completare la verifica. In questo modo viene confermato che il numero SAP a cui si fa riferimento appartiene all'organizzazione.

    >[!NOTE]
    >Se sono elencate più entità aziendali Microsoft, è necessario selezionare un profilo di pagamento per ogni entità.

    >[!NOTE]
    >La disponibilità dei metodi di pagamento dipende dalle regole del programma di incentivi.
    
5. Selezionare la **valuta**.

6. Una volta completati tutti i campi di pagamento, selezionare **Invia**.

## <a name="create-your-bank-profile"></a>Creare il profilo bancario

I profili bancari vengono creati a livello di organizzazione. Questo consente l'assegnazione di un profilo bancario tra più ID MPN e programmi incentive all'interno di un'organizzazione. È possibile che si verifichino eccezioni durante l'applicazione del profilo bancario a paesi diversi, in quanto possono essere applicate diverse regole fiscali e bancarie.

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

Si verrà reindirizzati alla pagina dei **profili di pagamento e fiscali** . Lo stato del nuovo profilo rifletterà la **convalida Microsoft in sospeso** fino a quando non sarà stata completata la convalida. Questo processo può richiedere fino a 48 ore. Al termine della convalida, lo stato del profilo rifletterà l' **approvazione** o l' **azione richiesta**. Se è **richiesta l'azione**, ripetere i passaggi precedenti fornendo le informazioni necessarie. 

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

## <a name="next-steps"></a>Passaggi successivi

- [Domande frequenti su proventi da incentivi e profilo fiscale](incentives-payout-tax-profile-faqs.md)
