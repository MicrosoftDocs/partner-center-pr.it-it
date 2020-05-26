---
title: Connettore di co-selling per Salesforce CRM Partner Center
ms.topic: article
ms.date: 05/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Uso del connettore Salesforce CRM, ottenere i riferimenti da Microsoft
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: ''
ms.localizationpriority: medium
ms.openlocfilehash: ad39bdde92611066d0dd0c56d8b9133f4d9dcaa9
ms.sourcegitcommit: 97f1ff7386562cbb945bdfbcf15c85bc8303cac2
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/25/2020
ms.locfileid: "83825698"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="1233a-103">Co-selling Connector per Salesforce CRM-Panoramica</span><span class="sxs-lookup"><span data-stu-id="1233a-103">Co-sell connector for Salesforce CRM - overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="1233a-104">Ruoli appropriati</span><span class="sxs-lookup"><span data-stu-id="1233a-104">Appropriate roles</span></span>

- <span data-ttu-id="1233a-105">Amministratore delle segnalazioni</span><span class="sxs-lookup"><span data-stu-id="1233a-105">Referrals admin</span></span>
- <span data-ttu-id="1233a-106">Amministratore di sistema o verbi di sistema in CRM</span><span class="sxs-lookup"><span data-stu-id="1233a-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="1233a-107">Il connettore di co-selling del centro partner consente ai venditori di co-selling con Microsoft all'interno dei sistemi CRM.</span><span class="sxs-lookup"><span data-stu-id="1233a-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="1233a-108">Non dovranno essere sottoposti a training per usare il centro per i partner per gestire le offerte di co-selling.</span><span class="sxs-lookup"><span data-stu-id="1233a-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="1233a-109">Utilizzando i connettori di co-selling, sarà possibile creare un nuovo riferimento di co-selling per coinvolgere un venditore Microsoft, ricevere i riferimenti da Microsoft seller, accettare o rifiutare i riferimenti, modificare i dati relativi alle trattative, ad esempio il valore dell'offerta, la data di chiusura e così via, nonché ricevere eventuali aggiornamenti dai venditori Microsoft per le offerte di co-selling.</span><span class="sxs-lookup"><span data-stu-id="1233a-109">Using the Co-sell connectors, you will be able to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, closing date etc. as well as receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="1233a-110">Questa operazione può essere eseguita all'interno del CRM scelto piuttosto che nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="1233a-110">You can do all of this while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="1233a-111">La soluzione è basata sulla soluzione Microsoft Power automatizzate e usa le API del centro per i partner Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1233a-111">The solution is based on Microsoft Power Automate Solution and uses Microsoft Partner Center APIs.</span></span>


## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="1233a-112">Prima di installare-prerequisiti</span><span class="sxs-lookup"><span data-stu-id="1233a-112">Before you install - pre-requisites</span></span>

|<span data-ttu-id="1233a-113">**Argomenti**</span><span class="sxs-lookup"><span data-stu-id="1233a-113">**Topics**</span></span>   |<span data-ttu-id="1233a-114">**Dettagli**</span><span class="sxs-lookup"><span data-stu-id="1233a-114">**Details**</span></span>   |<span data-ttu-id="1233a-115">**Collegamenti**</span><span class="sxs-lookup"><span data-stu-id="1233a-115">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="1233a-116">ID Microsoft Partner Network</span><span class="sxs-lookup"><span data-stu-id="1233a-116">Microsoft Partner Network ID</span></span> |<span data-ttu-id="1233a-117">È necessario un ID MPN valido</span><span class="sxs-lookup"><span data-stu-id="1233a-117">You need a valid MPN ID</span></span>|<span data-ttu-id="1233a-118">Per aggiungere [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="1233a-118">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="1233a-119">Co-selling pronto</span><span class="sxs-lookup"><span data-stu-id="1233a-119">Co-sell ready</span></span>|<span data-ttu-id="1233a-120">La soluzione IP/servizi deve essere pronta per il co-selling.</span><span class="sxs-lookup"><span data-stu-id="1233a-120">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="1233a-121">Vendi con Microsoft</span><span class="sxs-lookup"><span data-stu-id="1233a-121">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="1233a-122">Account del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="1233a-122">Partner Center account</span></span>|<span data-ttu-id="1233a-123">L'ID MPN associato al tenant del centro per i partner deve corrispondere all'ID MPN associato alla soluzione di co-selling.</span><span class="sxs-lookup"><span data-stu-id="1233a-123">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="1233a-124">Prima di distribuire i connettori, verificare che sia possibile visualizzare i riferimenti di co-selling nel portale del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="1233a-124">Verify that you can see your co-sell referrals in Partner Center portal prior to deploying the connectors.</span></span>|[<span data-ttu-id="1233a-125">Gestire l'account</span><span class="sxs-lookup"><span data-stu-id="1233a-125">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="1233a-126">Ruoli utente del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="1233a-126">Partner Center user roles</span></span>|<span data-ttu-id="1233a-127">Il dipendente che installerà e userà i connettori deve essere un amministratore dei riferimenti</span><span class="sxs-lookup"><span data-stu-id="1233a-127">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="1233a-128">Assegnare autorizzazioni e ruoli utente</span><span class="sxs-lookup"><span data-stu-id="1233a-128">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="1233a-129">CRM Salesforce</span><span class="sxs-lookup"><span data-stu-id="1233a-129">Salesforce CRM</span></span>|<span data-ttu-id="1233a-130">Il ruolo utente CRM è amministratore sistema o sistema verbi</span><span class="sxs-lookup"><span data-stu-id="1233a-130">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="1233a-131">Assegnare i ruoli in Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="1233a-131">Assign roles in Dynamics 365</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="1233a-132">Power automatizzare l'account di flusso</span><span class="sxs-lookup"><span data-stu-id="1233a-132">Power Automate Flow Account</span></span>|<span data-ttu-id="1233a-133">Un account di [Power automatici](https://flow.microsoft.com) attivo per l'amministratore del sistema CRM o verbi di sistema.</span><span class="sxs-lookup"><span data-stu-id="1233a-133">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="1233a-134">L'utente deve accedere a [Power Automate](https://flow.microsoft.com) almeno una volta prima dell'installazione.</span><span class="sxs-lookup"><span data-stu-id="1233a-134">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="1233a-135">Installare la sincronizzazione dei riferimenti del centro per i partner per Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="1233a-135">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="1233a-136">Passare a [Power automatici](https://flow.microsoft.com) e selezionare **ambienti** nell'angolo superiore destro.</span><span class="sxs-lookup"><span data-stu-id="1233a-136">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="1233a-137">Vengono visualizzate le istanze di CRM disponibili.</span><span class="sxs-lookup"><span data-stu-id="1233a-137">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="1233a-138">Selezionare l'istanza di CRM appropriata dall'elenco a discesa nell'angolo in alto a destra.</span><span class="sxs-lookup"><span data-stu-id="1233a-138">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span> 

3. <span data-ttu-id="1233a-139">Selezionare **soluzioni** sulla barra di spostamento a sinistra.</span><span class="sxs-lookup"><span data-stu-id="1233a-139">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="1233a-140">Fare clic sul collegamento **Apri AppSource** nel menu in alto.</span><span class="sxs-lookup"><span data-stu-id="1233a-140">Click on the **Open AppSource** link on the top menu.</span></span>

![Apri AppSource](images/cosellconnectors/openappsource.png)

5. <span data-ttu-id="1233a-142">Cercare **connettori per i riferimenti del centro per i partner per Salesforce** nella schermata popup.</span><span class="sxs-lookup"><span data-stu-id="1233a-142">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

6. <span data-ttu-id="1233a-143">Fai clic sul pulsante **Get it Now (Ottieni ora** ) e **continua**.</span><span class="sxs-lookup"><span data-stu-id="1233a-143">Click the **Get it now** button and then **Continue**.</span></span> 

7. <span data-ttu-id="1233a-144">Verrà visualizzata la pagina in cui è possibile selezionare l'ambiente CRM (Dynamics 365) per installare l'applicazione.</span><span class="sxs-lookup"><span data-stu-id="1233a-144">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="1233a-145">Accettare i termini e le condizioni.</span><span class="sxs-lookup"><span data-stu-id="1233a-145">Agree to terms and conditions.</span></span> 

8. <span data-ttu-id="1233a-146">Si verrà quindi indirizzati alla pagina **Gestisci soluzioni** .</span><span class="sxs-lookup"><span data-stu-id="1233a-146">You are then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="1233a-147">Passare a "centro per i partner" usando i pulsanti freccia nella parte inferiore della pagina.</span><span class="sxs-lookup"><span data-stu-id="1233a-147">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="1233a-148">L' **installazione pianificata** verrà visualizzata accanto alla soluzione di riferimento del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="1233a-148">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="1233a-149">L'installazione può richiedere 10-15 minuti.</span><span class="sxs-lookup"><span data-stu-id="1233a-149">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="1233a-150">Al termine dell'installazione, tornare a [Power automatizzate](https://flow.microsoft.com) e selezionare **soluzioni** dall'area di spostamento a sinistra.</span><span class="sxs-lookup"><span data-stu-id="1233a-150">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="1233a-151">Si noti che la **sincronizzazione dei riferimenti del centro per i partner per Salesforce** è disponibile nell'elenco soluzioni.</span><span class="sxs-lookup"><span data-stu-id="1233a-151">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="1233a-152">Selezionare **la sincronizzazione dei riferimenti del centro per i partner per Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="1233a-152">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="1233a-153">Sono disponibili i flussi e le entità seguenti per l'automazione dell'energia elettrica:</span><span class="sxs-lookup"><span data-stu-id="1233a-153">The following Power Automate flows and entities are available:</span></span>

![DISPONGONO disponibili](images/cosellconnectors/dynamics-available-crms.png)

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="1233a-155">Procedura consigliata: testare prima di iniziare</span><span class="sxs-lookup"><span data-stu-id="1233a-155">Best Practice: Test before you go live</span></span>

<span data-ttu-id="1233a-156">Prima di installare, configurare e personalizzare la soluzione Power automatizzate nell'ambiente di produzione, assicurarsi di testare la soluzione in un'istanza di CRM di staging.</span><span class="sxs-lookup"><span data-stu-id="1233a-156">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="1233a-157">Installare la soluzione Microsoft Power automatizzate in un ambiente di gestione temporanea o in un'istanza di CRM.</span><span class="sxs-lookup"><span data-stu-id="1233a-157">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="1233a-158">Creare una copia della soluzione ed eseguire la configurazione e Power automatizzare le personalizzazioni dei flussi nell'ambiente di gestione temporanea.</span><span class="sxs-lookup"><span data-stu-id="1233a-158">Make a copy of the solution and perform your configuration and Power Automate flow customizations on the staging environment.</span></span>
- <span data-ttu-id="1233a-159">Testare la soluzione in un'istanza di staging/CRM.</span><span class="sxs-lookup"><span data-stu-id="1233a-159">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="1233a-160">In caso di esito positivo, importare come soluzione gestita nell'istanza di produzione.</span><span class="sxs-lookup"><span data-stu-id="1233a-160">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="1233a-161">Configurare la soluzione</span><span class="sxs-lookup"><span data-stu-id="1233a-161">Configure the solution</span></span>

1. <span data-ttu-id="1233a-162">Dopo aver installato la soluzione nell'istanza di CRM, tornare a [Power automatizzate](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="1233a-162">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="1233a-163">Dall'elenco a discesa **ambienti** nell'angolo superiore destro selezionare l'istanza di CRM in cui è stata installata la soluzione Power automatizzate.</span><span class="sxs-lookup"><span data-stu-id="1233a-163">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="1233a-164">Sarà necessario creare connessioni che associano i tre account utente:</span><span class="sxs-lookup"><span data-stu-id="1233a-164">You will need to create connections that associate the three user accounts:</span></span> 

- <span data-ttu-id="1233a-165">Utente del centro per i partner con credenziali di amministratore per i riferimenti</span><span class="sxs-lookup"><span data-stu-id="1233a-165">Partner Center user with referrals admin credentials</span></span> 
- <span data-ttu-id="1233a-166">Eventi del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="1233a-166">Partner Center Events</span></span>
- <span data-ttu-id="1233a-167">L'amministratore di CRM con la funzionalità Power automatizza i flussi nella soluzione.</span><span class="sxs-lookup"><span data-stu-id="1233a-167">CRM admin with the Power Automate flows in the solution.</span></span> 

    <span data-ttu-id="1233a-168">a.</span><span class="sxs-lookup"><span data-stu-id="1233a-168">a.</span></span> <span data-ttu-id="1233a-169">Selezionare **Connections (connessioni** ) dalla barra di spostamento a sinistra e selezionare la soluzione "Partner Center referrals" dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="1233a-169">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>
    <span data-ttu-id="1233a-170">b.</span><span class="sxs-lookup"><span data-stu-id="1233a-170">b.</span></span> <span data-ttu-id="1233a-171">Creare una connessione facendo clic su **Crea una connessione**.</span><span class="sxs-lookup"><span data-stu-id="1233a-171">Create a connection by clicking **Create a connection**.</span></span> 

    ![Creare la connessione](images/cosellconnectors/createconnection.png)

    <span data-ttu-id="1233a-173">c.</span><span class="sxs-lookup"><span data-stu-id="1233a-173">c.</span></span> <span data-ttu-id="1233a-174">Cercare i riferimenti per il centro per i **partner (anteprima)** nella barra di ricerca nell'angolo superiore destro.</span><span class="sxs-lookup"><span data-stu-id="1233a-174">Search for **Partner Center Referrals (preview)** in the search bar on the top right corner.</span></span>
    <span data-ttu-id="1233a-175">d.</span><span class="sxs-lookup"><span data-stu-id="1233a-175">d.</span></span> <span data-ttu-id="1233a-176">Creare una connessione per l'utente del centro per i partner con il ruolo delle credenziali di amministratore dei riferimenti. e.</span><span class="sxs-lookup"><span data-stu-id="1233a-176">Create a connection for your Partner Center user with the credentials role of Referrals admin. e.</span></span> <span data-ttu-id="1233a-177">Successivamente, creare una connessione per gli eventi del centro partner per l'utente del centro per i partner con le credenziali di amministratore dei riferimenti. f.</span><span class="sxs-lookup"><span data-stu-id="1233a-177">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin. f.</span></span> <span data-ttu-id="1233a-178">Creare una connessione per Common Data Service (ambiente corrente) per l'utente amministratore CRM.</span><span class="sxs-lookup"><span data-stu-id="1233a-178">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

4. <span data-ttu-id="1233a-179">Per associare i flussi di automazione dell'alimentazione con le connessioni, modificare ognuno dei flussi di automazione dell'alimentazione per connettersi a Common Data Service e ai riferimenti del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="1233a-179">To associate the Power Automate flows with the connections, edit each of the Power Automate flows to connect to Common Data Service and Partner Center Referrals.</span></span> <span data-ttu-id="1233a-180">Salvare le modifiche.</span><span class="sxs-lookup"><span data-stu-id="1233a-180">Save the changes.</span></span>

5. <span data-ttu-id="1233a-181">**Attivare** i flussi di automazione dell'alimentazione.</span><span class="sxs-lookup"><span data-stu-id="1233a-181">**Turn on** the the Power Automate flows.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1233a-182">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="1233a-182">Next steps</span></span>

- [<span data-ttu-id="1233a-183">Usare i webhook per ottenere gli eventi di modifica delle risorse</span><span class="sxs-lookup"><span data-stu-id="1233a-183">Use Webhooks to get resource change events</span></span>](referral-connector-webhooks.md)

- [<span data-ttu-id="1233a-184">Altre informazioni sulla piattaforma Microsoft Power automatizzate?</span><span class="sxs-lookup"><span data-stu-id="1233a-184">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/power-automate/)

- [<span data-ttu-id="1233a-185">Gestire lead</span><span class="sxs-lookup"><span data-stu-id="1233a-185">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="1233a-186">Gestire opportunità di co-selling</span><span class="sxs-lookup"><span data-stu-id="1233a-186">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
