---
title: Profili di pagamento e fiscali nel Centro per i partner
ms.topic: how-to
ms.date: 11/12/2020
description: Crea e Gestisci il tuo profilo di pagamento e di imposte, in modo da potervi pagare per il lavoro di incentivi. Include la creazione, la gestione e l'uso di profili diversi.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: 66177c6e3cd0091081866e1508d28346f49ec713
ms.sourcegitcommit: bfc9e6f6476766cf10ba714f03ca2e96560003b1
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/14/2020
ms.locfileid: "94626032"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="677cd-104">Creazione e gestione di incentivi per il pagamento e i profili fiscali nel centro per i partner</span><span class="sxs-lookup"><span data-stu-id="677cd-104">Create and manage incentives payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="677cd-105">**Si applica a:**</span><span class="sxs-lookup"><span data-stu-id="677cd-105">**Applies to:**</span></span>

- <span data-ttu-id="677cd-106">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="677cd-106">Partner Center</span></span>

<span data-ttu-id="677cd-107">**Ruoli appropriati:**</span><span class="sxs-lookup"><span data-stu-id="677cd-107">**Appropriate roles:**</span></span>

- <span data-ttu-id="677cd-108">Amministratore degli incentivi</span><span class="sxs-lookup"><span data-stu-id="677cd-108">Incentives admin</span></span>
- <span data-ttu-id="677cd-109">Amministratore degli account</span><span class="sxs-lookup"><span data-stu-id="677cd-109">Account admin</span></span>
- <span data-ttu-id="677cd-110">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="677cd-110">Global admin</span></span>

<span data-ttu-id="677cd-111">Prima di poter ricevere il pagamento per i programmi Incentivi per una particolare posizione MPN, è necessario completare la registrazione associando un profilo di pagamento e fiscale valido al programma e alla posizione MPN.</span><span class="sxs-lookup"><span data-stu-id="677cd-111">Before you can receive payment for your incentive programs for a particular MPN location, you must complete your enrollment by associating a valid payout and tax profile with the program and MPN location.</span></span> <span data-ttu-id="677cd-112">Microsoft userà il profilo di pagamento e fiscale per emettere i pagamenti.</span><span class="sxs-lookup"><span data-stu-id="677cd-112">Microsoft will use this payout and tax profile to issue payments.</span></span> <span data-ttu-id="677cd-113">È possibile che l'utente sia autorizzato a usare il trasferimento bancario elettronico o una nota di accredito per il pagamento, a seconda delle regole del programma Incentivi.</span><span class="sxs-lookup"><span data-stu-id="677cd-113">You may be allowed to use electronic bank transfer or a credit note for payment, depending on the rules of the incentive program.</span></span> 

## <a name="roles-currencies-and-other-microsoft-programs"></a><span data-ttu-id="677cd-114">Ruoli, valute e altri programmi Microsoft</span><span class="sxs-lookup"><span data-stu-id="677cd-114">Roles, currencies, and other Microsoft programs</span></span>

<span data-ttu-id="677cd-115">È importante comprendere le informazioni riportate di seguito prima di iniziare con il profilo di pagamento e di imposta.</span><span class="sxs-lookup"><span data-stu-id="677cd-115">It's important to understand the information below before you get started with your payout and tax profile.</span></span>

### <a name="roles-and-permissions"></a><span data-ttu-id="677cd-116">Ruoli e autorizzazioni</span><span class="sxs-lookup"><span data-stu-id="677cd-116">Roles and permissions</span></span>

<span data-ttu-id="677cd-117">È necessario essere un amministratore di incentivi per immettere le informazioni fiscali e bancarie per i pagamenti di incentivi.</span><span class="sxs-lookup"><span data-stu-id="677cd-117">You must be an Incentives Admin to enter bank and tax information for incentive payments.</span></span> <span data-ttu-id="677cd-118">Se si è un amministratore MPN/account, è possibile assegnare se stessi e/o un collega come amministratore di incentivi.</span><span class="sxs-lookup"><span data-stu-id="677cd-118">If you're an MPN/Account Admin, you can assign yourself and/or a colleague to be the Incentives Admin.</span></span>

<span data-ttu-id="677cd-119">Se è necessario richiedere le autorizzazioni di amministratore per gli incentivi, contattare l'amministratore MPN o l'amministratore globale. È possibile scoprire chi ha questi ruoli nell'azienda accedendo al [Dashboard del centro](https://partner.microsoft.com/dashboard/)per i partner.</span><span class="sxs-lookup"><span data-stu-id="677cd-119">If you need to request Incentives Admin permissions, contact your MPN Admin or Global Admin. You can find out who in your company has these roles by signing into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span> <span data-ttu-id="677cd-120">Dall'icona **Impostazioni** in alto a destra selezionare **Gestione utenti** , quindi filtrare in base a amministratore globale.</span><span class="sxs-lookup"><span data-stu-id="677cd-120">From the **Settings** icon at the top right, select **User Management** and then filter on Global Admin.</span></span>

<span data-ttu-id="677cd-121">Gli incentivi consentono agli utenti di visualizzare i guadagni e i dettagli di pagamento e i report, ma non possono modificare i dettagli di banca e fiscali.</span><span class="sxs-lookup"><span data-stu-id="677cd-121">Incentives Users can view Incentive earnings and payment details and reports, but can’t edit bank and tax details.</span></span>

### <a name="choose-your-disbursement-currency"></a><span data-ttu-id="677cd-122">Scegliere la valuta per il pagamento</span><span class="sxs-lookup"><span data-stu-id="677cd-122">Choose your disbursement currency</span></span>

<span data-ttu-id="677cd-123">I pagamenti degli incentivi vengono effettuati nella valuta selezionata durante la configurazione del profilo di pagamento.</span><span class="sxs-lookup"><span data-stu-id="677cd-123">Incentive payments are made in the currency you selected when you set up your payment profile.</span></span> <span data-ttu-id="677cd-124">I pagamenti verranno calcolati usando un tasso di cambio impostato su base mensile da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="677cd-124">Payments will be calculated using an exchange rate as set monthly by Microsoft.</span></span> <span data-ttu-id="677cd-125">L'utente sarà responsabile di tutte le modifiche apportate al valore a causa della valuta selezionata.</span><span class="sxs-lookup"><span data-stu-id="677cd-125">You’ll be responsible for any changes in value due to the currency selected.</span></span>

### <a name="using-different-profiles-for-different-microsoft-programs"></a><span data-ttu-id="677cd-126">Uso di profili diversi per programmi Microsoft diversi</span><span class="sxs-lookup"><span data-stu-id="677cd-126">Using different profiles for different Microsoft programs</span></span>

<span data-ttu-id="677cd-127">Se la società è registrata in più programmi incentive, è possibile usare lo stesso account di pagamento per tutti i programmi o scegliere di usare account di pagamento diversi per programmi diversi.</span><span class="sxs-lookup"><span data-stu-id="677cd-127">If your company is enrolled in multiple incentive programs, you can use the same payment account for all of them, or choose to use different payment accounts for different programs.</span></span>

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="677cd-128">Creare e gestire il profilo di pagamento e il profilo fiscale nel Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="677cd-128">Create and manage payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="677cd-129">Le sezioni seguenti illustrano il processo di creazione e gestione dei profili di pagamento e di imposta nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="677cd-129">The sections below will walk you through the process of creating and managing payment and tax profiles in Partner Center.</span></span>

>[!IMPORTANT]
><span data-ttu-id="677cd-130">È necessario essere un amministratore di incentivi per creare o gestire i profili di pagamento nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="677cd-130">You must be an Incentive admin to create or manage payment profiles in Partner Center.</span></span> <span data-ttu-id="677cd-131">I ruoli incentivo devono essere assegnati a ogni località MPN in ogni programma di incentivi.</span><span class="sxs-lookup"><span data-stu-id="677cd-131">Incentive roles must be assigned to each MPN location under each incentive program.</span></span> <span data-ttu-id="677cd-132">Per altre informazioni su come aggiungere gli amministratori di incentivi in Partner Center, vedere [creare account utente](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="677cd-132">For more information on how to add Incentive admins in Partner Center, see [Create user accounts](create-user-accounts-and-set-permissions.md).</span></span>

## <a name="access-the-payout-and-tax-section-in-partner-center"></a><span data-ttu-id="677cd-133">Accedere alla sezione relativa ai pagamenti e alle imposte nel centro per i partner</span><span class="sxs-lookup"><span data-stu-id="677cd-133">Access the payout and tax section in Partner Center</span></span>

1. <span data-ttu-id="677cd-134">Accedere al [Dashboard del centro](https://partner.microsoft.com/dashboard/) per i partner usando l'account Azure Active Directory (Azure ad) (account aziendale) o l'indirizzo di posta elettronica appropriato se ne è stato assegnato uno.</span><span class="sxs-lookup"><span data-stu-id="677cd-134">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/) using your Azure Active Directory (Azure AD) account (company account), or the appropriate email address if one was assigned.</span></span>

   - <span data-ttu-id="677cd-135">È possibile registrare più domini all'interno di un account Azure AD.</span><span class="sxs-lookup"><span data-stu-id="677cd-135">Multiple domains can be registered within one Azure AD account.</span></span> <span data-ttu-id="677cd-136">Contattare l'amministratore globale per determinare quali domini sono associati.</span><span class="sxs-lookup"><span data-stu-id="677cd-136">Contact your Global admin to determine which domains are associated.</span></span>
   - <span data-ttu-id="677cd-137">Se si è in grado di accedere solo con il @onmicrosoft.com dominio, contattare l'amministratore dell'account per aggiungere ulteriori domini all'account Azure ad.</span><span class="sxs-lookup"><span data-stu-id="677cd-137">If you're only able to log in with the @onmicrosoft.com domain, contact your Account admin to add additional domains to the Azure AD account.</span></span>
   - <span data-ttu-id="677cd-138">Se viene richiesto di selezionare un account aziendale o dell' **Istituto di istruzione** o un account **personale** , selezionare account aziendale o dell'Istituto di **istruzione**.</span><span class="sxs-lookup"><span data-stu-id="677cd-138">If you're prompted to select **Work or school account** or **Personal Account** , select **Work or school account**.</span></span>

2. <span data-ttu-id="677cd-139">Selezionare l'icona a forma di ingranaggio per aprire il menu **Impostazioni** , quindi selezionare **Impostazioni partner**.</span><span class="sxs-lookup"><span data-stu-id="677cd-139">Select the gear icon to open the **Settings** menu, and then select **Partner settings**.</span></span>

3. <span data-ttu-id="677cd-140">Nel menu **Impostazioni account** selezionare **pagamenti e imposte**.</span><span class="sxs-lookup"><span data-stu-id="677cd-140">In the **Account settings** menu, select **Payout and tax**.</span></span> 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a><span data-ttu-id="677cd-141">Assegnare i profili di pagamento e di imposta a singoli programmi</span><span class="sxs-lookup"><span data-stu-id="677cd-141">Assign payout and tax profiles to individual programs</span></span>

1. <span data-ttu-id="677cd-142">Accedere al [Dashboard del centro](https://partner.microsoft.com/dashboard/)per i partner, quindi selezionare l'icona a forma di ingranaggio per aprire il menu **Impostazioni** .</span><span class="sxs-lookup"><span data-stu-id="677cd-142">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/), and then select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="677cd-143">Selezionare **Impostazioni partner** , espandere la **sezione pagamenti e imposte** , quindi selezionare **assegnazione del profilo di pagamento e di imposta**.</span><span class="sxs-lookup"><span data-stu-id="677cd-143">Select **Partner settings** , expand the **Payout and tax section** , and then select **Payout and tax profile assignment**.</span></span> 
   
   <span data-ttu-id="677cd-144">Verrà visualizzato un elenco dei programmi.</span><span class="sxs-lookup"><span data-stu-id="677cd-144">A list of your programs will be displayed.</span></span> <span data-ttu-id="677cd-145">Selezionare la freccia accanto a un programma per visualizzare i dettagli del profilo.</span><span class="sxs-lookup"><span data-stu-id="677cd-145">Select the arrow next to a program to see profile details.</span></span> 

3. <span data-ttu-id="677cd-146">Nel menu a discesa **profilo fiscale** selezionare il profilo fiscale desiderato oppure selezionare l'opzione per creare un nuovo profilo.</span><span class="sxs-lookup"><span data-stu-id="677cd-146">In the **Tax Profile** dropdown menu, select the tax profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="677cd-147">Quando si seleziona l'opzione per creare un nuovo profilo, si verrà reindirizzati in modo appropriato.</span><span class="sxs-lookup"><span data-stu-id="677cd-147">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="677cd-148">Selezionare continua nella finestra popup.</span><span class="sxs-lookup"><span data-stu-id="677cd-148">Select Continue in the pop-up window.</span></span> <span data-ttu-id="677cd-149">Il processo per la creazione di un nuovo profilo fiscale è stato fornito di seguito.</span><span class="sxs-lookup"><span data-stu-id="677cd-149">The process for creating a new tax profile has been provided below.</span></span>

4. <span data-ttu-id="677cd-150">Selezionare il **metodo di pagamento**.</span><span class="sxs-lookup"><span data-stu-id="677cd-150">Select **Payment method**.</span></span>

   - <span data-ttu-id="677cd-151">Se è stato selezionato **Electronic Bank Transfer** come metodo di pagamento, selezionare il profilo di pagamento desiderato oppure selezionare l'opzione per creare un nuovo profilo.</span><span class="sxs-lookup"><span data-stu-id="677cd-151">If you have selected **Electronic bank transfer** as your payment method, select the payment profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="677cd-152">Quando si seleziona l'opzione per creare un nuovo profilo, si verrà reindirizzati in modo appropriato.</span><span class="sxs-lookup"><span data-stu-id="677cd-152">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span> <span data-ttu-id="677cd-153">Selezionare continua nella finestra popup.</span><span class="sxs-lookup"><span data-stu-id="677cd-153">Select Continue in the pop-up window.</span></span> <span data-ttu-id="677cd-154">Di seguito è riportato il processo per la creazione di un nuovo profilo di pagamento.</span><span class="sxs-lookup"><span data-stu-id="677cd-154">The process for creating a new payment profile has been provided below.</span></span>

   - <span data-ttu-id="677cd-155">Se è stata selezionata la **Nota di credito** come metodo di pagamento, completare la verifica.</span><span class="sxs-lookup"><span data-stu-id="677cd-155">If you have selected **Credit Note** as your payment method, then complete the verification.</span></span> <span data-ttu-id="677cd-156">In questo modo viene confermato che il numero SAP a cui si fa riferimento appartiene all'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="677cd-156">This confirms that the referenced SAP number belongs to your organization.</span></span>

    >[!NOTE]
    ><span data-ttu-id="677cd-157">Se sono elencate più entità aziendali Microsoft, è necessario selezionare un profilo di pagamento per ogni entità.</span><span class="sxs-lookup"><span data-stu-id="677cd-157">If there are multiple Microsoft business entities listed, you must select a payment profile for each entity.</span></span>

    >[!NOTE]
    ><span data-ttu-id="677cd-158">La disponibilità dei metodi di pagamento dipende dalle regole del programma di incentivi.</span><span class="sxs-lookup"><span data-stu-id="677cd-158">The payment method availability is dependent on the rules of the incentive program.</span></span>
    
5. <span data-ttu-id="677cd-159">Selezionare la **valuta**.</span><span class="sxs-lookup"><span data-stu-id="677cd-159">Select the **Currency**.</span></span>

6. <span data-ttu-id="677cd-160">Una volta completati tutti i campi di pagamento, selezionare **Invia**.</span><span class="sxs-lookup"><span data-stu-id="677cd-160">When you’ve completed all of the payment fields, select **Submit**.</span></span>

## <a name="create-your-bank-profile"></a><span data-ttu-id="677cd-161">Creare il profilo bancario</span><span class="sxs-lookup"><span data-stu-id="677cd-161">Create your bank profile</span></span>

<span data-ttu-id="677cd-162">I profili bancari vengono creati a livello di organizzazione.</span><span class="sxs-lookup"><span data-stu-id="677cd-162">Bank profiles are created at an organization level.</span></span> <span data-ttu-id="677cd-163">Questo consente l'assegnazione di un profilo bancario tra più ID MPN e programmi incentive all'interno di un'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="677cd-163">This allows one bank profile to be assigned across multiple MPN ID’s and incentive programs within an organization.</span></span> <span data-ttu-id="677cd-164">È possibile che si verifichino eccezioni durante l'applicazione del profilo bancario a paesi diversi, in quanto possono essere applicate diverse regole fiscali e bancarie.</span><span class="sxs-lookup"><span data-stu-id="677cd-164">There may be exceptions when applying the banking profile to different countries, as different banking and tax rules may apply.</span></span>

>[!NOTE]
><span data-ttu-id="677cd-165">Nelle pagine seguenti sono necessari campi con un asterisco.</span><span class="sxs-lookup"><span data-stu-id="677cd-165">On the following pages, fields with an asterisk are required.</span></span> <span data-ttu-id="677cd-166">Se non si conosce il campo, selezionare l'icona informazioni.</span><span class="sxs-lookup"><span data-stu-id="677cd-166">If you don’t know what a field is, select the information icon.</span></span> 

1. <span data-ttu-id="677cd-167">Nella pagina **Dettagli** completare i campi seguenti: **nome profilo:** immettere un nome univoco per identificare il profilo di pagamento.</span><span class="sxs-lookup"><span data-stu-id="677cd-167">On the **Details** page, complete the following fields: **Profile name:** Enter a unique name to identify this payment profile.</span></span>
    <span data-ttu-id="677cd-168">**Posizione conto bancario:** Il paese in cui si trova la banca della società.</span><span class="sxs-lookup"><span data-stu-id="677cd-168">**Bank account location:** The country in which your company’s bank is located.</span></span>
    <span data-ttu-id="677cd-169">**Metodo di pagamento:** Il metodo di pagamento preferito per il centro per i partner è il trasferimento bancario elettronico.</span><span class="sxs-lookup"><span data-stu-id="677cd-169">**Payment method:** The preferred payment method for Partner Center is electronic bank transfer.</span></span>

2. <span data-ttu-id="677cd-170">Selezionare **Avanti**.</span><span class="sxs-lookup"><span data-stu-id="677cd-170">Select **Next**.</span></span>

3. <span data-ttu-id="677cd-171">Nella pagina **conto bancario** immettere le informazioni.</span><span class="sxs-lookup"><span data-stu-id="677cd-171">On the **Bank account** page, enter your information.</span></span> <span data-ttu-id="677cd-172">I campi visualizzati in questa pagina variano in base al paese.</span><span class="sxs-lookup"><span data-stu-id="677cd-172">Fields shown on this page will vary by country.</span></span> 

4. <span data-ttu-id="677cd-173">Selezionare **Avanti**.</span><span class="sxs-lookup"><span data-stu-id="677cd-173">Select **Next**.</span></span>

5. <span data-ttu-id="677cd-174">Nella pagina **beneficiari** immettere le informazioni appropriate.</span><span class="sxs-lookup"><span data-stu-id="677cd-174">On the **Beneficiary** page, enter the appropriate information.</span></span> <span data-ttu-id="677cd-175">Il beneficiario è la persona dell'azienda a cui la banca potrebbe rivolgersi se deve discutere l'account.</span><span class="sxs-lookup"><span data-stu-id="677cd-175">The beneficiary is the person in your company that the bank would contact if they need to discuss your account.</span></span>

6. <span data-ttu-id="677cd-176">Una volta completati i campi, selezionare **fine** , quindi selezionare **conferma** per creare il profilo bancario.</span><span class="sxs-lookup"><span data-stu-id="677cd-176">When the fields are completed, select **Finish** , and then select **Confirm** to create your bank profile.</span></span>

<span data-ttu-id="677cd-177">Si verrà reindirizzati alla pagina dei **profili di pagamento e fiscali** .</span><span class="sxs-lookup"><span data-stu-id="677cd-177">You’ll be redirected to the **Payout and tax profiles** page.</span></span> <span data-ttu-id="677cd-178">Lo stato del nuovo profilo rifletterà la **convalida Microsoft in sospeso** fino a quando non sarà stata completata la convalida.</span><span class="sxs-lookup"><span data-stu-id="677cd-178">The status of your new profile will reflect **Pending Microsoft validation** until the validation has been completed.</span></span> <span data-ttu-id="677cd-179">Questo processo può richiedere fino a 48 ore.</span><span class="sxs-lookup"><span data-stu-id="677cd-179">This process may take up to 48 hours.</span></span> <span data-ttu-id="677cd-180">Al termine della convalida, lo stato del profilo rifletterà l' **approvazione** o l' **azione richiesta**.</span><span class="sxs-lookup"><span data-stu-id="677cd-180">Once validation has been completed, your profile status will reflect either **Approved** or **Action required**.</span></span> <span data-ttu-id="677cd-181">Se è **richiesta l'azione** , ripetere i passaggi precedenti fornendo le informazioni necessarie.</span><span class="sxs-lookup"><span data-stu-id="677cd-181">If **Action Required** , repeat the steps above providing the necessary information.</span></span> 

## <a name="create-your-tax-profile"></a><span data-ttu-id="677cd-182">Creare il profilo fiscale</span><span class="sxs-lookup"><span data-stu-id="677cd-182">Create your tax profile</span></span>

<span data-ttu-id="677cd-183">Utilizzare la seguente procedura per fornire a Microsoft le informazioni fiscali necessarie per l'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="677cd-183">Use the following procedure to provide Microsoft with the tax information required for your organization.</span></span> <span data-ttu-id="677cd-184">Le pagine di questa sezione sono dinamiche e variano in base al paese o all'area geografica.</span><span class="sxs-lookup"><span data-stu-id="677cd-184">The pages in this section are dynamic and will vary according to your country or region.</span></span> <span data-ttu-id="677cd-185">Se è necessario assistenza per identificare le informazioni fiscali corrette, contattare le fonti governative appropriate nel proprio paese.</span><span class="sxs-lookup"><span data-stu-id="677cd-185">If you need help with identifying the correct tax information, contact the appropriate government sources in your country.</span></span>

<span data-ttu-id="677cd-186">Per le società partner in America, se sono necessarie informazioni sul completamento dei moduli W8 o W9, i seguenti indirizzi indirizzano al sito di IRS:</span><span class="sxs-lookup"><span data-stu-id="677cd-186">For partner companies in the Americas, if you require information on completing the W8 or W9 forms, the following addresses take you to the IRS site:</span></span>

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> <span data-ttu-id="677cd-187">Immettere solo i dettagli della società.</span><span class="sxs-lookup"><span data-stu-id="677cd-187">Enter only details for your company.</span></span> <span data-ttu-id="677cd-188">Non immettere mai i dettagli personali.</span><span class="sxs-lookup"><span data-stu-id="677cd-188">Never enter personal details.</span></span>

1. <span data-ttu-id="677cd-189">Nella pagina **profilo business** completare i campi obbligatori e quindi fare clic su **Avanti**.</span><span class="sxs-lookup"><span data-stu-id="677cd-189">On the **Business Profile** page, complete the required fields and then select **Next**.</span></span> 

2. <span data-ttu-id="677cd-190">Nella pagina di **installazione** selezionare l'opzione che si applica alla società.</span><span class="sxs-lookup"><span data-stu-id="677cd-190">On the **Setup** page, select the option that applies to your company.</span></span>

   - <span data-ttu-id="677cd-191">Selezionare l'opzione a sinistra se la società è incorporata solo nel Stati Uniti o se il profilo è per un singolo utente.</span><span class="sxs-lookup"><span data-stu-id="677cd-191">Select the option on the left if your company is incorporated in the United States only, or if this profile is for an individual.</span></span>
   - <span data-ttu-id="677cd-192">Selezionare l'opzione a destra se la società è incorporata all'esterno del Stati Uniti, quindi selezionare il paese dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="677cd-192">Select the option on the right if your company is incorporated outside of the United States, and then select your country/region from the list.</span></span>

3. <span data-ttu-id="677cd-193">Selezionare **Avanti**.</span><span class="sxs-lookup"><span data-stu-id="677cd-193">Select **Next**.</span></span> 

4. <span data-ttu-id="677cd-194">Nella pagina **Tax status** immettere le informazioni necessarie e quindi fare clic su **Next (avanti** ).</span><span class="sxs-lookup"><span data-stu-id="677cd-194">On the **Tax status** page, enter the required information, and then select **Next**.</span></span> <span data-ttu-id="677cd-195">I campi in questa pagina variano in base al paese.</span><span class="sxs-lookup"><span data-stu-id="677cd-195">Fields on this page will vary by country.</span></span> <span data-ttu-id="677cd-196">dettagli.</span><span class="sxs-lookup"><span data-stu-id="677cd-196">your details.</span></span> 

5. <span data-ttu-id="677cd-197">Nella pagina **documentazione aggiuntiva** , i campi obbligatori e selezionare **Avanti**.</span><span class="sxs-lookup"><span data-stu-id="677cd-197">On the **Additional documentation** page, the required fields and select **Next**.</span></span> 

6. <span data-ttu-id="677cd-198">Selezionare **Browse (Sfoglia** ) per caricare i documenti richiesti dal paese o dall'area geografica.</span><span class="sxs-lookup"><span data-stu-id="677cd-198">Select **Browse** to upload any documents required by your country or region.</span></span> <span data-ttu-id="677cd-199">Quando viene visualizzato il nome del documento, selezionare **carica**.</span><span class="sxs-lookup"><span data-stu-id="677cd-199">When the document name is shown, select **Upload**.</span></span> 

7. <span data-ttu-id="677cd-200">Se è necessario rimuovere il documento, selezionare **Rimuovi**.</span><span class="sxs-lookup"><span data-stu-id="677cd-200">If you need to remove the document, select **Remove**.</span></span>

8. <span data-ttu-id="677cd-201">Per salvare e continuare, selezionare **fine**.</span><span class="sxs-lookup"><span data-stu-id="677cd-201">To save and continue, select **Finish**.</span></span>

9. <span data-ttu-id="677cd-202">Selezionare **conferma** nel messaggio popup.</span><span class="sxs-lookup"><span data-stu-id="677cd-202">Select **Confirm** on the pop-up message.</span></span> <span data-ttu-id="677cd-203">Verrà ripristinata la pagina di **configurazione dei pagamenti e delle imposte** .</span><span class="sxs-lookup"><span data-stu-id="677cd-203">You’ll be taken back to the **Payout and tax setup** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="677cd-204">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="677cd-204">Next steps</span></span>

- [<span data-ttu-id="677cd-205">Domande frequenti su proventi da incentivi e profilo fiscale</span><span class="sxs-lookup"><span data-stu-id="677cd-205">Incentives payout and tax profile FAQs</span></span>](incentives-payout-tax-profile-faqs.md)
