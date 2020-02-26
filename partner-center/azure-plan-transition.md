---
title: Transizioni dei clienti al piano di Azure | Centro per i partner
ms.topic: article
ms.date: 11/25/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Scopri come spostare i clienti con facilità nel piano di Azure.
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: high
ms.openlocfilehash: d9a283242fb911537004719fd62a58478c511565
ms.sourcegitcommit: c3de2c04d761314116b876ffdd4b2c79641007c1
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 02/24/2020
ms.locfileid: "77567237"
---
# <a name="transition-your-customers-to-azure-plan"></a>Eseguire la transizione dei clienti al piano di Azure

**Ruoli appropriati**

- Agente amministratore
- Amministratore fatturazione
- Amministratore globale
- Agente di supporto tecnico
- Agente di vendita
- Amministratore gestione utenti

I provider indiretti e i partner di fatturazione diretti possono passare alla nuova esperienza commerciale disponibile nel programma Microsoft Cloud Solution Provider (CSP) per Azure. I rivenditori indiretti dovranno passare attraverso i loro provider indiretti. I clienti avranno una soluzione semplificata per l'acquisto di servizi cloud dai partner, dai venditori Microsoft o direttamente sul Web.

La funzionalità di transizione è destinata solo ai clienti che passano alla nuova esperienza commerciale per Azure e che hanno firmato il Contratto per clienti Microsoft e non per altre offerte in CSP, come Office 365 o Dynamics 365.

## <a name="available-azure-services-in-azure-csp"></a>Servizi di Azure disponibili in Azure CSP

Questa sezione illustra i servizi di Azure disponibili e non disponibili nel programma Azure Cloud Solution Provider (CSP). Descrive anche la disponibilità dei servizi nei cloud nazionali [Microsoft Azure Germania](https://azure.microsoft.com/overview/clouds/germany/) e [Microsoft Azure per enti pubblici](https://azure.microsoft.com/overview/clouds/government/).

>[!Note]
>[Azure Cina]( https://www.azure.cn/) non è disponibile nel programma Azure CSP.

### <a name="global-cloud"></a>Cloud globale 

Tutti i servizi basati sul modello di Azure Resource Manager sono disponibili nel programma CSP.  I servizi non basati su Azure Resource Manager non sono disponibili nel programma CSP.  

### <a name="csp-specific-service-configurations"></a>Configurazioni di servizio specifiche di CSP

Per i servizi seguenti sono necessarie configurazioni speciali in CSP:

- [StorSimple](https://docs.microsoft.com/azure/storsimple/storsimple-partner-csp-overview)

- [Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-csp)

- [Key Vault](https://azurecsp.blob.core.windows.net/files/key-vault-in-csp.docx) 

- [Azure Time Series Insights](https://azure.microsoft.com/services/time-series-insights/): solo gli utenti del tenant del cliente possono accedere ai dati contenuti nell'ambiente Time Series Insights specifico. Per impostazione predefinita, i partner possono gestire l'ambiente Time Series Insights del cliente. Tuttavia, se devono accedere ai dati contenuti in tale ambiente, devono essere aggiunti al tenant del cliente. 

### <a name="visual-studio-marketplace"></a>Visual Studio Marketplace

Puoi ora acquistare gli articoli elencati di seguito da Visual Studio Marketplace, ad eccezione delle estensioni di terze parti.

- [Azure DevOps](https://www.visualstudio.com/team-services/) 

- [Sottoscrizioni di Visual Studio](https://www.visualstudio.com/subscriptions/)

- [Formazione Xamarin University](https://marketplace.visualstudio.com/items?itemName=ms.xamarin-university)

Per aiutarti a usare questi prodotti, abbiamo creato video e documentazione sulle [procedure per configurare, acquistare e gestire Azure DevOps](https://docs.microsoft.com/vsts/billing/csp/set-up-csp-customer) in CSP.

### <a name="azure-marketplace-items-in-azure-csp"></a>Articoli di Azure Marketplace in Azure CSP

Non tutti gli articoli di Azure Marketplace sono attualmente disponibili nelle sottoscrizioni di Azure CSP.

- Servizi di Azure basati su Microsoft: questi servizi sono disponibili. Rivedi la tabella e i commenti precedenti.

- Articoli Bring Your Own License (BYOL): questi articoli sono disponibili. Nella [pagina relativa ai prodotti BYOL di Azure Marketplace](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) è disponibile un elenco completo degli articoli di Azure Marketplace con capacità BYOL.

- Articoli di Azure Marketplace di terze parti con pagamento in base al consumo: questi articoli sono disponibili se il provider li ha pubblicati nel canale CSP. Per altre informazioni, vedi [Vendere sottoscrizioni di prodotti di Azure Marketplace](https://aka.ms/marketplaceincsp).   

- Citrix XenApp Essentials: i partner possono acquistare XenApp Essentials per i clienti in CSP. Per altre informazioni, vedi il blog di Citrix seguente: [XenApp Essentials now available through Microsoft Cloud Solution Provider Channel](https://www.citrix.com/blogs/2018/02/01/xenapp-essentials-now-available-through-microsoft-cloud-solution-provider-channel/) (XenApp Essentials ora disponibile tramite il canale Microsoft Cloud Solution Provider).

### <a name="national-clouds"></a>Cloud nazionali 
La tabella seguente contiene un elenco regolarmente aggiornato dei prodotti, dei servizi e delle funzionalità proprietari di Azure disponibili per CSP nei cloud nazionali. 

| Prodotto, servizio o funzionalità di Azure | Enti pubblici Stati Uniti | Germania |
| ------ | :-----------: | :-----------: |
|  **Compute**  |    |    |
|  Macchine virtuali  |  X  |  X  |
|  Servizi cloud  |    |    |
|  Set di scalabilità di macchine virtuali  |  X  |  X  |
|  Funzioni  |    |    |
|  Servizio Azure Container  |    |    |
|  **Funzionalità di rete**  |    |    |
|  Azure DNS  |    |    |
|  Rete di distribuzione dei contenuti  |    |    |
|  Gestione traffico  |    |    |
|  ExpressRoute  |  X  |  X  |
|  Rete virtuale  |  X  |  X  |
|  Bilanciamento del carico  |  X  |  X  |
|  Gateway VPN  |  X  |  X  |
|  Gateway applicazione  |  X  |  X  |
|  Network Watcher  |  X  |  X  |
|  **Archiviazione**  |    |    |
|  Archiviazione:  |  X  |  X  |
|  Backup  |  X  |  X  |
|  StorSimple  |    |  X  |
|  Site Recovery  |  X  |  X  |
|  Data Lake Store  |    |    |
|  Managed Disks  |  X  |  X  |
|  **Web e dispositivi mobili**  |    |    |
|  Servizio app  |  X  |  X  |
|  Servizio app in Linux  |    |  X  |
|  Gestione API  |  X  |    |
|  Rete di distribuzione dei contenuti  |    |    |
|  Servizi multimediali  |  X  |  X  |
|  Hub di notifica  |  X  |  X  |
|  Ricerca di Azure  |    |    |
|  Funzionalità App per la logica di Servizio app di Azure  |    |    |
|  **Contenitori**  |    |    |
|  Servizio app  |  X  |  X  |
|  Servizio app in Linux  |    |  X  |
|  Batch  |  X  |  X  |
|  Registro Container  |    |    |
|  Istanze di Container  |    |    |
|  Service Fabric  |  X  |  X  |
|  Servizio Container  |    |    |
|  **Database**  |    |    |
|  Database di SQL Server  |  X  |  X  |
|  Azure Cosmos DB  |  X  |  X  |
|  SQL Data Warehouse  |  X  |  X  |
|  Cache Redis  |  X  |  X  |
|  SQL Server Stretch Database  |  X  |  X  |
|  Database di Azure per MySQL  |    |    |
|  Database di Azure per PostgreSQL  |    |    |
|  **Dati e analisi**  |    |    |
|  Databricks  |    |    |
|  HDInsight  |  X  |  X  |
|  Analisi di flusso  |    |  X  |
|  Data Factory  |    |    |
|  Log Analytics  |  X  |    |
|  Data Catalog  |    |    |
|  Data Lake Store  |    |    |
|  Data Lake Analytics  |    |    |
|  Azure Analysis Services  |    |    |
|  Power BI Embedded  |    |    |
|  **Intelligenza artificiale e servizi cognitivi**  |    |    |
|  Machine Learning  |    |  X  |
|  servizio Azure Bot  |    |    |
|  Servizi cognitivi  |    |    |
|  Azure Batch per intelligenza artificiale  |    |    |
|  **Internet delle cose**  |    |    |
|  Hub IoT  |  X  |  X  |
|  IoT Central  |    |    |
|  Machine Learning  |    |  X  |
|  Analisi di flusso  |    |  X  |
|  Hub eventi  |  X  |  X  |
|  Servizi Location Based  |    |    |
|  Hub di notifica  |  X  |  X  |
|  Time Series Insights  |    |    |
|  **Integrazione aziendale**  |    |    |
|  StorSimple  |  X  |    |
|  Gestione API  |    |    |
|  Griglia di eventi  |    |    |
|  Data Factory  |    |    |
|  Bus di servizio  |  X  |  X  |
|  Data Catalog  |    |    |
|  SQL Server Stretch Database  |    |  X  |
|  Funzionalità App per la logica di Servizio app di Azure  |    |    |
|  **Sicurezza e identità**  |    |    |
|  Azure Active Directory  |  X  |  X  |
|  Azure Active Directory B2C  |    |    |
|  Multi-Factor Authentication  |    |    |
|  Azure Active Directory Domain Services  |    |    |
|  Key Vault  |  X  |  X  |
|  Centro sicurezza  |  X  |  X  |
|  **Strumenti di sviluppo**  |    |    |
|  Visual Studio Team Services  |    |    |
|  Application Insights  |    |    |
|  DevTest Labs  |    |    |
|  Visual Studio App Center  |    |    |
|  Xamarin University  |    |    |
|  **Monitoraggio e gestione**  |    |    |
|  Advisor  |    |    |
|  Backup  |  X  |  X  |
|  Site Recovery  |  X  |  X  |
|  Utilità di pianificazione  |  X  |  X  |
|  Automazione  |  X  |  X  |
|  Log Analytics  |  X  |    |
|  Monitoraggio di Azure  |    |    |
|  Applicazioni gestite di Azure  |    |    |
|  Azure Migrate  |    |    |
|  Gruppi di gestione  |    |  

### <a name="next-steps"></a>Passaggi successivi

- [Scopri](https://docs.microsoft.com/azure/cloud-solution-provider/overview/partner-center-overview) le funzionalità disponibili per Azure nel Centro per i partner.

- [Crea](https://docs.microsoft.com/azure/cloud-solution-provider/customer-management/create-new-customer) il tuo primo cliente in Azure CSP e distribuisci i servizi di Azure.

## <a name="transition-existing-csp-offers-to-an-azure-plan"></a>Eseguire la transizione delle offerte CSP esistenti a un piano di Azure

È possibile eseguire la transizione di un cliente da un'offerta CSP per Azure esistente ai servizi di Azure inclusi nel piano per Azure della nuova esperienza commerciale del programma CSP dall'interno del Centro per i partner. A questo scopo, il partner deve aver stabilito con il cliente una relazione come rivenditore tramite il Centro per i partner e il cliente deve aver firmato il Contratto del cliente Microsoft.

### <a name="select-transition-to-azure-plan"></a>Selezionare la transizione al piano di Azure

1. Seleziona il piano di Azure per il cliente.

2. Seleziona **Fatturazione di transizione al piano di Azure**.

![transizione](images/azure/transition1.png)

3. Seleziona **Continua**.

![transizione](images/azure/transition2.png)

Verrà eseguita la transizione del cliente al piano di Azure.

**Durante il flusso della transizione vengono eseguiti automaticamente i passaggi preliminari seguenti**:

- Acquisto di uno o più piani di Azure
- Un piano per cliente in scenari CSP diretti  
- Un piano per rivenditore  

Si supponga, ad esempio, che un partner abbia acquistato due offerte Microsoft Azure e abbia incluso due partner registrati distinti nell'acquisto. In questo caso, durante il flusso della transizione verranno acquistati due piani di Azure (uno per rivenditore) e verrà eseguito automaticamente il mapping delle rispettive sottoscrizioni di Azure in base ai piani di Azure.  

**Mapping della sottoscrizione di Azure al piano di Azure**

Dopo aver acquistato uno o più piani di Azure, il sistema eseguirà il mapping delle sottoscrizioni di Azure esistenti ai piani di Azure. Lo stato di avanzamento può essere visualizzato nel portale di Azure e nel Centro per i partner. 

4. Torna alla pagina **Sottoscrizioni** del cliente nel Centro per i partner per aggiornare il relativo limite di budget nella valuta locale. 

![Transizione](images/azure/transition3.png)

>[!NOTE]
>Il budget che imposti nel Centro per i partner non viene trasferito al portale di Azure. Devi quindi impostare il budget e l'avviso nel portale di Azure.

Dopo essere passato al piano di Azure, non potrai più acquistare sottoscrizioni di Azure per questo cliente. Le sottoscrizioni vengono create in base al piano di Azure nel portale di Azure.

>[!NOTE]
> Tutte le sottoscrizioni di Azure acquistate tramite il controllo degli accessi in base al ruolo nel piano di Azure verranno addebitate e fatturate in valuta locale. Non verranno usati i tassi di cambio.

### <a name="track-your-transition-details"></a>Tenere traccia dei dettagli della transizione

Puoi seguire lo stato di avanzamento della transizione sia nel portale di Azure sia nel Centro per i partner.

![Mostra dettagli](images/azure/details1.png)

**Effetti sulla fatturazione per i partner**

Se esegui la transizione di un cliente da un'offerta CSP per Azure esistente, avrai gli effetti seguenti sulla fatturazione:

- Ti verrà addebitato il costo della fattura CSP esistente per tutto l'utilizzo fino al momento della chiusura della sottoscrizione CSP per Azure originale.

- Se disponi dei diritti di accesso di amministratore per la sottoscrizione CSP esistente, continuerai ad avere gli stessi diritti anche dopo la migrazione della sottoscrizione.

Per eseguire la transizione diretta dei contratti Enterprise Agreement a CSP e delle registrazioni SCE (Server and Cloud Enrollment) ai servizi di Azure, leggi [Acquisire la proprietà della fatturazione delle sottoscrizioni di Azure per il Contratto Microsoft Partner](https://docs.microsoft.com/azure/billing/mpa-request-ownership).

**Log di controllo**:

Per riconciliare la fatturazione, visualizza la cronologia delle sottoscrizioni di "Microsoft Azure" (0145P) nella pagina **Sottoscrizioni**. 

La sottoscrizione di "Microsoft Azure" (0145P) è costituita da due parti:
1. Sottoscrizione commerciale 
2. Sottoscrizione di Azure (diritto)

Al termine della transizione, la sottoscrizione di Azure viene spostata nel nuovo piano di Azure e la sottoscrizione commerciale viene sospesa per evitare la registrazione di altro utilizzo.  

>[Nota]\: quando la sottoscrizione di Microsoft Azure (0145P) viene acquistata in CSP, la sottoscrizione commerciale e la sottoscrizione di Azure (diritto) hanno lo stesso valore. I valori sono diversi solo nel caso di modifiche o trasferimenti della proprietà della fatturazione. 

**Problemi di transizione**

Non sono previsti problemi durante le transizioni. Se si verifica un errore, verrai aggiornato durante il flusso della transizione. Non vi saranno interferenze con l'utilizzo di Azure.  

## <a name="next-steps"></a>Passaggi successivi

- [Gestire sottoscrizioni e risorse nel piano di Azure](azure-plan-manage.md)

- [Credito ottenuto dai partner - Panoramica](partner-earned-credit.md)



