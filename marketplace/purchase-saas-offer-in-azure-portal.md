---
title: Come acquistare un'offerta SaaS in portale di Azure
description: Informazioni su come trovare e acquistare un'offerta SaaS in portale di Azure.
author: mingshen-ms
ms.author: mingshen
ms.reviewer: dannyevers
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: how-to
ms.date: 06/04/2021
ms.openlocfilehash: 8dba9f95607a4172e6d5d0bc2ec148a25b599cd1
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431455"
---
# <a name="purchase-a-saas-offer-in-azure-portal"></a>Acquistare un'offerta SaaS in portale di Azure

Questo articolo illustra le diverse opzioni e i requisiti per la ricerca, il tentativo e l'acquisto di un'offerta Software-as-a-Service (SaaS) dal portale di Azure.

## <a name="saas-offers-discovery-in-azure-portal"></a>SaaS offre l'individuazione in portale di Azure

Quando si è in portale di Azure, esistono diversi modi per restringere la ricerca per concentrarsi sulle offerte SaaS.

### <a name="narrowing-your-search"></a>Restringere la ricerca

Nella home page, in **Servizi di Azure** selezionare + Crea una risorsa **o** **Marketplace.** Oppure usare il tasto **di scelta rapida G + N** in qualsiasi punto della piattaforma.

- Limitare i risultati alle offerte SaaS usando il filtro **Tipo di** offerta e quindi **selezionando SaaS.**
- Usare la ricerca globale nella parte superiore dell'area di spostamento per trovare un'offerta SaaS specifica.

Trovare [un'offerta SaaS privata](/marketplace/private-offers) selezionando il banner nella parte superiore della home **page del Marketplace.** Non tutte le offerte o i piani sono disponibili in tutte le aree geografiche e alcune potrebbero essere visualizzate solo per determinati tenant.

La visualizzazione filtrata mostra ogni offerta SaaS disponibile rappresentata da un titolo. Selezionarne uno per visualizzare la pagina dei dettagli del prodotto. Che include le sezioni seguenti:

- Panoramica: informazioni dettagliate sul servizio, il marketing e i materiali per l'apprendimento
- Piani e prezzi: ogni offerta includerà almeno un piano con prezzi e termini di fatturazione diversi
- Informazioni sull'utilizzo e supporto: include l'ID editore, l'ID offerta e l'ID piano
- Valutazione e recensioni dell'offerta SaaS specifica

## <a name="available-billing-models-plansskus-for-saas-offers"></a>Modelli di fatturazione disponibili (piani/SKU) per le offerte SaaS

Ogni offerta SaaS avrà uno o più piani. A ogni offerta è associato un modello di prezzi: tariffa flat o per utente. Ogni prezzo del piano è una tariffa ricorrente, che può essere pari a zero dollari (tutti i prezzi elencati sono solo a scopo di esempio e non sono destinati a riflettere i costi effettivi). Si tratta di una tariffa fissa o di un prezzo per utente. Tipi di piani disponibili:

- **Piani mensili:** tariffa mensile ricorrente; tariffa mensile fissa o per utente che viene pagata con una ricorrenza mensile. Al termine del periodo, il piano verrà rinnovato automaticamente.
- **Piani annuali:** tariffa annuale ricorrente; tariffa annuale fissa o per utente pagata in base a una ricorrenza annuale. Al termine del periodo, il piano verrà rinnovato automaticamente.
- **Contatori personalizzati:** insieme alle tariffe ricorrenti, un piano tariffare fisso può includere anche dimensioni a consumo personalizzate facoltative per l'utilizzo in evaso non incluso nella tariffa flat. Ogni dimensione rappresenta un'unità fatturabile. Si tratta di un costo variabile che cambia in base all'utilizzo delle unità a consumo, ad esempio larghezza di banda, ticket o posta elettronica elaborata. L'addebito verrà addebitato in base al consumo di queste dimensioni su base mensile. Si noti che il consumo in evaso inizia solo quando sono state usate tutte le unità a consumo incluse nella tariffa flat.
- **Versione di valutazione** gratuita: in alcuni casi, il piano include un periodo di valutazione di un mese, durante il quale è possibile usare il software gratuitamente.  Al termine del periodo di valutazione, verranno addebitati i costi in base al piano. Le offerte di valutazione non sono compatibili con i contatori personalizzati.

Questi modelli di determinazione prezzi sono disponibili sia per i piani pubblici che per i piani privati.

## <a name="saas-purchase-experience"></a>Esperienza di acquisto SaaS

1. Nella pagina del prodotto selezionare un piano che soddisfi le proprie esigenze e continuare a **configurare e sottoscrivere**
2. Come parte del processo di acquisto, si verrà reindirizzati alla scheda **Informazioni** di base e verrà richiesto di:
    1. Definire la *sottoscrizione* da usare per la fatturazione. Per la sottoscrizione di Azure in uso deve essere definito un metodo di acquisto valido. È necessario disporre del livello di autorizzazione giusto o disporre di un gruppo di risorse in tale sottoscrizione con il livello di autorizzazioni giusto. Inoltre, il paese di fatturazione deve essere un paese in cui l'offerta è disponibile per l'acquisto. Le sottoscrizioni di Azure senza un metodo di pagamento valido (ad esempio una sottoscrizione MSDN) possono essere usate solo per acquistare piani gratuiti
    1. Scegliere o creare un **gruppo di risorse a* cui appartenga la risorsa SaaS.
    1. Digitare un *nome per* la sottoscrizione SaaS per identificarla facilmente in un secondo momento. Dopo l'acquisto, non è possibile modificare il nome.
    1. In **Piano** verrà visualizzato il piano selezionato nella pagina dei dettagli del prodotto. Se non è stata effettuata una selezione attiva nel PDP, verrà visualizzato il piano predefinito. È possibile modificare la selezione selezionando il **collegamento Cambia** piano. Selezionare il periodo di fatturazione pertinente e quindi scegliere un altro piano. È possibile modificare il piano dopo l'acquisto, se l'editore lo supporta. Tuttavia, non sarà possibile modificare il periodo da mensile a annuale o da annuale a mensile.
    1. Nei casi in cui il modello tariffario *è per utente*, potrebbe essere necessario specificare il numero di *utenti*. Il prezzo visualizzato cambierà in base alla sottoscrizione, al piano e al termine selezionati.
3. Passare alla **scheda Tag:** *i* tag sono coppie chiave/valore definite dall'utente, che possono essere inserite direttamente in una risorsa o in un gruppo di risorse. È possibile usare i tag per trovare facilmente la risorsa SaaS in un secondo momento. Azure supporta attualmente fino a 50 tag per risorsa e gruppo di risorse. I tag possono essere posizionati su una risorsa al momento della creazione o aggiunti a una risorsa esistente.
4. Passare a **Rivedi e sottoscrivi** per esaminare i dettagli dell'offerta e del piano.
    1. Esaminare *Condizioni per l'utilizzo,* *le modifiche* e *l'informativa sulla privacy* dell'editore e anche per Azure Marketplace
    1. Potrebbe essere richiesto di aggiungere i dettagli di contatto
    1. Esaminare *i dettagli di nozioni* di base *e* tag
5. Al momento della conferma, selezionare **Sottoscrivi**.

## <a name="saas-subscription-and-configuration"></a>Sottoscrizione e configurazione SaaS

Quando si seleziona sottoscrivi, viene visualizzato un messaggio che indica che la sottoscrizione SaaS è in corso. Questo processo dovrebbe richiedere alcuni minuti. Non chiudere la finestra fino al termine.

Al termine della sottoscrizione, viene visualizzato un messaggio che indica che la sottoscrizione SaaS è stata completata ed è necessario configurare l'account per iniziare a usufruire dell'acquisto. Si riceverà anche un messaggio di posta elettronica che richiede di attivare la nuova sottoscrizione. Se non si è l'utente che configurerà l'account SaaS, inoltrare questo messaggio di posta elettronica alla persona pertinente.

Per completare il processo e iniziare a usare saaS, è necessario avviare la configurazione della sottoscrizione. Selezionando il pulsante **Configura account ora,** si verrà reindirizzati al sito Web dell'editore.

È anche possibile controllare lo stato della sottoscrizione selezionando l'icona a forma di campana nell'angolo superiore destro dell'intestazione.

Se il processo di configurazione non viene completato entro *30* giorni, questa sottoscrizione SaaS verrà eliminata *automaticamente.* La fatturazione inizierà dopo la configurazione dell'account nel sito Web dell'editore.

Messaggi di errore che potrebbero verificarsi durante il processo:

- Il nome *del piano selezionato non può* essere acquistato in una sottoscrizione gratuita
  - Aggiornare l'account. Per https://aka.ms/UpgradeFreeSub altri dettagli, vedere .

- L'acquisto non è riuscito perché non è stato possibile trovare una carta di credito valida o un metodo di pagamento associato alla sottoscrizione di Azure.
  - Usare una sottoscrizione di Azure diversa o aggiungere o aggiornare la carta di credito o il metodo di pagamento corrente per questa sottoscrizione e riprovare.

- Il nome del piano  selezionato per  *il* nome dell'offerta in base all'editore dell'offerta non è disponibile per l'acquisto in base alle regole impostate dall'amministratore IT.
  - Contattare l'amministratore IT.

- Il *nome del piano selezionato* dal  piano di offerta selezionato dall'editore dell'offerta non è disponibile per l'acquisto a causa delle impostazioni del marketplace privato effettuate dall'amministratore IT del tenant. 
  - Contattare l'amministratore IT

- L'acquisto non è riuscito perché il periodo di fatturazione richiesto è vuoto o non valido.
  - Provare ad acquistare un piano o un periodo di fatturazione diverso.

- L'acquisto non è riuscito perché non è stato possibile verificare l'accesso al contratto legale.
  - Riprovare. Se l'errore persiste, provare a effettuare l'acquisto usando una sottoscrizione di Azure diversa o contattare il supporto tecnico.

- L'acquisto *dell'OFFER OFFERID* per publisher *publisherID* non è riuscito. Questa offerta non è attualmente disponibile per l'acquisto.
  - Riprovare più tardi. Se dopo un'ora si continua a ricevere questo messaggio di errore, contattare il supporto tecnico.  

- L'acquisto di *planID del piano* dell'offerta *offerID* per *publisher publisherID* non è riuscito. Questo piano non è attualmente disponibile per l'acquisto.
  - Riprovare più tardi. Se dopo un'ora si continua a ricevere questo messaggio di errore, contattare il supporto tecnico. 

- L'indirizzo *di posta elettronica* del client con ID oggetto *ObjectID* non ha l'autorizzazione per eseguire l'azione *DeploymentValidationAction* sull'ambito *ResourceGroup. DeploymentScope o* l'ambito non è valido.  
  - Questo messaggio verrà visualizzato se non si hanno le autorizzazioni appropriate per la sottoscrizione o il gruppo di risorse di Azure.  
    Se l'accesso è stato concesso di recente, aggiornare le credenziali.  
    Per distribuire le risorse in un gruppo di risorse, è necessario avere almeno l'accesso collaboratore. Controllare lo stato di accesso in **Gruppi di risorse e** quindi controllo di **accesso**. Viene visualizzato chi è il "Proprietario", a cui è possibile chiedere di assegnare l'utente come "Collaboratore".

- La sottoscrizione usata per questo acquisto non consente gli acquisti nel Marketplace.  
  - Usare una sottoscrizione diversa o chiedere all'amministratore di modificare la definizione della sottoscrizione e riprovare.

## <a name="next-steps"></a>Passaggi successivi

- Se è già stata acquistata un'offerta nel marketplace, passare [a Fatturazione](/marketplace/billing-invoicing)
- È anche possibile ottenere altre informazioni sulle [opzioni dei piani](/marketplace/private-offers) privati.
