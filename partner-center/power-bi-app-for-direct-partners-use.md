---
title: Usare Partner Center Analytics per Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come visualizzare i dati aziendali usando app Analisi del Centro per i Partner per Power BI (per i partner diretti nel programma Cloud Solution Provider (CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 95eb018a3284d2de98c0ce6a9cd0ce6299d5571a
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/24/2021
ms.locfileid: "112564982"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="49508-103">Visualizzare i dati aziendali con l'app Partner Center Analytics per Microsoft Power BI</span><span class="sxs-lookup"><span data-stu-id="49508-103">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>



<span data-ttu-id="49508-104">**Ruoli appropriati:** Amministratore globale | Amministratore di gestione utenti | Agente di vendita | Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="49508-104">**Appropriate roles**: Global admin | User management admin | Sales agent | Admin agent</span></span>

## <a name="view-your-business-data"></a><span data-ttu-id="49508-105">Visualizzare i dati aziendali</span><span class="sxs-lookup"><span data-stu-id="49508-105">View your business data</span></span>

<span data-ttu-id="49508-106">Ottenere una rappresentazione visiva dei dati aziendali con l'app Partner Center Analytics per Microsoft Power BI, tra cui:</span><span class="sxs-lookup"><span data-stu-id="49508-106">Get a visual representation of your business data with the Partner Center Analytics app for Microsoft Power BI, including:</span></span>

- <span data-ttu-id="49508-107">Crescita della base clienti, delle sottoscrizioni e delle licenze</span><span class="sxs-lookup"><span data-stu-id="49508-107">Growth of your customer base, subscriptions, and licenses</span></span>

- <span data-ttu-id="49508-108">L'utilizzo dei prodotti Office 365, Microsoft Dynamics e Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="49508-108">Usage of Office 365, Microsoft Dynamics, and Microsoft Azure products</span></span>

- <span data-ttu-id="49508-109">Le unità di consumo giornaliere per ogni risorsa a consumo negli abbonamenti di Azure per gli ultimi 60 giorni</span><span class="sxs-lookup"><span data-stu-id="49508-109">Daily consumption units for each metered resource in each Azure subscription for the last 60 days</span></span>

- <span data-ttu-id="49508-110">Costo stimato (in base alla scheda tariffa più recente)</span><span class="sxs-lookup"><span data-stu-id="49508-110">Estimated cost (based on latest rate card)</span></span>

- <span data-ttu-id="49508-111">Possibilità di esportare set di dati e creare report personalizzati, incluso per cliente.</span><span class="sxs-lookup"><span data-stu-id="49508-111">Ability to export datasets and create custom reports, including per customer.</span></span>

### <a name="about-the-partner-center-analytics-app-preview-release"></a><span data-ttu-id="49508-112">Informazioni sulla versione Partner Center di anteprima dell'app Di Analytics</span><span class="sxs-lookup"><span data-stu-id="49508-112">About the Partner Center Analytics app preview release</span></span>

- <span data-ttu-id="49508-113">Questa app è solo per i partner diretti nel programma Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="49508-113">This app is for direct partners in the Cloud Solution Provider (CSP) program only.</span></span> <span data-ttu-id="49508-114">Altri partner in CSP (rivenditori indiretti, ad esempio) non saranno in grado di accedere.</span><span class="sxs-lookup"><span data-stu-id="49508-114">Other partners in CSP (indirect resellers, for example) will not be able to sign in.</span></span>

- <span data-ttu-id="49508-115">I costi stimati sono dati di fatturazione/fattura pre-imposta e non sono legalmente vincolanti.</span><span class="sxs-lookup"><span data-stu-id="49508-115">Any estimated costs are pre-tax billing / invoice data, and are not legally binding.</span></span> <span data-ttu-id="49508-116">I costi stimati devono essere usati solo per le informazioni dettagliate sui dati.</span><span class="sxs-lookup"><span data-stu-id="49508-116">Estimated costs are meant to be used for data insights only.</span></span>

- <span data-ttu-id="49508-117">Le informazioni sui clienti si basano sulle sottoscrizioni.</span><span class="sxs-lookup"><span data-stu-id="49508-117">Customer information is based on subscriptions.</span></span> <span data-ttu-id="49508-118">Tutti i clienti per cui sono stati creati di recente gli account, ma che non hanno ancora sottoscrizioni, non vengono inclusi nei conteggi.</span><span class="sxs-lookup"><span data-stu-id="49508-118">Any customers that you've recently created accounts for, but who don't yet have subscriptions, aren't included in counts.</span></span>

- <span data-ttu-id="49508-119">Il costo stimato si basa sulla scheda tariffa più recente, basata sui prezzi CSP.</span><span class="sxs-lookup"><span data-stu-id="49508-119">Estimated cost is based on latest rate card, which is based on CSP pricing.</span></span>

- <span data-ttu-id="49508-120">I giorni sono giorni di calendario.</span><span class="sxs-lookup"><span data-stu-id="49508-120">Days are calendar days.</span></span>

### <a name="business-insights-report"></a><span data-ttu-id="49508-121">Approfondimento azienda report</span><span class="sxs-lookup"><span data-stu-id="49508-121">Business Insights report</span></span>

- <span data-ttu-id="49508-122">**Tenant dei clienti:** numero di tenant Azure Active Directory (Azure AD) distinti dei clienti che hanno acquistato sottoscrizioni</span><span class="sxs-lookup"><span data-stu-id="49508-122">**Customer tenants**: Number of distinct Azure Active Directory (Azure AD) tenants of customers that have purchased subscriptions</span></span>

- <span data-ttu-id="49508-123">**Nuovo (ultimi 30 giorni):** nuovi clienti che acquistano almeno una sottoscrizione negli ultimi 30 giorni</span><span class="sxs-lookup"><span data-stu-id="49508-123">**New (last 30 days)**: New customers purchasing at least one subscription in last 30 days</span></span>

- <span data-ttu-id="49508-124">**Varianza (ultimi 30 giorni):** clienti senza sottoscrizioni "attive", "in stato di tolleranza" o "disabilitate"</span><span class="sxs-lookup"><span data-stu-id="49508-124">**Churn (last 30 days)**: Customers without any “active", “in grace" or “disabled" subscriptions</span></span>

- <span data-ttu-id="49508-125">**Nuovo (ultime 24 ore):** nuovi clienti che acquistano almeno una sottoscrizione nelle ultime 24 ore</span><span class="sxs-lookup"><span data-stu-id="49508-125">**New (last 24 hours)**: New customers purchasing at least one subscription in last 24 hours</span></span>

- <span data-ttu-id="49508-126">**Costo mensile stimato negli ultimi 12** mesi: tendenza mensile dell'importo stimato in dollari della fattura pre-imposta aggregato mensilmente nel periodo degli ultimi 12 mesi</span><span class="sxs-lookup"><span data-stu-id="49508-126">**Estimated monthly cost over last 12 months**: Month over month trend of estimated pre-tax invoice dollar amount aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="49508-127">**Costo stimato per prodotto negli ultimi 12** mesi: prodotti venduti ordinati in base all'importo stimato in dollari della fattura pre-imposta aggregati nel periodo degli ultimi 12 mesi.</span><span class="sxs-lookup"><span data-stu-id="49508-127">**Estimated cost by product over last 12 months**: Products sold sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="49508-128">Questo stato indica i principali prodotti che hanno prodotto la maggior parte dei ricavi.</span><span class="sxs-lookup"><span data-stu-id="49508-128">This status indicates top products bringing most revenue.</span></span>

- <span data-ttu-id="49508-129">**Clienti negli ultimi 12 mesi:** tendenza mese su mese dei nuovi clienti e varianza dei clienti aggregati mensilmente nel periodo degli ultimi 12 mesi</span><span class="sxs-lookup"><span data-stu-id="49508-129">**Customers over last 12 months**: Month over month trend of new customers and churn customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="49508-130">**Costo stimato per cliente negli ultimi 12** mesi: clienti ordinati in base all'importo stimato in dollari della fattura pre-imposta aggregati nel periodo degli ultimi 12 mesi.</span><span class="sxs-lookup"><span data-stu-id="49508-130">**Estimated cost by customer over last 12 months**: Customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="49508-131">Questo stato indica che i clienti principali hanno la maggior parte dei ricavi.</span><span class="sxs-lookup"><span data-stu-id="49508-131">This status indicates top customers bringing most revenue.</span></span>

- <span data-ttu-id="49508-132">**Conteggio clienti per prodotto:** prodotti venduti ordinati in base ai clienti associati.</span><span class="sxs-lookup"><span data-stu-id="49508-132">**Customer count by product**: Products sold sorted by associated customers.</span></span> <span data-ttu-id="49508-133">Questo stato indica i prodotti più venduti alla maggior parte dei clienti.</span><span class="sxs-lookup"><span data-stu-id="49508-133">This status indicates top products sold to most customers.</span></span>

### <a name="subscription-insights-report"></a><span data-ttu-id="49508-134">Report informazioni dettagliate sulla sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="49508-134">Subscription Insights report</span></span>

- <span data-ttu-id="49508-135">**Stato sottoscrizione**:</span><span class="sxs-lookup"><span data-stu-id="49508-135">**Subscription status**:</span></span>

- <span data-ttu-id="49508-136">Attivo: sottoscrizioni appartenenti allo stato "attivo" o "in stato di tolleranza"</span><span class="sxs-lookup"><span data-stu-id="49508-136">Active: Subscriptions belonging to either “active" or “in grace" state</span></span>

  - <span data-ttu-id="49508-137">Sospeso: sottoscrizioni appartenenti allo stato "disabilitato"</span><span class="sxs-lookup"><span data-stu-id="49508-137">Suspended: Subscriptions belonging to “disabled" state</span></span>

  - <span data-ttu-id="49508-138">De-provisioning: sottoscrizioni appartenenti allo stato "de-provisioning" o "scaduto"</span><span class="sxs-lookup"><span data-stu-id="49508-138">De-provisioned: Subscriptions belonging to “de-provisioned" or “expired" status</span></span>

- <span data-ttu-id="49508-139">**Stato di scadenza:**</span><span class="sxs-lookup"><span data-stu-id="49508-139">**Expiry status**:</span></span>

  - <span data-ttu-id="49508-140">Scaduto: sottoscrizioni già scadute (in cui la data di fine della sottoscrizione è passata)</span><span class="sxs-lookup"><span data-stu-id="49508-140">Expired: Subscriptions that have already expired (where subscription end date is in past)</span></span>

  - <span data-ttu-id="49508-141">Scadenza dopo 30 giorni: sottoscrizioni che scadranno dopo 30 giorni (in cui la data di fine della sottoscrizione è successiva ai 30 giorni successivi)</span><span class="sxs-lookup"><span data-stu-id="49508-141">Expiring after 30 days: Subscriptions that will expire after 30 days (where subscription end date is after next 30 days)</span></span>

  - <span data-ttu-id="49508-142">Scadenza tra 30 giorni: sottoscrizioni che scadranno entro i 30 giorni successivi (dove la data di fine della sottoscrizione è compresa tra oggi e i 30 giorni successivi)</span><span class="sxs-lookup"><span data-stu-id="49508-142">Expiring in 30 days: Subscriptions that will expire within next 30 days (where subscription end date is between today and next 30 days)</span></span>

- <span data-ttu-id="49508-143">**Totale sottoscrizioni:** sottoscrizioni con stato "attivo", "in stato di tolleranza" o "disabilitato"</span><span class="sxs-lookup"><span data-stu-id="49508-143">**Total subscriptions**: Subscriptions in “active," “in grace" or “disabled" status</span></span>

- <span data-ttu-id="49508-144">**Nuovo (ultimi 30 giorni):** nuove sottoscrizioni acquistate dai clienti negli ultimi 30 giorni</span><span class="sxs-lookup"><span data-stu-id="49508-144">**New (last 30 days)**: New subscriptions purchased by customers within last 30 days</span></span>

- <span data-ttu-id="49508-145">**Nuovo (ultime 24 ore):** nuove sottoscrizioni acquistate dai clienti nelle ultime 24 ore</span><span class="sxs-lookup"><span data-stu-id="49508-145">**New (last 24 hours)**: New subscriptions purchased by customers within last 24 hours</span></span>

- <span data-ttu-id="49508-146">**Scadenza tra 30 giorni:** sottoscrizioni che scadranno entro i prossimi 30 giorni</span><span class="sxs-lookup"><span data-stu-id="49508-146">**Expiring in 30 days**: Subscriptions that will expire within next 30 days</span></span>

- <span data-ttu-id="49508-147">**Varianza (ultimi 30 giorni):** sottoscrizioni di cui è stato effettuato il de-provisioning o che sono state sospese (disabilitate) negli ultimi 30 giorni</span><span class="sxs-lookup"><span data-stu-id="49508-147">**Churn (last 30 days)**: Subscriptions that have been de-provisioned or suspended (disabled) within last 30 days</span></span>

- <span data-ttu-id="49508-148">**Distribuzione in base ai tipi di sottoscrizione:**% distribuzione delle sottoscrizioni totali in base alla licenza e al tipo di sottoscrizione basata sull'utilizzo</span><span class="sxs-lookup"><span data-stu-id="49508-148">**Distribution by subscription types**: % distribution of total subscriptions by License based and usage-based subscription type</span></span>

- <span data-ttu-id="49508-149">**Conteggio sottoscrizioni attive per prodotto:** prodotti venduti ordinati in base al numero di sottoscrizioni attive</span><span class="sxs-lookup"><span data-stu-id="49508-149">**Active subscription count by product**: Products sold sorted by active subscriptions count</span></span>

- <span data-ttu-id="49508-150">**Sottoscrizioni negli ultimi 12 mesi:** tendenza mensile delle nuove sottoscrizioni e delle sottoscrizioni di varianza aggregate mensilmente nel periodo degli ultimi 12 mesi</span><span class="sxs-lookup"><span data-stu-id="49508-150">**Subscriptions over last 12 months**: Month over month trend of new subscriptions and churn subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="49508-151">**Dettagli della sottoscrizione del** cliente: visualizzazione dettagliata di clienti, sottoscrizioni e offerte</span><span class="sxs-lookup"><span data-stu-id="49508-151">**Customer subscription details**: Detailed view of the customers, subscriptions, and offers</span></span>

### <a name="license-insights-report"></a><span data-ttu-id="49508-152">Report di Informazioni dettagliate sulle licenze:</span><span class="sxs-lookup"><span data-stu-id="49508-152">License Insights report:</span></span>

- <span data-ttu-id="49508-153">**Totale licenze:** numero totale di licenze aggregate in tutte le sottoscrizioni basate su licenza</span><span class="sxs-lookup"><span data-stu-id="49508-153">**Total licenses**: Total number of licenses aggregated across all license-based subscriptions</span></span>

- <span data-ttu-id="49508-154">**Nuovo (ultimi 30 giorni):** aggiunta della licenza negli ultimi 30 giorni</span><span class="sxs-lookup"><span data-stu-id="49508-154">**New (last 30 days)**: License addition within last 30 days</span></span>

- <span data-ttu-id="49508-155">**Varianza (ultimi 30 giorni):** riduzione delle licenze negli ultimi 30 giorni</span><span class="sxs-lookup"><span data-stu-id="49508-155">**Churn (last 30 days)**: License reduction within last 30 days</span></span>

- <span data-ttu-id="49508-156">**Nuovo (ultime 24 ore):** aggiunta della licenza nelle ultime 24 ore</span><span class="sxs-lookup"><span data-stu-id="49508-156">**New (last 24 hours)**: License addition within last 24 hours</span></span>

- <span data-ttu-id="49508-157">**Licenze negli ultimi 90 giorni:** tendenza mensile delle aggiunte e delle riduzioni delle licenze aggregate mensilmente nel periodo degli ultimi 90 giorni</span><span class="sxs-lookup"><span data-stu-id="49508-157">**Licenses over last 90 days**: Month over month trend of license additions and reductions aggregated monthly over the period of last 90 days</span></span>

- <span data-ttu-id="49508-158">**Numero di licenze attive per prodotto:** prodotti venduti ordinati in base al numero di licenze attive</span><span class="sxs-lookup"><span data-stu-id="49508-158">**Active license count by product**: Products sold sorted by active license count</span></span>

- <span data-ttu-id="49508-159">**Numero di licenze attive per cliente:** clienti ordinati in base al numero di licenze attive</span><span class="sxs-lookup"><span data-stu-id="49508-159">**Active license count by customer**: Customers sorted by active license count</span></span>

- <span data-ttu-id="49508-160">**Dettagli dell'evento** di licenza del cliente negli ultimi 90 giorni: visualizzazione dettagliata dei clienti, delle sottoscrizioni e degli eventi di sottoscrizione, tra cui la data dell'evento, il nome dell'evento, la quantità e la modifica della quantità.</span><span class="sxs-lookup"><span data-stu-id="49508-160">**Customer license event details over last 90 days**: Detailed view of the customers, subscriptions, and subscription events including event date, event name, quantity, and change in quantity.</span></span>

### <a name="licenses-usage-report"></a><span data-ttu-id="49508-161">Report utilizzo licenze:</span><span class="sxs-lookup"><span data-stu-id="49508-161">Licenses Usage report:</span></span>

- <span data-ttu-id="49508-162">**Licenze assegnate per prodotto:** prodotti venduti ordinati in base al numero di assegnazioni di licenze</span><span class="sxs-lookup"><span data-stu-id="49508-162">**Licenses assigned by product**: Products sold sorted by license assignment count</span></span>

- <span data-ttu-id="49508-163">**Licenze in uso per prodotto:** prodotti venduti ordinati in base al numero di utilizzo delle licenze</span><span class="sxs-lookup"><span data-stu-id="49508-163">**Licenses in use by product**: Products sold sorted by license usage count</span></span>

- <span data-ttu-id="49508-164">**Distribuzione delle licenze assegnate dai clienti:**% distribuzione del totale dei clienti suddivisi in bucket di intervallo del 20% in base alla % di assegnazione delle licenze</span><span class="sxs-lookup"><span data-stu-id="49508-164">**Customer distribution of licenses assigned**: % distribution of total customers broken in buckets of 20% range by license assignment %</span></span>

- <span data-ttu-id="49508-165">**Distribuzione delle licenze in uso da** parte del cliente: % distribuzione del totale dei clienti suddivisi in bucket di intervallo del 20% in base alla % di utilizzo delle licenze</span><span class="sxs-lookup"><span data-stu-id="49508-165">**Customer distribution of licenses in use**: % distribution of total customers broken in buckets of 20% range by license usage %</span></span>

- <span data-ttu-id="49508-166">**Licenze assegnate dal cliente:** visualizzazione dettagliata delle licenze vendute e delle licenze assegnate da clienti e prodotti</span><span class="sxs-lookup"><span data-stu-id="49508-166">**Licenses assigned by customer**: Detailed view of licenses sold and licenses assigned by customers and products</span></span>

- <span data-ttu-id="49508-167">**Licenze in uso dal cliente:** visualizzazione dettagliata delle licenze vendute e delle licenze in uso da clienti e prodotti</span><span class="sxs-lookup"><span data-stu-id="49508-167">**Licenses in use by customer**: Detailed view of licenses sold and licenses in use by customers and products</span></span>

### <a name="azure-insights-report"></a><span data-ttu-id="49508-168">Report di Azure Insights:</span><span class="sxs-lookup"><span data-stu-id="49508-168">Azure Insights report:</span></span>

- <span data-ttu-id="49508-169">Clienti basati sull'utilizzo negli ultimi **12** mesi: tendenza mensile dei nuovi clienti basati sull'utilizzo e dei clienti basati sull'utilizzo variati aggregati mensilmente nel periodo degli ultimi 12 mesi</span><span class="sxs-lookup"><span data-stu-id="49508-169">**Usage-based customers over last 12 months**: Month over month trend of new usage-based customers and churned usage-based customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="49508-170">Sottoscrizioni basate sull'utilizzo negli ultimi **12** mesi: tendenza mensile delle nuove sottoscrizioni basate sull'utilizzo e delle sottoscrizioni basate sull'utilizzo variate aggregate mensilmente nel periodo degli ultimi 12 mesi</span><span class="sxs-lookup"><span data-stu-id="49508-170">**Usage-based subscriptions over last 12 months**: Month over month trend of new usage-based subscriptions and churned usage-based subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="49508-171">Costo stimato di utilizzo per cliente negli ultimi **60** giorni: clienti basati sull'utilizzo ordinati in base all'importo stimato in dollari della fattura pre-imposta aggregati nel periodo degli ultimi 60 giorni.</span><span class="sxs-lookup"><span data-stu-id="49508-171">**Estimated cost of usage by customer over last 60 days**: Usage-based customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span> <span data-ttu-id="49508-172">Questo stato indica che i principali clienti basati sull'utilizzo hanno portato la maggior parte dei ricavi</span><span class="sxs-lookup"><span data-stu-id="49508-172">This status indicates top usage-based customers bringing most revenue</span></span>

- <span data-ttu-id="49508-173">Costo stimato di utilizzo per categoria negli ultimi **60** giorni: categorie del contatore delle sottoscrizioni basate sull'utilizzo ordinate in base all'importo stimato in dollari della fattura pre-imposta aggregato nel periodo degli ultimi 60 giorni.</span><span class="sxs-lookup"><span data-stu-id="49508-173">**Estimated cost of usage by category over last 60 days**: Meter categories of usage-based subscriptions sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="49508-174">Costo stimato di utilizzo per sottoscrizione negli ultimi **60** giorni: sottoscrizioni basate sull'utilizzo in base all'importo stimato in dollari della fattura pre-imposta aggregato nel periodo degli ultimi 60 giorni.</span><span class="sxs-lookup"><span data-stu-id="49508-174">**Estimated cost of usage by subscription over last 60 days**: Usage-based subscriptions by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="49508-175">**Costo di utilizzo stimato dal cliente in** base al budget di spesa: i clienti ordinati in base alla percentuale del budget di spesa corrente che supera la soglia (100%).</span><span class="sxs-lookup"><span data-stu-id="49508-175">**Customer estimated usage cost by spending budget**: Customers sorted by percentage of their current usage spending budget exceeding threshold (100%).</span></span>

### <a name="azure-resource-usage-report"></a><span data-ttu-id="49508-176">Report Utilizzo risorse di Azure:</span><span class="sxs-lookup"><span data-stu-id="49508-176">Azure Resource Usage report:</span></span>

- <span data-ttu-id="49508-177">**Utilizzo delle risorse di Azure** per giorno per il periodo selezionato: unità di consumo giornaliere per ogni risorsa a consumo in ogni sottoscrizione basata sull'utilizzo per il periodo selezionato negli ultimi 60 giorni.</span><span class="sxs-lookup"><span data-stu-id="49508-177">**Usage of Azure resources by day for selected period**: Daily consumption units for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span>

- <span data-ttu-id="49508-178">**Costo di utilizzo stimato** delle risorse di Azure per il periodo selezionato: costo stimato in base alla tariffa più recente per ogni risorsa a consumo in ogni sottoscrizione basata sull'utilizzo per il periodo selezionato negli ultimi 60 giorni.</span><span class="sxs-lookup"><span data-stu-id="49508-178">**Estimated usage cost of Azure resources for selected period**: Estimated cost based on latest rate card for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="49508-179">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="49508-179">Next steps</span></span>

- [<span data-ttu-id="49508-180">Partner Center Di Analytics per Power BI'app</span><span class="sxs-lookup"><span data-stu-id="49508-180">Partner Center Analytics for Power BI app overview</span></span>](power-bi-app-for-direct-partners.md)

- [<span data-ttu-id="49508-181">Installare e visualizzare in anteprima l'app Analisi del Centro per i Partner per Microsoft Power BI</span><span class="sxs-lookup"><span data-stu-id="49508-181">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-install.md)
