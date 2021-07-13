---
title: Profili di pagamento e fiscali nel Centro per i partner
ms.topic: how-to
ms.date: 04/15/2021
description: Creare e gestire il profilo di pagamento e fiscale in modo che sia possibile ottenere i pagamenti per il lavoro degli incentivi. Include la creazione, la gestione e l'uso di profili diversi.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: a6d578c2ad09e1f8bb03f520d659f1a9b1e199a9
ms.sourcegitcommit: a09a5f893e876de23a8aa5c0d637e50c5be84941
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/13/2021
ms.locfileid: "113684254"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a>Creare e gestire profili di pagamento e fiscali per gli incentivi in Partner Center

**Ruoli appropriati:** amministratore degli incentivi | Account admin | Amministratore globale

Prima di poter ricevere il pagamento per i programmi Incentivi per una particolare posizione MPN, è necessario completare la registrazione associando un profilo di pagamento e fiscale valido al programma e alla posizione MPN. Microsoft userà il profilo di pagamento e fiscale per emettere i pagamenti. È possibile che l'utente sia autorizzato a usare il trasferimento bancario elettronico o una nota di accredito per il pagamento, a seconda delle regole del programma Incentivi. 

## <a name="roles-currencies-and-multiple-microsoft-incentive-programs"></a>Ruoli, valute e più programmi di incentivi Microsoft

È importante comprendere le informazioni seguenti prima di iniziare a usare il profilo di pagamento e fiscale.

### <a name="roles-and-permissions"></a>Ruoli e autorizzazioni

Per immettere informazioni bancarie e fiscali per i pagamenti di incentivi, è necessario essere un amministratore degli incentivi. Gli amministratori mpn/account possono assegnare se stessi e/o un collega come amministratore incentivi.

Se è necessario richiedere le autorizzazioni di amministratore incentivi, contattare l'amministratore MPN o l'amministratore globale. È possibile scoprire chi nell'azienda ha questi ruoli accedendo al [dashboard di Partner Center](https://partner.microsoft.com/dashboard/). **Nell'Impostazioni** in alto a destra selezionare **Gestione utenti** e quindi filtrare in base ad Amministratore globale.

Incentivi Gli utenti possono visualizzare i dettagli e i report relativi agli utili e ai pagamenti degli incentivi, ma non possono modificare i dettagli bancari e fiscali.

### <a name="choose-your-disbursement-currency"></a>Scegliere la valuta di pagamento

I pagamenti di incentivi vengono effettuati nella valuta selezionata durante la configurazione del profilo di pagamento. I pagamenti verranno calcolati usando un tasso di cambio impostato mensilmente da Microsoft. L'utente sarà responsabile di eventuali modifiche di valore a causa della valuta selezionata.

### <a name="using-different-profiles-for-different-microsoft-programs"></a>Uso di profili diversi per programmi Microsoft diversi

Se l'azienda è iscritta a più programmi di incentivi, è possibile usare lo stesso account di pagamento per tutti oppure scegliere di usare account di pagamento diversi per programmi diversi.

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a>Creare e gestire il profilo di pagamento e il profilo fiscale nel Centro per i partner

Le sezioni seguenti illustrano il processo di creazione e gestione dei profili di pagamento e fiscali in Partner Center.

>[!IMPORTANT]
>È necessario essere un amministratore incentivi per creare o gestire profili di pagamento e fiscali in Partner Center. I ruoli di incentivi devono essere assegnati a ogni località MPN in ogni programma di incentivi. Per altre informazioni su come aggiungere amministratori di Incentivi in Partner Center, vedere [Creare account utente.](create-user-accounts-and-set-permissions.md)

## <a name="access-the-payout-and-tax-section-in-partner-center"></a>Accedere alla sezione relativa ai pagamenti e alle imposte in Partner Center

1. Accedere al [dashboard di Partner Center](https://partner.microsoft.com/dashboard/) usando l'account Azure Active Directory (Azure AD) (account aziendale) o l'indirizzo di posta elettronica appropriato, se assegnato.

   - È possibile registrare più domini all'interno di Azure AD account. Contattare l'amministratore globale per determinare i domini associati.
   - Se si è in grado di accedere solo con il dominio e sono necessari altri domini, contattare l'amministratore dell'account per aggiungere altri domini @onmicrosoft.com all'account Azure AD dominio.
   - Se viene richiesto di selezionare Account aziendale o dell'istituto di istruzione o **Account** **personale,** selezionare Account **aziendale o dell'istituto di istruzione.**

2. Selezionare l'icona a forma di ingranaggio **per aprire Impostazioni** e quindi selezionare Impostazioni **account.**

3. Nel menu **Impostazioni account** selezionare Pagamenti **e imposte.**

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a>Assegnare profili di pagamento e fiscali a singoli programmi

1. Accedere al [dashboard Partner Center e](https://partner.microsoft.com/dashboard/)quindi selezionare l'icona a forma di ingranaggio per aprire il menu **Impostazioni.** 

2. Selezionare **Account settings (Impostazioni account),** espandere **la sezione Payout and tax**(Pagamenti e imposte) e quindi selezionare Payout and tax profile assignment (Assegnazione profilo di pagamento e **imposta).** 
   
   Verrà visualizzato un elenco dei programmi. Selezionare la freccia accanto a un programma per visualizzare i dettagli del profilo. 

3. Nel menu **a discesa Profilo** fiscale selezionare il profilo fiscale desiderato oppure selezionare l'opzione per creare un nuovo profilo. Quando si seleziona l'opzione per creare un nuovo profilo, si verrà reindirizzati in modo appropriato.  Selezionare **Continua** nella finestra popup. Il processo per la creazione di un nuovo profilo fiscale è illustrato di seguito.

4. Selezionare **Metodo di pagamento.**

   - Se è stato selezionato **Il trasferimento bancario elettronico** come metodo di pagamento, selezionare il profilo di pagamento desiderato oppure selezionare l'opzione per creare un nuovo profilo. Quando si seleziona l'opzione per creare un nuovo profilo, si verrà reindirizzati in modo appropriato. Selezionare Continua nella finestra popup. Il processo per la creazione di un nuovo profilo di pagamento è stato fornito di seguito.

   - Se è stata selezionata **l'opzione Nota di** credito come metodo di pagamento, completare la verifica. Ciò conferma che il numero SAP a cui si fa riferimento appartiene all'organizzazione.

    >[!NOTE]
    >Se sono elencate più entità aziendali Microsoft, è necessario selezionare un profilo di pagamento per ogni entità.

    >[!NOTE]
    >La disponibilità del metodo di pagamento dipende dalle regole del programma di incentivi.

    - Se l'ID MPN della posizione viene pagato da una filiale Microsoft locale per un particolare programma di incentivi e consente la nota di credito LRD (distributore a rischio limitato) come metodo di pagamento, il profilo di pagamento verrà precompilato con il metodo di pagamento LRD Credit Note. Nella riga del metodo di pagamento della nota di credito LRD per il  rispettivo programma di incentivi e l'ID MPN della posizione verrà visualizzato **Confermata** o Verifica necessaria come stato nella sezione del profilo di pagamento.
    
       Selezionare **Verifica necessaria per** confermare e verificare i dettagli dell'ID tenant CSP associati alla posizione MPN e al metodo di pagamento per ricevere il pagamento della nota di credito. Nella finestra **di dialogo Credit Note Details (Dettagli** nota di credito) esaminare e verificare che l'ID tenant CSP e i dettagli specificati siano corretti. Se viene visualizzato più di un ID tenant, selezionare con attenzione l'ID tenant CSP per cui si vogliono ricevere i pagamenti. Selezionare quindi **Conferma per** confermare che i dettagli della società sono corretti e che il pagamento dell'incentivo deve essere effettuato all'ID tenant CSP selezionato.
 
      Se lo stato è **Confermato**, l'assegnazione dell'ID tenant CSP è stata completata e non sono necessarie altre azioni. È comunque possibile selezionare Confermato per visualizzare i dettagli dell'assegnazione.
   
      Nei paesi che richiedono ai partner di richiedere in modo esplicito di applicare un'esenzione fiscale, è possibile applicare l'esenzione fiscale accanto al profilo fiscale nella sezione relativa al profilo fiscale del programma di incentivi e alla posizione MPN. Selezionando questa casella, i vantaggi dell'esenzione fiscale verranno applicati alla nota di credito dell'incentivo. 
   
      Attualmente, il metodo di pagamento della nota di credito LRD è disponibile solo per i partner Australia, Nuova Zelanda e Canada per il programma Microsoft Commerce Incentive. Se sei un partner con fatturazione diretta o un provider indiretto in questi tre paesi registrati al programma MCI e non vedi la nota di credito LRD come metodo di pagamento disponibile, verifica che l'ID tenant sia associato all'account della posizione MPN del partner pertinente. Per altre informazioni, leggere come [aggiornare il profilo dell'organizzazione.](update-your-partner-profile.md)

    
5. Selezionare la **valuta**.

6. Dopo aver completato tutti i campi di pagamento, selezionare **Invia.**

## <a name="set-up-a-default-bank-profile"></a>Configurare un profilo bancario predefinito

È possibile configurare i profili bancari predefiniti e assegnarli alle sedi MPN. Questi profili predefiniti verranno usati da Microsoft per le registrazioni successive per tale posizione MPN. 

1. Accedere al [dashboard Partner Center e](https://partner.microsoft.com/dashboard/)quindi selezionare l'icona a forma di ingranaggio per aprire il menu **Impostazioni.**   

2. Selezionare Account settings (Impostazioni **account),** **espandere la sezione Payout and tax** (Pagamenti e imposte) e quindi selezionare **Payout and tax profiles (Profili di pagamento e fiscali).** 

3. Selezionare **Gestisci profili predefiniti** nella sezione Profili **di** pagamento. 

4. Per creare un profilo bancario predefinito, selezionare **Aggiungi un profilo bancario predefinito.** 

5. Selezionare un profilo bancario dall'elenco dei profili bancari disponibili della società, selezionare la valuta da usare con questo profilo bancario e quindi selezionare l'elenco di sedi MPN a cui si vuole applicare questo profilo predefinito.

6. Dopo **aver completato** le selezioni, selezionare Fine. Il pulsante Fine sarà selezionabile solo dopo il completamento di tutti i campi obbligatori. 

>[!NOTE]
>La stessa associazione bancaria e valuta può essere applicata a più posizioni. Se alla località MPN è stata assegnata una sola volta una combinazione di profilo e valuta predefinita, non verrà più visualizzata nell'elenco a discesa delle località per le future assegnazioni di profilo predefinite. Se la selezione predefinita viene eliminata, il mpn della posizione verrà nuovamente visualizzato per le future assegnazioni di profilo predefinite. Ogni combinazione di profilo bancario e valuta viene aggiunta come riga univoca e modificabile.

7. Dopo aver aggiunto tutte le modifiche necessarie, selezionare **Salva**.  

## <a name="create-your-bank-profile"></a>Creare il profilo bancario

I profili bancari vengono creati a livello aziendale. In questo modo è possibile assegnare un profilo bancario tra più programmi di incentivi e ID MPN all'interno di un'azienda. Potrebbero esserci eccezioni quando si applica il profilo bancario a paesi diversi, in quanto possono essere applicate regole bancarie e fiscali diverse.

>[!NOTE]
>Nelle pagine seguenti sono necessari campi con un asterisco. Se non si conosce un campo, selezionare l'icona delle informazioni. 

1. Nella pagina **Dettagli** completare i campi seguenti: **Nome profilo:** immettere un nome univoco per identificare il profilo di pagamento.
    **Posizione del conto bancario:** Paese in cui si trova la banca della società.
    **Metodo di pagamento:** Il metodo di pagamento preferito per Partner Center è il trasferimento bancario elettronico.

2. Selezionare **Avanti**.

3. Nella pagina **Conto bancario** immettere le informazioni. I campi visualizzati in questa pagina variano in base al paese. 

4. Selezionare **Avanti**.

5. Nella pagina **Beneficiary** immettere le informazioni appropriate. Il beneficiario è la persona dell'azienda che la banca deve contattare se deve discutere del proprio account.

6. Dopo aver completato i campi, selezionare **Fine** e quindi selezionare **Conferma per** creare il profilo bancario.

Si verrà reindirizzati alla pagina **Profili di pagamento e** fiscali. Lo stato del nuovo profilo riflette la convalida **Microsoft in** sospeso fino al completamento della convalida. Questo processo può richiedere fino a 48 ore. Al termine della convalida, lo stato del profilo rifletterà **Approvato** o **Azione richiesta.** Se **l'azione è** obbligatoria, ripetere i passaggi precedenti fornendo le informazioni necessarie. 

## <a name="create-your-tax-profile"></a>Creare il profilo fiscale

Usare la procedura seguente per fornire a Microsoft le informazioni fiscali necessarie per l'organizzazione. Le pagine di questa sezione sono dinamiche e variano a seconda del paese o dell'area geografica. Per informazioni sull'identificazione delle informazioni fiscali corrette, contattare le origini governative appropriate nel proprio paese.

Per le aziende partner nelle Americhe, se sono necessarie informazioni sul completamento dei moduli W8 o W9, gli indirizzi seguenti ti consereranno al sito IRS:

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> Immettere solo i dettagli per l'azienda. Non immettere mai i dettagli personali.

1. Nella pagina **Profilo aziendale** completare i campi obbligatori e quindi selezionare **Avanti.** 

2. Nella pagina **Configurazione** selezionare l'opzione applicabile all'azienda.

   - Selezionare l'opzione a sinistra se l'azienda è incorporata nel Stati Uniti o se questo profilo è per un singolo utente.
   - Selezionare l'opzione a destra se l'azienda è incorporata all'esterno del Stati Uniti e quindi selezionare il paese o l'area geografica dall'elenco.

3. Selezionare **Avanti**. 

4. Nella pagina **Stato imposta** immettere le informazioni necessarie e quindi selezionare **Avanti.** I campi in questa pagina variano in base al paese. i dettagli. 

5. Nella pagina **Documentazione aggiuntiva** i campi obbligatori e selezionare **Avanti.** 

6. Selezionare **Sfoglia** per caricare tutti i documenti richiesti dal paese o dall'area geografica. Quando viene visualizzato il nome del documento, selezionare **Upload**. 

7. Se è necessario rimuovere il documento, selezionare **Rimuovi**.

8. Per salvare e continuare, selezionare **Fine.**

9. Selezionare **Conferma** nel messaggio popup. Verrà visualizzata di nuovo la pagina **Di configurazione dei pagamenti e delle** imposte.
 
## <a name="update-expired-tax-profiles"></a>Aggiornare i profili fiscali scaduti

1. Accedere al [dashboard Partner Center](https://partner.microsoft.com/dashboard/)e quindi selezionare l'icona a forma di ingranaggio per aprire Impostazioni menu. 

1. Selezionare **Impostazioni account,** espandere la **sezione Pagamento** e imposta e quindi selezionare Pagamento e profilo **fiscale**.

1. Selezionare **Profilo fiscale**.

1. Controllare la colonna **Expiration Date (Data** di scadenza) e passare al profilo fiscale scaduto o in scadenza.

1. Selezionare **Modifica**.

1. Nella sezione modulo fiscale aggiornare i moduli fiscali specificando i nuovi dettagli. 

## <a name="next-steps"></a>Passaggi successivi

- [Domande comuni su pagamenti e imposte](payout-faq.yml)
