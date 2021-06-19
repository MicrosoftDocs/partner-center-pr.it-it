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
ms.openlocfilehash: b73a9acb7b9cf9eee1151de1f8e45f6fd6ef256f
ms.sourcegitcommit: 8511fec63961d8c77a4d1eea3e3f1d37cdea46c6
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/19/2021
ms.locfileid: "112373475"
---
# <a name="purchase-a-saas-offer-in-azure-portal"></a>Acquistare un'offerta SaaS in portale di Azure

Questo articolo illustra le diverse opzioni e requisiti per la ricerca, il tentativo e l'acquisto di un'offerta SaaS (Software-as-a-Service) dal portale di Azure.

## <a name="saas-offers-discovery-in-azure-portal"></a>SaaS offre l'individuazione in portale di Azure

Quando si è in portale di Azure, è possibile restringere la ricerca per concentrarsi sulle offerte SaaS.

### <a name="narrowing-your-search"></a>Restringere la ricerca

Nella home page, in **Servizi di Azure selezionare** + Crea una **risorsa** o **Marketplace.** Oppure usare il tasto **di scelta rapida G + N** in qualsiasi punto della piattaforma.

- Limitare i risultati alle offerte SaaS usando il filtro **Tipo di** offerta e quindi selezionando **SaaS**.
- Usare la ricerca globale nella parte superiore dell'area di spostamento per trovare un'offerta SaaS specifica.

Trovare [un'offerta SaaS privata](/marketplace/private-offers) selezionando il banner nella parte superiore della home page **del Marketplace.** Non tutte le offerte o i piani sono disponibili in tutte le aree geografiche e alcune potrebbero essere visualizzate solo per determinati tenant.

La visualizzazione filtrata mostra ogni offerta SaaS disponibile rappresentata da un titolo. Selezionarne uno per visualizzare la pagina dei dettagli del prodotto. Che include le sezioni seguenti:

- Panoramica: informazioni dettagliate sul servizio, sul marketing e sui materiali di apprendimento
- Piani e prezzi: ogni offerta includerà almeno un piano con termini e prezzi di fatturazione diversi
- Informazioni sull'utilizzo e supporto: include l'ID editore, l'ID offerta e l'ID piano
- Valutazione e recensioni dell'offerta SaaS specifica

## <a name="available-billing-models-plansskus-for-saas-offers"></a>Modelli di fatturazione disponibili (piani/SKU) per le offerte SaaS

Ogni offerta SaaS avrà uno o più piani. A ogni offerta è associato un modello di prezzi: tariffa forfattia o per utente. Ogni prezzo del piano è una tariffa ricorrente, che può essere pari a zero dollari (tutti i prezzi elencati sono solo a scopo di esempio e non sono destinati a riflettere i costi effettivi). Questa tariffa è una tariffa fissa o un prezzo per utente. Tipi di piani disponibili:

- **Piani mensili:** tariffa mensile ricorrente; tariffa mensile fissa o per utente che viene pagata in base a una ricorrenza mensile. Al termine del periodo, il piano verrà rinnovato automaticamente.
- **Piani annuali:** tariffa annuale ricorrente; tariffa annuale fissa o per utente che viene pagata in una ricorrenza annuale. Al termine del periodo, il piano verrà rinnovato automaticamente.
- **Contatori personalizzati:** insieme alle tariffe ricorrenti, un piano tariffare flat può includere anche dimensioni a consumo personalizzate facoltative per l'utilizzo di sovrattesto non incluse nella tariffa forfazione. Ogni dimensione rappresenta un'unità fatturabile. Si tratta di un costo variabile che cambia in base all'utilizzo delle unità a consumo, ad esempio larghezza di banda, ticket o posta elettronica elaborata. L'addebito verrà addebitato in base al consumo di queste dimensioni su base mensile. Si noti che il consumo di sovrattesto inizia solo quando sono state usate tutte le unità a consumo incluse nella tariffa forfazione.
- **Versione di** valutazione gratuita: in alcuni casi, il piano include un periodo di valutazione di un mese, durante il quale è possibile usare il software gratuitamente.  Al termine del periodo di valutazione, l'addebito verrà addebitato in base al piano. Le offerte di valutazione non sono compatibili con i contatori personalizzati.

Questi modelli di prezzi sono disponibili sia per i piani pubblici che per i piani privati.

## <a name="saas-purchase-experience"></a>Esperienza di acquisto SaaS

1. Nella pagina del prodotto selezionare un piano che soddisfi le proprie esigenze e continuare a **configurare e sottoscrivere**
2. Come parte del processo di acquisto, si verrà reindirizzati alla scheda **Informazioni** di base e sarà necessario:
    1. Definire la *sottoscrizione* da usare per la fatturazione. Per la sottoscrizione di Azure in uso deve essere definito un metodo di acquisto valido. È necessario disporre del livello di autorizzazione giusto o disporre di un gruppo di risorse in tale sottoscrizione con il livello di autorizzazioni giusto. Inoltre, il paese di fatturazione deve essere un paese in cui l'offerta è disponibile per l'acquisto. Le sottoscrizioni di Azure senza un metodo di pagamento valido (ad esempio una sottoscrizione MSDN) possono essere usate solo per acquistare piani gratuiti
    1. Scegliere o creare un **gruppo di risorse a* cui appartiene la risorsa SaaS.
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

- Se si sta vendendo l'offerta tramite Microsoft, vedere Come aggiungere un gruppo di destinatari di [anteprima per l'offerta SaaS.](/azure/marketplace/create-new-saas-offer-preview)
- In caso contrario, passare [a Come vendere l'offerta SaaS.](/azure/marketplace/create-new-saas-offer-marketing)
