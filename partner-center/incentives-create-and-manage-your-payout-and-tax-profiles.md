---
title: Profili di pagamento e fiscali nel Centro per i partner
ms.topic: how-to
ms.date: 09/11/2020
description: Crea e Gestisci il tuo profilo di pagamento e di imposte, in modo da potervi pagare per il lavoro di incentivi.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: de143ecfae1b803e0743a28db5cda5ae9a3d5f2d
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/22/2020
ms.locfileid: "90999315"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="b12c5-103">Creazione e gestione di incentivi per il pagamento e i profili fiscali nel centro per i partner</span><span class="sxs-lookup"><span data-stu-id="b12c5-103">Create and manage incentives payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="b12c5-104">**Si applica a:**</span><span class="sxs-lookup"><span data-stu-id="b12c5-104">**Applies to:**</span></span>

- <span data-ttu-id="b12c5-105">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="b12c5-105">Partner Center</span></span>

<span data-ttu-id="b12c5-106">**Ruoli appropriati:**</span><span class="sxs-lookup"><span data-stu-id="b12c5-106">**Appropriate roles:**</span></span>

- <span data-ttu-id="b12c5-107">Amministratore degli incentivi</span><span class="sxs-lookup"><span data-stu-id="b12c5-107">Incentives admin</span></span>
- <span data-ttu-id="b12c5-108">Amministratore fatturazione</span><span class="sxs-lookup"><span data-stu-id="b12c5-108">Billing admin</span></span>
- <span data-ttu-id="b12c5-109">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="b12c5-109">Global admin</span></span>

<span data-ttu-id="b12c5-110">Prima di poter ricevere il pagamento per i programmi Incentivi per una particolare posizione MPN, è necessario completare la registrazione associando un profilo di pagamento e fiscale valido al programma e alla posizione MPN.</span><span class="sxs-lookup"><span data-stu-id="b12c5-110">Before you can receive payment for your incentive programs for a particular MPN location, you must complete your enrollment by associating a valid payout and tax profile with the program and MPN location.</span></span> <span data-ttu-id="b12c5-111">Microsoft userà il profilo di pagamento e fiscale per emettere i pagamenti.</span><span class="sxs-lookup"><span data-stu-id="b12c5-111">Microsoft will use this payout and tax profile to issue payments.</span></span> <span data-ttu-id="b12c5-112">È possibile che l'utente sia autorizzato a usare il trasferimento bancario elettronico o una nota di accredito per il pagamento, a seconda delle regole del programma Incentivi.</span><span class="sxs-lookup"><span data-stu-id="b12c5-112">You may be allowed to use electronic bank transfer or a credit note for payment, depending on the rules of the incentive program.</span></span> 

## <a name="roles-currencies-and-other-microsoft-programs"></a><span data-ttu-id="b12c5-113">Ruoli, valute e altri programmi Microsoft</span><span class="sxs-lookup"><span data-stu-id="b12c5-113">Roles, currencies, and other Microsoft programs</span></span>

<span data-ttu-id="b12c5-114">È importante comprendere le informazioni riportate di seguito prima di iniziare con il profilo di pagamento e di imposta.</span><span class="sxs-lookup"><span data-stu-id="b12c5-114">It's important to understand the information below before you get started with your payout and tax profile.</span></span>

### <a name="roles-and-permissions"></a><span data-ttu-id="b12c5-115">Ruoli e autorizzazioni</span><span class="sxs-lookup"><span data-stu-id="b12c5-115">Roles and permissions</span></span>

<span data-ttu-id="b12c5-116">È necessario essere un amministratore di incentivi per immettere le informazioni fiscali e bancarie per i pagamenti di incentivi.</span><span class="sxs-lookup"><span data-stu-id="b12c5-116">You must be an Incentives Admin to enter bank and tax information for incentive payments.</span></span> <span data-ttu-id="b12c5-117">Se si è un amministratore MPN/account, è possibile assegnare se stessi e/o un collega come amministratore di incentivi.</span><span class="sxs-lookup"><span data-stu-id="b12c5-117">If you're an MPN/Account Admin, you can assign yourself and/or a colleague to be the Incentives Admin.</span></span>

<span data-ttu-id="b12c5-118">Se è necessario richiedere le autorizzazioni di amministratore per gli incentivi, contattare l'amministratore MPN o l'amministratore globale. È possibile scoprire chi ha questi ruoli nell'azienda accedendo al [Dashboard del centro](https://partner.microsoft.com/dashboard/)per i partner.</span><span class="sxs-lookup"><span data-stu-id="b12c5-118">If you need to request Incentives Admin permissions, contact your MPN Admin or Global Admin. You can find out who in your company has these roles by signing into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span> <span data-ttu-id="b12c5-119">Dall'icona **Impostazioni** in alto a destra selezionare **Gestione utenti** , quindi filtrare in base a amministratore globale.</span><span class="sxs-lookup"><span data-stu-id="b12c5-119">From the **Settings** icon at the top right, select **User Management** and then filter on Global Admin.</span></span>

<span data-ttu-id="b12c5-120">Gli incentivi consentono agli utenti di visualizzare i guadagni e i dettagli di pagamento e i report, ma non possono modificare i dettagli di banca e fiscali.</span><span class="sxs-lookup"><span data-stu-id="b12c5-120">Incentives Users can view Incentive earnings and payment details and reports, but can’t edit bank and tax details.</span></span>

### <a name="choose-your-disbursement-currency"></a><span data-ttu-id="b12c5-121">Scegliere la valuta per il pagamento</span><span class="sxs-lookup"><span data-stu-id="b12c5-121">Choose your disbursement currency</span></span>

<span data-ttu-id="b12c5-122">Per impostazione predefinita, i pagamenti per gli incentivi vengono effettuati nella valuta locale di ogni entità corrispondente.</span><span class="sxs-lookup"><span data-stu-id="b12c5-122">By default, incentives payments are made in the local currency of each respective entity.</span></span> <span data-ttu-id="b12c5-123">È possibile specificare una valuta diversa durante la configurazione del profilo.</span><span class="sxs-lookup"><span data-stu-id="b12c5-123">You can specify a different currency during profile setup.</span></span> <span data-ttu-id="b12c5-124">I pagamenti verranno calcolati usando un tasso di cambio impostato su base mensile da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b12c5-124">Payments will be calculated using an exchange rate as set monthly by Microsoft.</span></span> <span data-ttu-id="b12c5-125">L'utente sarà responsabile di tutte le modifiche apportate al valore a causa della valuta selezionata.</span><span class="sxs-lookup"><span data-stu-id="b12c5-125">You’ll be responsible for any changes in value due to the currency selected.</span></span>

### <a name="bank-and-tax-information-and-other-programs"></a><span data-ttu-id="b12c5-126">Informazioni bancarie e fiscali e altri programmi</span><span class="sxs-lookup"><span data-stu-id="b12c5-126">Bank and tax information and other programs</span></span>

<span data-ttu-id="b12c5-127">Fornire le informazioni descritte di seguito anche se Microsoft utilizza già i dati bancari per i pagamenti.</span><span class="sxs-lookup"><span data-stu-id="b12c5-127">Provide the information described below even if Microsoft already uses your bank data for payments.</span></span> <span data-ttu-id="b12c5-128">Ciò consente di garantire la privacy e la sicurezza dei dati aziendali, perché la copia del profilo nel nuovo strumento potrebbe esporre informazioni riservate.</span><span class="sxs-lookup"><span data-stu-id="b12c5-128">This helps ensure the privacy and security of your company’s data, since copying your profile to the new tool could expose sensitive information.</span></span> <span data-ttu-id="b12c5-129">L'esecuzione di questo processo è anche un'opportunità ideale per garantire che i dati siano completi e accurati.</span><span class="sxs-lookup"><span data-stu-id="b12c5-129">Going through this process is also a good opportunity to ensure the data is complete and accurate.</span></span>

### <a name="using-different-profiles-for-different-microsoft-programs"></a><span data-ttu-id="b12c5-130">Uso di profili diversi per programmi Microsoft diversi</span><span class="sxs-lookup"><span data-stu-id="b12c5-130">Using different profiles for different Microsoft programs</span></span>

<span data-ttu-id="b12c5-131">All'interno del dettaglio, i pagamenti per ognuno dei cinque programmi per incentivi al dettaglio possono essere inviati allo stesso account bancario.</span><span class="sxs-lookup"><span data-stu-id="b12c5-131">Within retail, payments for each of the five retail incentive programs can go to the same bank account.</span></span> <span data-ttu-id="b12c5-132">In alternativa, è possibile scegliere di fare in modo che i pagamenti per la vendita al dettaglio vengano inseriti in un conto bancario mentre l'ufficio vendite al dettaglio viene pagato per un conto bancario diverso.</span><span class="sxs-lookup"><span data-stu-id="b12c5-132">Alternatively, you can choose to have Retail Xbox payments go into one bank account while Retail Office is paid to a different bank account.</span></span>

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="b12c5-133">Creare e gestire il profilo di pagamento e il profilo fiscale nel Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="b12c5-133">Create and manage payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="b12c5-134">Le sezioni seguenti illustrano il processo di creazione e gestione dei profili di pagamento e di imposta nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="b12c5-134">The sections below will walk you through the process of creating and managing payment and tax profiles in Partner Center.</span></span>

>[!IMPORTANT]
><span data-ttu-id="b12c5-135">È necessario essere un amministratore di incentivi per creare o gestire i profili di pagamento nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="b12c5-135">You must be an Incentive admin to create or manage payment profiles in Partner Center.</span></span> <span data-ttu-id="b12c5-136">I ruoli incentivo devono essere assegnati a ogni località MPN in ogni programma di incentivi.</span><span class="sxs-lookup"><span data-stu-id="b12c5-136">Incentive roles must be assigned to each MPN location under each incentive program.</span></span> <span data-ttu-id="b12c5-137">Per altre informazioni su come aggiungere gli amministratori di incentivi in Partner Center, vedere [creare account utente](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="b12c5-137">For more information on how to add Incentive admins in Partner Center, see [Create user accounts](create-user-accounts-and-set-permissions.md).</span></span>

## <a name="access-the-payout-and-tax-section-in-partner-center"></a><span data-ttu-id="b12c5-138">Accedere alla sezione relativa ai pagamenti e alle imposte nel centro per i partner</span><span class="sxs-lookup"><span data-stu-id="b12c5-138">Access the payout and tax section in Partner Center</span></span>

1. <span data-ttu-id="b12c5-139">Accedere al [Dashboard del centro](https://partner.microsoft.com/dashboard/) per i partner usando l'account Azure Active Directory (Azure ad) (account aziendale) o l'indirizzo di posta elettronica appropriato se ne è stato assegnato uno.</span><span class="sxs-lookup"><span data-stu-id="b12c5-139">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/) using your Azure Active Directory (Azure AD) account (company account), or the appropriate email address if one was assigned.</span></span>

   - <span data-ttu-id="b12c5-140">È possibile registrare più domini all'interno di un account Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b12c5-140">Multiple domains can be registered within one Azure AD account.</span></span> <span data-ttu-id="b12c5-141">Contattare l'amministratore globale per determinare quali domini sono associati.</span><span class="sxs-lookup"><span data-stu-id="b12c5-141">Contact your Global admin to determine which domains are associated.</span></span>
   - <span data-ttu-id="b12c5-142">Se si è in grado di accedere solo con il @onmicrosoft.com dominio, contattare l'amministratore dell'account per aggiungere ulteriori domini all'account Azure ad.</span><span class="sxs-lookup"><span data-stu-id="b12c5-142">If you're only able to log in with the @onmicrosoft.com domain, contact your Account admin to add additional domains to the Azure AD account.</span></span>
   - <span data-ttu-id="b12c5-143">Se viene richiesto di selezionare un account aziendale o dell' **Istituto di istruzione** o un account **personale**, selezionare account aziendale o dell'Istituto di **istruzione**.</span><span class="sxs-lookup"><span data-stu-id="b12c5-143">If you're prompted to select **Work or school account** or **Personal Account**, select **Work or school account**.</span></span>

2. <span data-ttu-id="b12c5-144">Selezionare l'icona a forma di ingranaggio per aprire il menu **Impostazioni** , quindi selezionare **Impostazioni partner**.</span><span class="sxs-lookup"><span data-stu-id="b12c5-144">Select the gear icon to open the **Settings** menu, and then select **Partner settings**.</span></span>

3. <span data-ttu-id="b12c5-145">Nel menu **Impostazioni account** selezionare **pagamenti e imposte**.</span><span class="sxs-lookup"><span data-stu-id="b12c5-145">In the **Account settings** menu, select **Payout and tax**.</span></span> 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a><span data-ttu-id="b12c5-146">Assegnare i profili di pagamento e di imposta a singoli programmi</span><span class="sxs-lookup"><span data-stu-id="b12c5-146">Assign payout and tax profiles to individual programs</span></span>

1. <span data-ttu-id="b12c5-147">Accedere al [Dashboard del centro](https://partner.microsoft.com/dashboard/)per i partner, quindi selezionare l'icona a forma di ingranaggio per aprire il menu **Impostazioni** .</span><span class="sxs-lookup"><span data-stu-id="b12c5-147">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/), and then select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="b12c5-148">Selezionare **Impostazioni partner**, espandere la **sezione pagamenti e imposte**, quindi selezionare **assegnazione del profilo di pagamento e di imposta**.</span><span class="sxs-lookup"><span data-stu-id="b12c5-148">Select **Partner settings**, expand the **Payout and tax section**, and then select **Payout and tax profile assignment**.</span></span> 
   
   <span data-ttu-id="b12c5-149">Verrà visualizzato un elenco dei programmi.</span><span class="sxs-lookup"><span data-stu-id="b12c5-149">A list of your programs will be displayed.</span></span> <span data-ttu-id="b12c5-150">Selezionare la freccia accanto a un programma per visualizzare i dettagli del profilo.</span><span class="sxs-lookup"><span data-stu-id="b12c5-150">Select the arrow next to a program to see profile details.</span></span> 

3. <span data-ttu-id="b12c5-151">Nel menu a discesa **profilo fiscale** selezionare il profilo fiscale desiderato oppure selezionare l'opzione per creare un nuovo profilo.</span><span class="sxs-lookup"><span data-stu-id="b12c5-151">In the **Tax Profile** dropdown menu, select the tax profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="b12c5-152">Quando si seleziona l'opzione per creare un nuovo profilo, si verrà reindirizzati in modo appropriato.</span><span class="sxs-lookup"><span data-stu-id="b12c5-152">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="b12c5-153">Selezionare continua nella finestra popup.</span><span class="sxs-lookup"><span data-stu-id="b12c5-153">Select Continue in the pop-up window.</span></span> <span data-ttu-id="b12c5-154">Il processo per la creazione di un nuovo profilo fiscale è stato fornito di seguito.</span><span class="sxs-lookup"><span data-stu-id="b12c5-154">The process for creating a new tax profile has been provided below.</span></span>

4. <span data-ttu-id="b12c5-155">Selezionare il **metodo di pagamento**.</span><span class="sxs-lookup"><span data-stu-id="b12c5-155">Select **Payment method**.</span></span>

   - <span data-ttu-id="b12c5-156">Se è stato selezionato **Electronic Bank Transfer** come metodo di pagamento, selezionare il profilo di pagamento desiderato oppure selezionare l'opzione per creare un nuovo profilo.</span><span class="sxs-lookup"><span data-stu-id="b12c5-156">If you have selected **Electronic bank transfer** as your payment method, select the payment profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="b12c5-157">Quando si seleziona l'opzione per creare un nuovo profilo, si verrà reindirizzati in modo appropriato.</span><span class="sxs-lookup"><span data-stu-id="b12c5-157">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span> <span data-ttu-id="b12c5-158">Selezionare continua nella finestra popup.</span><span class="sxs-lookup"><span data-stu-id="b12c5-158">Select Continue in the pop-up window.</span></span> <span data-ttu-id="b12c5-159">Di seguito è riportato il processo per la creazione di un nuovo profilo di pagamento.</span><span class="sxs-lookup"><span data-stu-id="b12c5-159">The process for creating a new payment profile has been provided below.</span></span>

   - <span data-ttu-id="b12c5-160">Se è stata selezionata la **Nota di credito** come metodo di pagamento, completare la verifica.</span><span class="sxs-lookup"><span data-stu-id="b12c5-160">If you have selected **Credit Note** as your payment method, then complete the verification.</span></span> <span data-ttu-id="b12c5-161">In questo modo viene confermato che il numero SAP a cui si fa riferimento appartiene all'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="b12c5-161">This confirms that the referenced SAP number belongs to your organization.</span></span>

    >[!NOTE]
    ><span data-ttu-id="b12c5-162">Se sono elencate più entità aziendali Microsoft, è necessario selezionare un profilo di pagamento per ogni entità.</span><span class="sxs-lookup"><span data-stu-id="b12c5-162">If there are multiple Microsoft business entities listed, you must select a payment profile for each entity.</span></span>

    >[!NOTE]
    ><span data-ttu-id="b12c5-163">La disponibilità dei metodi di pagamento dipende dalle regole del programma di incentivi.</span><span class="sxs-lookup"><span data-stu-id="b12c5-163">The payment method availability is dependent on the rules of the incentive program.</span></span>
    
5. <span data-ttu-id="b12c5-164">Selezionare la **valuta**.</span><span class="sxs-lookup"><span data-stu-id="b12c5-164">Select the **Currency**.</span></span>

6. <span data-ttu-id="b12c5-165">Una volta completati tutti i campi di pagamento, selezionare **Invia**.</span><span class="sxs-lookup"><span data-stu-id="b12c5-165">When you’ve completed all of the payment fields, select **Submit**.</span></span>

## <a name="create-your-bank-profile"></a><span data-ttu-id="b12c5-166">Creare il profilo bancario</span><span class="sxs-lookup"><span data-stu-id="b12c5-166">Create your bank profile</span></span>

<span data-ttu-id="b12c5-167">I profili bancari vengono creati a livello di organizzazione.</span><span class="sxs-lookup"><span data-stu-id="b12c5-167">Bank profiles are created at an organization level.</span></span> <span data-ttu-id="b12c5-168">Questo consente l'assegnazione di un profilo bancario tra più ID MPN e programmi incentive all'interno di un'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="b12c5-168">This allows one bank profile to be assigned across multiple MPN ID’s and incentive programs within an organization.</span></span> <span data-ttu-id="b12c5-169">È possibile che si verifichino eccezioni durante l'applicazione del profilo bancario a paesi diversi, in quanto possono essere applicate diverse regole fiscali e bancarie.</span><span class="sxs-lookup"><span data-stu-id="b12c5-169">There may be exceptions when applying the banking profile to different countries, as different banking and tax rules may apply.</span></span>

>[!NOTE]
><span data-ttu-id="b12c5-170">Nelle pagine seguenti sono necessari campi con un asterisco.</span><span class="sxs-lookup"><span data-stu-id="b12c5-170">On the following pages, fields with an asterisk are required.</span></span> <span data-ttu-id="b12c5-171">Se non si conosce il campo, selezionare l'icona informazioni.</span><span class="sxs-lookup"><span data-stu-id="b12c5-171">If you don’t know what a field is, select the information icon.</span></span> 

1. <span data-ttu-id="b12c5-172">Nella pagina **Dettagli** completare i campi seguenti: **nome profilo:** immettere un nome univoco per identificare il profilo di pagamento.</span><span class="sxs-lookup"><span data-stu-id="b12c5-172">On the **Details** page, complete the following fields: **Profile name:** Enter a unique name to identify this payment profile.</span></span>
    <span data-ttu-id="b12c5-173">**Posizione conto bancario:** Il paese in cui si trova la banca della società.</span><span class="sxs-lookup"><span data-stu-id="b12c5-173">**Bank account location:** The country in which your company’s bank is located.</span></span>
    <span data-ttu-id="b12c5-174">**Metodo di pagamento:** Il metodo di pagamento preferito per il centro per i partner è il trasferimento bancario elettronico.</span><span class="sxs-lookup"><span data-stu-id="b12c5-174">**Payment method:** The preferred payment method for Partner Center is electronic bank transfer.</span></span>

2. <span data-ttu-id="b12c5-175">Selezionare **Avanti**.</span><span class="sxs-lookup"><span data-stu-id="b12c5-175">Select **Next**.</span></span>

3. <span data-ttu-id="b12c5-176">Nella pagina **conto bancario** immettere le informazioni.</span><span class="sxs-lookup"><span data-stu-id="b12c5-176">On the **Bank account** page, enter your information.</span></span> <span data-ttu-id="b12c5-177">I campi visualizzati in questa pagina variano in base al paese.</span><span class="sxs-lookup"><span data-stu-id="b12c5-177">Fields shown on this page will vary by country.</span></span> 

4. <span data-ttu-id="b12c5-178">Selezionare **Avanti**.</span><span class="sxs-lookup"><span data-stu-id="b12c5-178">Select **Next**.</span></span>

5. <span data-ttu-id="b12c5-179">Nella pagina **beneficiari** immettere le informazioni appropriate.</span><span class="sxs-lookup"><span data-stu-id="b12c5-179">On the **Beneficiary** page, enter the appropriate information.</span></span> <span data-ttu-id="b12c5-180">Il beneficiario è la persona dell'azienda a cui la banca potrebbe rivolgersi se deve discutere l'account.</span><span class="sxs-lookup"><span data-stu-id="b12c5-180">The beneficiary is the person in your company that the bank would contact if they need to discuss your account.</span></span>

6. <span data-ttu-id="b12c5-181">Una volta completati i campi, selezionare **fine**, quindi selezionare **conferma** per creare il profilo bancario.</span><span class="sxs-lookup"><span data-stu-id="b12c5-181">When the fields are completed, select **Finish**, and then select **Confirm** to create your bank profile.</span></span>

<span data-ttu-id="b12c5-182">Si verrà reindirizzati alla pagina dei **profili di pagamento e fiscali** .</span><span class="sxs-lookup"><span data-stu-id="b12c5-182">You’ll be redirected to the **Payout and tax profiles** page.</span></span> <span data-ttu-id="b12c5-183">Lo stato del nuovo profilo rifletterà la **convalida Microsoft in sospeso** fino a quando non sarà stata completata la convalida.</span><span class="sxs-lookup"><span data-stu-id="b12c5-183">The status of your new profile will reflect **Pending Microsoft validation** until the validation has been completed.</span></span> <span data-ttu-id="b12c5-184">Questo processo può richiedere fino a 48 ore.</span><span class="sxs-lookup"><span data-stu-id="b12c5-184">This process may take up to 48 hours.</span></span> <span data-ttu-id="b12c5-185">Al termine della convalida, lo stato del profilo rifletterà l' **approvazione** o l' **azione richiesta**.</span><span class="sxs-lookup"><span data-stu-id="b12c5-185">Once validation has been completed, your profile status will reflect either **Approved** or **Action required**.</span></span> <span data-ttu-id="b12c5-186">Se è **richiesta l'azione**, ripetere i passaggi precedenti fornendo le informazioni necessarie.</span><span class="sxs-lookup"><span data-stu-id="b12c5-186">If **Action Required**, repeat the steps above providing the necessary information.</span></span> 

## <a name="create-your-tax-profile"></a><span data-ttu-id="b12c5-187">Creare il profilo fiscale</span><span class="sxs-lookup"><span data-stu-id="b12c5-187">Create your tax profile</span></span>

<span data-ttu-id="b12c5-188">Utilizzare la seguente procedura per fornire a Microsoft le informazioni fiscali necessarie per l'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="b12c5-188">Use the following procedure to provide Microsoft with the tax information required for your organization.</span></span> <span data-ttu-id="b12c5-189">Le pagine di questa sezione sono dinamiche e variano in base al paese o all'area geografica.</span><span class="sxs-lookup"><span data-stu-id="b12c5-189">The pages in this section are dynamic and will vary according to your country or region.</span></span> <span data-ttu-id="b12c5-190">Se è necessario assistenza per identificare le informazioni fiscali corrette, contattare le fonti governative appropriate nel proprio paese.</span><span class="sxs-lookup"><span data-stu-id="b12c5-190">If you need help with identifying the correct tax information, contact the appropriate government sources in your country.</span></span>

<span data-ttu-id="b12c5-191">Per le società partner in America, se sono necessarie informazioni sul completamento dei moduli W8 o W9, i seguenti indirizzi indirizzano al sito di IRS:</span><span class="sxs-lookup"><span data-stu-id="b12c5-191">For partner companies in the Americas, if you require information on completing the W8 or W9 forms, the following addresses take you to the IRS site:</span></span>

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> <span data-ttu-id="b12c5-192">Immettere solo i dettagli della società.</span><span class="sxs-lookup"><span data-stu-id="b12c5-192">Enter only details for your company.</span></span> <span data-ttu-id="b12c5-193">Non immettere mai i dettagli personali.</span><span class="sxs-lookup"><span data-stu-id="b12c5-193">Never enter personal details.</span></span>

1. <span data-ttu-id="b12c5-194">Nella pagina **profilo business** completare i campi obbligatori e quindi fare clic su **Avanti**.</span><span class="sxs-lookup"><span data-stu-id="b12c5-194">On the **Business Profile** page, complete the required fields and then select **Next**.</span></span> 

2. <span data-ttu-id="b12c5-195">Nella pagina di **installazione** selezionare l'opzione che si applica alla società.</span><span class="sxs-lookup"><span data-stu-id="b12c5-195">On the **Setup** page, select the option that applies to your company.</span></span>

   - <span data-ttu-id="b12c5-196">Selezionare l'opzione a sinistra se la società è incorporata solo nel Stati Uniti o se il profilo è per un singolo utente.</span><span class="sxs-lookup"><span data-stu-id="b12c5-196">Select the option on the left if your company is incorporated in the United States only, or if this profile is for an individual.</span></span>
   - <span data-ttu-id="b12c5-197">Selezionare l'opzione a destra se la società è incorporata all'esterno del Stati Uniti, quindi selezionare il paese dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="b12c5-197">Select the option on the right if your company is incorporated outside of the United States, and then select your country/region from the list.</span></span>

3. <span data-ttu-id="b12c5-198">Selezionare **Avanti**.</span><span class="sxs-lookup"><span data-stu-id="b12c5-198">Select **Next**.</span></span> 

4. <span data-ttu-id="b12c5-199">Nella pagina **Tax status** immettere le informazioni necessarie e quindi fare clic su **Next (avanti**).</span><span class="sxs-lookup"><span data-stu-id="b12c5-199">On the **Tax status** page, enter the required information, and then select **Next**.</span></span> <span data-ttu-id="b12c5-200">I campi in questa pagina variano in base al paese.</span><span class="sxs-lookup"><span data-stu-id="b12c5-200">Fields on this page will vary by country.</span></span> <span data-ttu-id="b12c5-201">dettagli.</span><span class="sxs-lookup"><span data-stu-id="b12c5-201">your details.</span></span> 

5. <span data-ttu-id="b12c5-202">Nella pagina **documentazione aggiuntiva** , i campi obbligatori e selezionare **Avanti**.</span><span class="sxs-lookup"><span data-stu-id="b12c5-202">On the **Additional documentation** page, the required fields and select **Next**.</span></span> 

6. <span data-ttu-id="b12c5-203">Selezionare **Browse (Sfoglia** ) per caricare i documenti richiesti dal paese o dall'area geografica.</span><span class="sxs-lookup"><span data-stu-id="b12c5-203">Select **Browse** to upload any documents required by your country or region.</span></span> <span data-ttu-id="b12c5-204">Quando viene visualizzato il nome del documento, selezionare **carica**.</span><span class="sxs-lookup"><span data-stu-id="b12c5-204">When the document name is shown, select **Upload**.</span></span> 

7. <span data-ttu-id="b12c5-205">Se è necessario rimuovere il documento, selezionare **Rimuovi**.</span><span class="sxs-lookup"><span data-stu-id="b12c5-205">If you need to remove the document, select **Remove**.</span></span>

8. <span data-ttu-id="b12c5-206">Per salvare e continuare, selezionare **fine**.</span><span class="sxs-lookup"><span data-stu-id="b12c5-206">To save and continue, select **Finish**.</span></span>

9. <span data-ttu-id="b12c5-207">Selezionare **conferma** nel messaggio popup.</span><span class="sxs-lookup"><span data-stu-id="b12c5-207">Select **Confirm** on the pop-up message.</span></span> <span data-ttu-id="b12c5-208">Verrà ripristinata la pagina di **configurazione dei pagamenti e delle imposte** .</span><span class="sxs-lookup"><span data-stu-id="b12c5-208">You’ll be taken back to the **Payout and tax setup** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b12c5-209">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="b12c5-209">Next steps</span></span>

- [<span data-ttu-id="b12c5-210">Domande frequenti su proventi da incentivi e profilo fiscale</span><span class="sxs-lookup"><span data-stu-id="b12c5-210">Incentives payout and tax profile FAQs</span></span>](incentives-payout-tax-profile-faqs.md)
