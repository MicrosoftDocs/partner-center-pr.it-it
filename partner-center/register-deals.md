---
title: Registrare le trattative
ms.topic: article
ms.date: 06/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Quando si registra un'offerta vinta in Partner Center, Microsoft offre altre opportunità in futuro.
author: rajap-ms
ms.author: rajap
ms.localizationpriority: medium
ms.openlocfilehash: eaa9bb6f8e57033669ef584e7c52c0d050a532e0
ms.sourcegitcommit: 8235c89e789cdb5115fc1c19151fa8e97c743fe5
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/30/2021
ms.locfileid: "113080665"
---
# <a name="register-deals-youve-won-in-partner-center"></a>Registrare le offerte vinte in Partner Center

**Ruoli appropriati:** Amministratore delle segnalazioni

Puoi registrare le trattative che sono andate a buon fine nel Centro per i partner fornendo altre informazioni sul contratto. Queste informazioni consentono di offrirti maggiori opportunità in futuro.

Esistono due percorsi che portano alla registrazione della trattativa:

- È stato creato un nuovo accordo nella sezione Opportunità di **co-selling** e l'accordo soddisfa i criteri per la registrazione dell'offerta.
- Si vuole segnalare un contratto ISV Connect chiuso, che non è stato co-venduto con Microsoft.

## <a name="register-a-deal-originating-from-a-co-sell-opportunity"></a>Registrare un'offerta originata da un'opportunità di co-selling

Se si sta cercando di registrare un'offerta originata da un'opportunità di co-selling, l'accordo deve soddisfare i requisiti di idoneità seguenti:

- Il tipo di trattativa è co-selling o partner(si è scelto di consentire ai venditori Microsoft di visualizzare l'offerta).
- Nell'offerta è presente almeno una soluzione idonea per gli incentivi. Una soluzione è idonea per gli incentivi se contiene almeno uno dei tag seguenti:
  - Co-selling ip di Azure
  - Business Applications Premium
  - Business Applications Standard
- Lo stato dell'accordo è "Won".
- Se il tipo di trattativa è co-selling, Microsoft deve aver accettato l'invito o contrassegnato come vinto. È possibile visualizzare lo stato di Microsoft esaminando la scheda Microsoft sotto i dettagli dell'offerta.

Se sono stati soddisfatti i requisiti di idoneità, verrà automaticamente richiesto  di registrare l'accordo con un pulsante Registra ora visualizzato sulla barra di stato dell'offerta:

:::image type="content" source="images/register-deals.png" alt-text="Screenshot che mostra l'indicatore di stato dell'offerta.":::

> [!NOTE]
> Se **l'elemento di registrazione** deal non viene visualizzato nell'indicatore di stato dell'operazione, l'operazione non soddisfa tutti i requisiti per la registrazione dell'offerta.

Dopo aver fatto clic su **Registra** ora, si verrà reindirizzati alla pagina Deal Registration (Registrazione trattative) e verrà richiesto di compilare un modulo con le informazioni precompilato per il cliente e la soluzione. Compilare il modulo usando le istruzioni seguenti e fare clic su **Registra**.

Al momento della registrazione, verranno creati uno o due record di registrazione delle trattative a seconda della soluzione.

- Se la soluzione è idonea per ISV Connect, verrà creato un record di registrazione dell'offerta ISV Connect. Questo record di registrazione dell'offerta verrà usato per la fatturazione.
- Se la soluzione è idonea per gli incentivi di co-selling IP, verrà creato un record di registrazione dell'offerta di co-selling IP. Questo record di registrazione dell'offerta verrà esaminato e approvato o rifiutato dal team di revisione delle trattative di co-selling.

## <a name="report-a-closed-isv-connect-deal"></a>Segnalare un contratto ISV Connect chiuso

Per segnalare un'offerta ISV Connect chiusa, passare alla scheda **Registrazione** dell'offerta e fare clic su + Segnala l'offerta **ISV Connect chiusa.** Compilare i campi obbligatori e fare clic su **Registra**. Questo record di registrazione dell'offerta verrà usato per la fatturazione.

## <a name="fill-out-the-deal-registration-form"></a>Compilare il modulo di registrazione dell'offerta

> [!NOTE]
> È possibile filtrare le offerte in base al nome del cliente, allo stato e al tipo di trattativa. A tale scopo, fare clic **sul pulsante** Filtro nella parte superiore della pagina Deal Registration (Registrazione trattative).

Sia che si sia verificata la registrazione da un'opportunità di co-selling o si sta segnalando un contratto ISV Connect chiuso, che non è stato co-venduto con Microsoft, verrà richiesto di compilare i campi seguenti nel modulo di registrazione dell'offerta.

- **Dettagli cliente:** immettere **il nome della società** per il cliente e selezionare il **paese/area geografica.** Immetti quindi i valori appropriati nei campi **Città** e **Stato/provincia**.
- **Soluzione:** selezionare la soluzione che verrà usata per l'operazione. Se la soluzione appropriata non è elencata, contatta il supporto tecnico.
- **Tipo di contratto:** specificare se l'accordo è un **nuovo** contratto o un **rinnovo** di un contratto precedente.
- **Valore totale del contratto:** valore totale previsto per l'engagement. Questo valore deve includere tutti i costi del software e del servizio, ma non i costi hardware. Assicurati di selezionare la valuta appropriata.
- **Valore della** soluzione: valore totale della soluzione cloud che verrà usata per l'operazione. Ricordati di includere tutti i costi associati al software e alla manutenzione, ma non includere le voci rimborsabili, le tariffe di personalizzazione non ricorrenti o le tariffe di licenze CSP direttamente associate e pagate da Microsoft.
- **La soluzione verrà distribuita in Azure? In caso contrario, scegliere Altro**: selezionare **Azure** o **Altro.**
- **L'utilizzo della soluzione verrà eseguito** nel tenant partner o nel tenant del cliente? : selezionare il tenant **Customer** o **partner.**
- **Data di inizio del** contratto: data di inizio del contratto. Per le trattative con pagamento in base al pagamento (PAYG), usare la data della prima fattura. Per impostazione predefinita, Partner Center consente di immettere una data di inizio precedente alla data di firma del contratto. Ciò può influire su alcune trattative, ad esempio le distribuzioni IP che iniziano prima della data di firma. Per immettere correttamente queste trattative, usare la data di firma del contratto sia per i campi **della** data di firma che della data di inizio durante l'invio. Il contratto deve indicare in modo esplicito la durata dell'operazione in modo che l'ACV possa essere calcolato correttamente.
- **Data di fine contratto:** se il contratto terminerà in una data specifica, selezionare **Ha una data di fine** e specificare tale data. Se il contratto non ha una data di fine specifica, selezionare **Perpetuo.** Per le trattative con pagamento in base al pagamento (PAYG), usare la data dell'ultima fattura o più recente.
- **Data di firma del** contratto: data in cui il contratto finale è stato firmato dall'organizzazione e dal cliente. Per le trattative con pagamento in base al pagamento (PAYG), usare la data della prima fattura.
- **Contatto di registrazione:** **nome,**  **cognome,** numero  di telefono e indirizzo di posta elettronica per una persona dell'organizzazione che può essere contattata se sono necessari altri dettagli su una delle informazioni fornite qui.

Dopo aver completato tutte le sezioni della pagina, fare clic su **Registra**.

- Se l'accordo è un contratto ISV Connect, si noterà che lo stato dell'offerta è "Inviato, Completato". Non sono necessarie altre azioni per questo record di registrazione dell'offerta. Questo record verrà usato per la fatturazione.
- Se l'accordo è un accordo di co-selling IP, si noterà che lo stato dell'offerta è "Inviato". Il team di revisione delle trattative di co-selling Microsoft rivedrà le informazioni fornite in questo record di registrazione dell'offerta. Il team di revisione richiederà più azioni all'utente, se necessario, o approverà/rifiuterà direttamente l'accordo.
- Se si registra un'offerta originata da un'opportunità di co-selling e si vede che sono stati creati due record di registrazione dell'offerta, significa che la soluzione per l'offerta è idonea sia per ISV Connect che per il co-selling IP. Il record ISV Connect verrà utilizzato per la fatturazione. Il record di co-selling IP verrà esaminato dal team di convalida delle trattative di co-selling.

