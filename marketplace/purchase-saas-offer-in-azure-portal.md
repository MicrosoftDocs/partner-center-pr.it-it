---
title: Come acquistare un'offerta SaaS in portale di Azure
description: Informazioni su come trovare e acquistare un'offerta SaaS in portale di Azure.
author: mingshen-ms
ms.author: mingshen
ms.reviewer: dannyevers
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: how-to
ms.date: 06/29/2021
ms.openlocfilehash: a124e4c5bb31a1fbb744bf2c5e1ea65a356bdd54
ms.sourcegitcommit: 1d09ccaaa54f167b0c63e99761172ebe84e89f2e
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/02/2021
ms.locfileid: "113221441"
---
# <a name="purchase-a-saas-offer-in-azure-portal"></a>Acquistare un'offerta SaaS in portale di Azure

Questo articolo illustra le diverse opzioni e i requisiti per la ricerca, il tentativo e l'acquisto di un'offerta SaaS (Software-as-a-Service) dal portale di Azure.

## <a name="create-a-saas-subscription"></a>Creare una sottoscrizione SaaS

Per acquistare una sottoscrizione SaaS, è necessario un account utente di Azure con accesso a una sottoscrizione di Azure appropriata. Questa sottoscrizione verrà usata per la fatturazione e per la raggruppamento delle risorse cloud acquistate. Per altre informazioni sulle sottoscrizioni di Azure, vedere [Creare una sottoscrizione di Azure aggiuntiva.](/azure/cost-management-billing/manage/create-subscription)

Nel portale di Azure selezionare l'offerta SaaS desiderata nella **sezione Marketplace.**

Una sottoscrizione Software-as-a-Service offre il diritto di usare un servizio per un determinato periodo di tempo tramite una sottoscrizione online anziché l'installazione locale nei singoli computer. Una sottoscrizione è un contratto per l'uso di una o più piattaforme o servizi cloud, per i quali gli addebiti si accumulano in base a una tariffa di licenza per utente o al consumo di risorse basato sul cloud. Un'organizzazione può avere più sottoscrizioni SaaS.

Le restrizioni per le sottoscrizioni SaaS includono:

- Nessuna sottoscrizione per studenti.
- Nessuna Visual Studio Enterprise sottoscrizione.
- Nessuna sottoscrizione di credito gratuita.
- Per le offerte a pagamento è necessario uno strumento di pagamento.

## <a name="saas-offers-discovery-in-azure-portal"></a>SaaS offre l'individuazione in portale di Azure

Una volta che si è portale di Azure, esistono alcuni modi per restringere la ricerca per concentrarsi sulle offerte SaaS.

### <a name="narrowing-your-search"></a>Restringere la ricerca

Nella home page, in **Servizi di Azure selezionare** + Crea una risorsa **o** **Marketplace.** Oppure usare il tasto **di scelta rapida G + N** in qualsiasi punto della piattaforma.

- Limitare i risultati alle offerte SaaS usando il filtro **Tipo di** offerta e quindi selezionando **SaaS**.
- Usare la ricerca globale nella parte superiore dell'area di spostamento per trovare un'offerta SaaS specifica.

Trovare [un'offerta SaaS privata](/marketplace/private-offers) selezionando il banner nella parte superiore della home page **del Marketplace.** Non tutte le offerte o i piani sono disponibili in tutte le aree geografiche e alcune potrebbero essere visualizzate solo per determinati tenant.

La visualizzazione filtrata mostra ogni offerta SaaS disponibile rappresentata da un titolo. Selezionarne uno per visualizzare la pagina dei dettagli del prodotto. Che include le sezioni seguenti:

- Panoramica: informazioni dettagliate sul servizio, sul marketing e sui materiali di apprendimento
- Piani e prezzi: ogni offerta includerà almeno un piano con termini e prezzi di fatturazione diversi
- Informazioni sull'utilizzo e supporto: include l'ID Publisher, l'ID offerta e l'ID piano
- Valutazione e recensioni dell'offerta SaaS specifica

## <a name="available-billing-models-plansskus-for-saas-offers"></a>Modelli di fatturazione disponibili (piani/SKU) per le offerte SaaS

Ogni offerta SaaS avrà uno o più piani. A ogni offerta è associato un modello di prezzi: tariffa forf semplice o per utente. Ogni prezzo del piano è una tariffa ricorrente, che può essere pari a zero dollari (tutti i prezzi elencati sono solo a scopo di esempio e non sono destinati a riflettere i costi effettivi). Questa tariffa è una tariffa fissa o un prezzo per utente. Tipi di piani disponibili:

- **Piani mensili:** tariffa mensile ricorrente; tariffa mensile fissa o per utente che viene pagata in base a una ricorrenza mensile. Al termine del periodo, il piano verrà rinnovato automaticamente.
- **Piani annuali:** tariffa annuale ricorrente; tariffa annuale fissa o per utente che viene pagata in base a una ricorrenza annuale. Al termine del periodo, il piano verrà rinnovato automaticamente.
- **Contatori personalizzati:** insieme alle tariffe ricorrenti, un piano tariffare fisso può includere anche dimensioni a consumo personalizzate facoltative per l'utilizzo delle sovrattese non incluse nella tariffa forfazione. Ogni dimensione rappresenta un'unità fatturabile. Si tratta di un costo variabile che cambia in base all'utilizzo delle unità a consumo, ad esempio: larghezza di banda, ticket o posta elettronica elaborata. L'addebito verrà addebitato in base al consumo di queste dimensioni su base mensile. Si noti che il consumo di sovrattesto inizia solo quando sono state usate tutte le unità a consumo incluse nella tariffa forfazione.
- **Versione di** valutazione gratuita: in alcuni casi, il piano include un periodo di valutazione di un mese, durante il quale è possibile usare il software gratuitamente.  Al termine del periodo di valutazione, l'addebito verrà addebitato in base al piano. Le offerte di valutazione non sono compatibili con i contatori personalizzati.

Questi modelli di prezzi sono disponibili sia per i piani pubblici che per i piani privati.

## <a name="saas-purchase-experience"></a>Esperienza di acquisto SaaS

1. Nella pagina del prodotto selezionare un piano che soddisfi le proprie esigenze e continuare a **configurare e sottoscrivere**
2. Come parte del processo di acquisto, si verrà reindirizzati alla scheda **Informazioni** di base e sarà necessario:
    1. Definire la *sottoscrizione* da usare per la fatturazione. Per la sottoscrizione di Azure in uso deve essere definito un metodo di acquisto valido. È necessario disporre del livello di autorizzazione giusto o disporre di un gruppo di risorse in tale sottoscrizione con il livello di autorizzazioni giusto. Inoltre, il paese di fatturazione deve essere un paese in cui l'offerta è disponibile per l'acquisto. Le sottoscrizioni di Azure senza un metodo di pagamento valido (ad esempio una sottoscrizione MSDN) possono essere usate solo per acquistare piani gratuiti
    1. Scegliere o creare un **gruppo di risorse* a cui appartiene la risorsa SaaS.
    1. Digitare un *nome per* la sottoscrizione SaaS per identificarla facilmente in un secondo momento. Dopo l'acquisto, non è possibile modificare il nome.
    1. In **Piano** verrà visualizzato il piano selezionato nella pagina dettagliata del prodotto (PDP). Se non è stata effettuata una selezione attiva nel PDP, verrà visualizzato il piano predefinito. È possibile modificare la selezione selezionando il **collegamento Cambia** piano. Selezionare il termine di fatturazione pertinente e quindi scegliere un altro piano. È possibile modificare il piano dopo l'acquisto, se l'editore lo supporta. Tuttavia, non sarà possibile modificare il termine da mensile a annuale o da annuale a mensile.
    1. Nei casi in cui il modello tariffario *è per utente,* potrebbe essere necessario specificare il numero di *utenti*. Il prezzo visualizzato cambierà in base alla sottoscrizione, al piano e al termine selezionati.
3. Passare alla **scheda** *Tag:* i tag sono coppie chiave/valore definite dall'utente, che possono essere inserite direttamente in una risorsa o in un gruppo di risorse. È possibile usare i tag per trovare facilmente la risorsa SaaS in un secondo momento. Azure supporta attualmente fino a 50 tag per risorsa e gruppo di risorse. I tag possono essere posizionati su una risorsa al momento della creazione o aggiunti a una risorsa esistente.
4. Continuare a **esaminare e sottoscrivere** per esaminare i dettagli dell'offerta e del piano.
    1. Esaminare *Condizioni per l'utilizzo,* *le modifiche* e l'informativa sulla *privacy* dell'editore e anche per Azure Marketplace
    1. Potrebbe essere richiesto di aggiungere i dettagli di contatto
    1. Esaminare *i dettagli di nozioni* di base *e* tag
5. Al momento della conferma, selezionare **Sottoscrivi**.

## <a name="saas-subscription-and-configuration"></a>Sottoscrizione e configurazione SaaS

Quando si seleziona sottoscrivi, viene visualizzato il messaggio "La sottoscrizione SaaS è in corso". Questo processo dovrebbe richiedere alcuni minuti, non chiudere la finestra fino al termine.

Al termine della sottoscrizione, un messaggio indica che la sottoscrizione SaaS è stata completata ed è necessario configurare l'account per iniziare a usufruire dell'acquisto. Si riceverà anche un messaggio di posta elettronica che richiede di attivare la nuova sottoscrizione. Se non si è l'utente che configurerà l'account SaaS, inoltrare questo messaggio di posta elettronica alla persona pertinente.

Per completare il processo e iniziare a usare SaaS, è necessario avviare la configurazione della sottoscrizione. Selezionando il **pulsante Configura account ora,** si reindirizza al sito Web dell'editore.

È anche possibile controllare lo stato della sottoscrizione selezionando l'icona "campanella" nell'angolo superiore destro dell'intestazione.

Se il processo di configurazione non viene completato entro *30* giorni, questa sottoscrizione SaaS verrà eliminata *automaticamente.* La fatturazione inizierà dopo la configurazione dell'account nel sito Web dell'editore.

Messaggi di errore che potrebbero verificarsi durante il processo:

- Il nome *del piano selezionato non* può essere acquistato in una sottoscrizione gratuita
  - Aggiornare l'account, vedere https://aka.ms/UpgradeFreeSub per altri dettagli.

- L'acquisto non è riuscito perché non è stata individuata una carta di credito valida né un metodo di pagamento associato alla sottoscrizione di Azure.
  - Usare una sottoscrizione di Azure diversa o aggiungere\aggiornare la carta di credito o il metodo di pagamento corrente per questa sottoscrizione e riprovare.

- Il *nome del piano selezionato del*  nome dell'offerta dall'editore dell'offerta non è disponibile per l'acquisto in base alle regole impostate dall'amministratore IT. 
  - Contattare l'amministratore IT.

- Il *nome del piano selezionato* dal  piano di offerta selezionato dall'editore dell'offerta non è disponibile per l'acquisto a causa delle impostazioni del marketplace privato effettuate dall'amministratore IT del tenant. 
  - Contattare l'amministratore IT

- L'acquisto non è riuscito perché il termine di fatturazione richiesto è vuoto o non valido.
  - Provare ad acquistare un piano o un periodo di fatturazione diverso.

- L'acquisto non è riuscito perché non è stato possibile verificare la firma del contratto legale.
  - Riprovare. Se l'errore persiste, provare a effettuare l'acquisto usando una sottoscrizione di Azure diversa o contattare il supporto tecnico.

- L'acquisto di *offerID da* parte dell'editore *publisherID* non è riuscito. Questa offerta non è attualmente disponibile per l'acquisto.
  - Riprovare più tardi. Se dopo un'ora si continua a ricevere questo messaggio di errore, contattare il supporto tecnico.  

- L'acquisto del *planID del piano* *dell'offer offerID* da publisher *publisherID* non è riuscito. Questo piano non è attualmente disponibile per l'acquisto.
  - Riprovare più tardi. Se dopo un'ora si continua a ricevere questo messaggio di errore, contattare il supporto tecnico. 

- L'indirizzo *di posta elettronica* del client con ID oggetto *ObjectID* non dispone dell'autorizzazione per eseguire l'azione *DeploymentValidationAction* sull'ambito *ResourceGroup. DeploymentScope o* l'ambito non è valido.  
  - Questo messaggio viene visualizzato se non si dispone delle autorizzazioni appropriate per la sottoscrizione o il gruppo di risorse di Azure.  
    Se l'accesso è stato concesso di recente, aggiornare le credenziali.  
    Per distribuire le risorse in un gruppo di risorse, è necessario disporre almeno dell'accesso collaboratore. Controllare lo stato di accesso in **Gruppi di risorse** e quindi Controllo di **accesso**. Questo mostra chi è il "Proprietario", a cui è possibile chiedere di assegnare l'utente come "Collaboratore".

- La sottoscrizione usata per questo acquisto non consente gli acquisti nel Marketplace.  
  - Usare una sottoscrizione diversa o chiedere all'amministratore di modificare la definizione della sottoscrizione e riprovare.

## <a name="next-steps"></a>Passaggi successivi

- Se è già stata acquistata un'offerta nel marketplace, passare a [Fatturazione e fatturazione](/marketplace/billing-invoicing)
- È anche possibile ottenere altre informazioni sulle [opzioni dei piani](/marketplace/private-offers) privati.
