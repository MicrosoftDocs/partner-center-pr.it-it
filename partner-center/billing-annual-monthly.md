---
title: Differenze tra fatturazione mensile e annuale
ms.topic: article
ms.date: 05/06/2020
Description: Scopri come la fatturazione mensile e annuale differisce dal centro per i partner. Viene inoltre illustrato come passare tra diversi tipi di fatturazione e le implicazioni del cambio.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 7a45b3033c448255d5508e7b7abb7a29c1c0a9e9
ms.sourcegitcommit: 37562b0e29ab921b6b454bb9801376f1feedb715
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/22/2020
ms.locfileid: "86943538"
---
# <a name="understand-the-difference-between-monthly-and-annual-billing-in-partner-center"></a>Comprendere la differenza tra fatturazione mensile e annuale nel centro per i partner


**Si applica a**

- Centro per i partner
- Centro per i partner per Microsoft Cloud for US Government

**Ruoli appropriati**

- Agente amministratore
- Amministratore fatturazione
- Amministratore globale
- Amministratore degli incentivi
- Utente di incentivi
- Agente di supporto tecnico
- Agente di vendita

Questo articolo illustra le differenze tra la **fatturazione mensile** e la **fatturazione annuale** nel centro per i partner, inclusi i vantaggi e i casi d'uso. È possibile pagare per determinate sottoscrizioni Cloud Solution Provider (CSP) su base mensile o annuale.

## <a name="applicability"></a>Applicabilità

Per la maggior parte delle sottoscrizioni basate su licenza è possibile utilizzare l'opzione di fatturazione mensile o annuale. Gli abbonamenti basati su utilizzo hanno solo l'opzione di fatturazione mensile.

La fatturazione annuale e mensile è **per sottoscrizione**, ** _non_ per licenza**.

### <a name="find-subscription-applicability"></a>Trova applicabilità della sottoscrizione

È possibile identificare le frequenze di fatturazione disponibili per ogni offerta usando la colonna J nella matrice dell'offerta. È possibile trovare la matrice di offerte nella sezione **vedere le offerte e i prezzi** del centro per i partner.

### <a name="applicable-partners"></a>Partner applicabili

Tutti i partner e i tipi di partner possono scegliere una fatturazione mensile o annuale.

### <a name="applicable-markets"></a>Mercati applicabili

La fatturazione mensile e annuale (per le offerte applicabili) è disponibile in tutti i mercati in cui il programma CSP è attualmente disponibile.

## <a name="change-billing-frequency"></a>Modificare la frequenza di fatturazione

È possibile passare da una fatturazione mensile a una fatturazione annuale in qualsiasi momento. Potrebbe essere necessario modificare la frequenza di fatturazione in caso di modifica delle esigenze aziendali.

Quando si imposta la frequenza di fatturazione su annuale, il termine annuale viene aggiornato in modo da riflettere la data in cui è stata modificata la frequenza di fatturazione. Viene stabilita anche una nuova data di rinnovo.

### <a name="monthly-to-annual-billing"></a>Fatturazione mensile a annuale

Il cambio dalla fatturazione mensile alla fatturazione annuale può essere utile se sono presenti numerose sottoscrizioni fatturate mensilmente. Quando si passa alla fatturazione annuale, è possibile allineare le sottoscrizioni a una data di fatturazione comune.

### <a name="annual-to-monthly-billing"></a>Fatturazione da annuale a mensile

Il trasferimento dalla fatturazione annuale alla fatturazione mensile può essere utile se si desidera modificare le date di fatturazione in base alle date dei singoli clienti.

## <a name="annual-billing"></a>Fatturazione annuale

La fatturazione annuale offre i vantaggi seguenti:

- Maggiore flessibilità nelle opzioni di pagamento.
- Migliore allineamento con la fatturazione dei clienti.
- Impatto ridotto delle fluttuazioni di valuta.
- Costi operativi di fatturazione ridotti.

### <a name="configure-annual-billing"></a>Configurare la fatturazione annuale

Se si prevede di passare alla fatturazione annuale nel centro per i partner, assicurarsi di prendere in considerazione il modo in cui verrà influenzato il movimento delle vendite. Informare il team e aggiornare i processi interni in modo necessario. È inoltre consigliabile esaminare le modifiche apportate alla fattura e al file di riconciliazione basato sulle licenze.

Sarà anche necessario [aggiornare le API per la fatturazione annuale](#required-api-changes).

#### <a name="required-api-changes"></a>Modifiche API richieste

Per poter sfruttare la fatturazione annuale, è necessario apportare alcune modifiche alle API.

- [Proprietà Order. BillingCycle](https://docs.microsoft.com/dotnet/api/microsoft.store.partnercenter.models.orders.order.billingcycle)
- [Creare un ordine](https://docs.microsoft.com/partner-center/develop/create-an-order)

Per ulteriori informazioni sulle API del centro per i partner, vedere tutte [le risorse e la documentazione per gli sviluppatori del centro partner](https://docs.microsoft.com/partner-center/develop/).

## <a name="placing-orders"></a>Posizionamento degli ordini

Il tipo di frequenza di fatturazione, inclusa la fatturazione annuale, viene assegnato all' **offerta** come attributo. Non è disponibile un'offerta univoca per gli ordini con fatturazione annuale. È tuttavia possibile rinominare un'offerta usando un nome più descrittivo per il cliente per distinguere facilmente.

### <a name="select-annual-billing"></a>Selezionare la fatturazione annuale

Quando si aggiunge una nuova sottoscrizione, verrà richiesto di scegliere la frequenza di fatturazione. A questo punto puoi scegliere l'opzione di fatturazione annuale. Quando si seleziona la fatturazione annuale, verranno visualizzate tutte le offerte disponibili.

### <a name="billing-time"></a>Tempo di fatturazione

Ti verrà addebitato il costo della prossima data di fatturazione. Se, ad esempio, la data di fatturazione è il 1 ° del mese e si acquista una sottoscrizione fatturata annualmente il 29 ottobre 2019, verrà addebitato il 1 ° novembre 2019. Supponendo che non vengano apportate modifiche alle licenze, l'addebito verrà addebitato il 1 ° novembre 2020. Se si effettua una modifica della licenza, si riceverà un credito e la fatturazione verrà addebitata alla data di fatturazione successiva.

### <a name="annual-renewals"></a>Rinnovi annuali

La data di rinnovo della sottoscrizione sarà di 12 mesi dopo la data di inizio del servizio. Il periodo del servizio inizia il giorno in cui viene creato l'abbonamento.  Una sottoscrizione creata il 10 gennaio 2019, ad esempio, verrà rinnovata il 10 gennaio 2020.

La fattura verrà emessa alla data di fatturazione successiva alla data di rinnovo dell'abbonamento. Se, ad esempio, acquisti un abbonamento con fatturazione annuale addebitato il 15 gennaio 2018 e la data di fatturazione è il 20 gennaio, l'abbonamento verrà rinnovato il 15 gennaio 2019. La fattura per il rinnovo verrà addebitata il 20 gennaio 2019.

### <a name="split-subscription-billing-frequency"></a>Frequenza di fatturazione della sottoscrizione Split

Non è possibile suddividere una **singola sottoscrizione** in modo che una parte venga fatturata mensilmente e l'altra venga fatturata ogni anno. L'intera sottoscrizione deve avere la stessa frequenza di fatturazione (fatturazione mensile o annuale).

Per i clienti con **più sottoscrizioni** della stessa offerta, potrebbe essere possibile avere frequenze di fatturazione diverse per ogni sottoscrizione. Sono disponibili alcune offerte limitate a una sottoscrizione per cliente. Se l'offerta non è limitata, un cliente può avere più abbonamenti della stessa offerta con frequenze di fatturazione diverse. Puoi trovare i dettagli di tutti i limiti e le restrizioni delle offerte nella colonna I della matrice dell'offerta. È possibile trovare la matrice di offerte nella sezione **vedere le offerte e i prezzi** del centro per i partner.

### <a name="free-subscription-period"></a>Periodo di sottoscrizione gratuito

Le sottoscrizioni con frequenza di fatturazione annuale non ricevono un periodo gratuito. Il termine a pagamento di dodici mesi inizia alla data di acquisto. A differenza delle sottoscrizioni con frequenza di fatturazione mensile che ricevono un periodo di tempo libero dalla data di acquisto alla data di fatturazione successiva.

### <a name="adding-and-removing-licenses"></a>Aggiunta e rimozione di licenze

Puoi modificare la quantità di licenze per gli abbonamenti in qualsiasi momento. L'aggiunta di altre licenze non influirà sulla frequenza di fatturazione.

Puoi aggiungere o rimuovere licenze in qualsiasi momento.  Dopo aver modificato il numero di licenze, si riceverà un credito e una fatturazione rivalutata alla data di fatturazione successiva.

Se la sottoscrizione esistente ha una fatturazione annuale, non è possibile aggiungere licenze con fatturazione mensile a tale sottoscrizione. Quando acquisti un abbonamento con fatturazione annuale, eventuali licenze aggiuntive seguiranno la stessa frequenza di fatturazione. Se quindi devi acquistare licenze con fatturazione mensile, dovrai acquistare un nuovo abbonamento.

### <a name="add-on-offers"></a>Offerte per i componenti aggiuntivi

L'abbonamento per un componente aggiuntivo avrà automaticamente la stessa frequenza di fatturazione dell'abbonamento principale. La fatturazione annuale è disponibile per le offerte per i componenti aggiuntivi. 

### <a name="cancelling-subscriptions"></a>Annullamento di sottoscrizioni

I criteri di annullamento sono identici per tutte le frequenze di fatturazione.

Per la fatturazione annuale, se la sottoscrizione viene annullata nei primi 30 giorni del periodo a pagamento di dodici mesi, si riceverà un credito del 100% sulla data di fatturazione successiva. Se la sottoscrizione viene annullata dopo 30 giorni del periodo di pagamento di dodici mesi, si riceverà un credito ricorsivo per la data di fatturazione successiva.

### <a name="moving-subscriptions-between-partners"></a>Trasferimento di sottoscrizioni tra partner

I clienti non possono spostare le sottoscrizioni tra un partner e l'altro. Questa restrizione si applica alle sottoscrizioni mensili e fatturate annualmente.

Il nuovo partner deve acquistare una nuova sottoscrizione per conto del cliente. Non è possibile spostare le sottoscrizioni tra partner.

### <a name="reactivating-subscriptions"></a>Riattivazione di sottoscrizioni

È possibile riattivare una sottoscrizione per un massimo di 90 giorni dopo la data di sospensione. Riceverai un addebito ripartito proporzionalmente alla data di fatturazione successiva. La data di rinnovo dell'abbonamento rimane invariata.

## <a name="pricing"></a>Prezzi

### <a name="offer-pricing"></a>Prezzi offerta

Il prezzo dell'offerta al momento dell'acquisto è garantito per il periodo di validità della sottoscrizione fatturato (un mese per la fatturazione mensile, 12 mesi per la fatturazione annuale). Quando un abbonamento viene rinnovato, il prezzo viene reimpostato in base al listino prezzi corrente alla data di rinnovo. Il nuovo prezzo è garantito per il periodo di validità della sottoscrizione successivo.

Se il prezzo di un'offerta diminuisce durante il periodo di fatturazione, l'importo addebitato non viene modificato. Il prezzo viene impostato per il periodo di fatturazione completo al momento dell'acquisto. Questa convenzione è valida per la fatturazione mensile e annuale.

### <a name="cancellation-credits"></a>Crediti di annullamento

Il credito per una licenza o una sottoscrizione annullata viene calcolato come segue:

**Credito di annullamento** = ((* * prezzo mensile * * * 12)/365) \* **giorni rimanenti nel** \* numero di licenze del periodo di dodici mesi annullato.

## <a name="reconciliation-file"></a>File di riconciliazione

### <a name="find-subscriptions-billing-frequency"></a>Trovare la frequenza di fatturazione della sottoscrizione

La colonna **AA** del file di riconciliazione indica se la sottoscrizione è fatturata mensilmente o annualmente.

Per sapere se è possibile modificare una sottoscrizione mensile per la fatturazione annuale, vedere l' [applicabilità della sottoscrizione](#find-subscription-applicability).

### <a name="reconciliation-file-changes-for-annual-billing"></a>Modifiche al file di riconciliazione per la fatturazione annuale

Quando si acquista o si rinnova una sottoscrizione con fatturazione annuale, il file di riconciliazione basato su licenza cambierà come segue:

- Nel file di riconciliazione basato su licenza sarà presente una nuova riga alla prima data di fatturazione dopo l'acquisto o una nuova sottoscrizione.

- Se non viene apportata alcuna modifica alla sottoscrizione, non saranno presenti righe nei file di riconciliazione per i mesi da 2 a 12 del periodo di validità della sottoscrizione. Se viene apportata una modifica alla sottoscrizione durante il periodo di dodici mesi, dopo aver apportato la modifica verrà visualizzato un accredito e una fatturazione rivalutata nel successivo file di riconciliazione.

- Quando la sottoscrizione viene rinnovata, verrà visualizzata la successiva modifica al file di riconciliazione. La modifica verrà visualizzata alla prima data di fatturazione dopo il rinnovo.

### <a name="usage-file-changes-for-annual-billing"></a>Modifiche dei file di utilizzo per la fatturazione annuale

Le seguenti modifiche della sottoscrizione fatturate annualmente vengono visualizzate nella colonna P del file di utilizzo:

- **Tariffe**propagate durante l'acquisto: l'acquisto iniziale di una sottoscrizione annuale.
- **Prorata dell'istanza del ciclo**: modifiche della licenza che comportano il credito e la fatturazione.
- **Annullamento della tariffa**: [annullamento di una sottoscrizione annuale](#cancellation-of-annual-subscription).

### <a name="cancellation-of-annual-subscription"></a>Annullamento della sottoscrizione annuale

Quando viene annullata una sottoscrizione fatturata annualmente, il file di riconciliazione conterrà una voce per un credito di annullamento.

Se l'annullamento viene eseguito nei primi 30 giorni del periodo di dodici mesi, la sottoscrizione verrà accreditata al 100%. Se l'annullamento si verifica dopo i primi 30 giorni, la sottoscrizione verrà accreditata proporzionalmente.

### <a name="adding-licenses-to-annual-subscription"></a>Aggiunta di licenze alla sottoscrizione annuale

Quando si aggiungono licenze a una sottoscrizione, il file di riconciliazione conterrà un credito e una fatturazione rivalutata. Questa convenzione si applica alle sottoscrizioni mensili e annuali fatturate.

### <a name="price-lists-for-annual-billing"></a>Elenchi prezzi per la fatturazione annuale

Gli elenchi prezzi del centro per i partner mostrano i prezzi mensili. Non sono elencati prezzi annuali. È possibile calcolare il prezzo annuo moltiplicando il prezzo mensile di 12.

### <a name="offer-matrix"></a>Matrice offerta

Gli ID offerta nella matrice dell'offerta sono gli stessi per tutte le frequenze di fatturazione. Non sono disponibili ID univoci per le offerte che possono essere fatturate annualmente.

## <a name="incentives"></a>Incentivi

### <a name="incentives-calculation"></a>Calcolo degli incentivi

Gli incentivi vengono calcolati in base ai **ricavi fatturati**, ai **ricavi *non* corretti**. I pagamenti degli incentivi realizzati verranno visualizzati in base ai nostri criteri disponibili nelle nostre guide agli incentivi CSP.

Quando viene venduta una sottoscrizione fatturata annualmente, i ricavi di tale sottoscrizione vengono riconosciuti per il calcolo degli incentivi in base ai ricavi fatturati.

### <a name="payout"></a>Proventi

Attualmente, tutti i pagamenti incentive vengono eseguiti due volte all'anno. 45 giorni dopo la fine del semestre.

### <a name="rates"></a>Rates

I partner ottengono incentivi per tutte le transazioni idonee, indipendentemente dalla fatturazione di una sottoscrizione. I guadagni degli incentivi vengono calcolati in base al tasso di incentivo globale (applicato ai ricavi fatturati per il periodo), all'acceleratore locale (per tutte le aree geografiche in cui sono presenti acceleratori locali) ed eventuali campagne globali (ove applicabile).

### <a name="contacts"></a>Contatti

Per domande sugli incentivi, contattare il team di supporto tecnico per gli incentivi regionali appropriato:

| Area | Indirizzo di posta elettronica |
| ------ | ------------- |
| America del Nord | <ocina@microsoft.com> |
|America Latina & Brasile | <ocilatam@microsoft.com> |
| EMEA | <ociemea@microsoft.com> |
| APOAC (escluso il Giappone) | <ociapgc@microsoft.com> |
| Giappone | <ocijp@microsoft.com> |


### <a name="suspension"></a>Sospensione

Se si sospende una sottoscrizione, nel centro per i partner o tramite le API, entro 30 giorni dall'acquisto, si riceverà un credito del 100%, indipendentemente dalla frequenza di fatturazione.

Per la fatturazione annuale:

1. Il partner Acquista la sottoscrizione il 1 ° gennaio. Viene creata una linea di fatturazione addebitata per il periodo di servizio dal 1 ° gennaio al 31 dicembre.
2. Il partner sospende la sottoscrizione il 25 gennaio. Viene creata una linea di fatturazione del credito per il periodo di servizio dal 1 ° gennaio al 31 dicembre.
3. Il partner riattiva la sottoscrizione il 29 gennaio. Viene creata una linea di fatturazione di addebito per il periodo di servizio dal 29 gennaio al 31 dicembre.

Per la fatturazione mensile:

1. Il partner Acquista la sottoscrizione il 1 ° gennaio. Viene creata una linea di fatturazione addebitata per il periodo di servizio dal 1 ° gennaio al 31 gennaio.
2. Il partner sospende la sottoscrizione il 25 gennaio. Viene creata una linea di fatturazione del credito per il periodo di servizio dal 1 ° gennaio al 31 gennaio.
3. Il partner riattiva la sottoscrizione il 29 gennaio. Viene creata una linea di fatturazione di addebito per il periodo di servizio dal 29 gennaio al 31 gennaio.
