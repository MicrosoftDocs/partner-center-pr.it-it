---
title: Ottenere il credito per la ritenuta d'acconto
ms.topic: article
ms.date: 06/05/2020
description: Ricevere credito nell'account Partner Center per la ritenuta d'acconto. Le informazioni includono i passaggi per inviare una richiesta di ritenuta d'acconto.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8674dfa337f0620b6c916f685fced9882134032a
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276366"
---
# <a name="receive-credit-on-your-partner-center-account-for-tax-withholding"></a>Ricevere credito nell'account Partner Center per la ritenuta d'acconto

**Ruoli appropriati:** Account admin | Amministratore della fatturazione

## <a name="overview"></a>Panoramica

I partner CSP in alcuni paesi ricevono gli importi delle fatture che includono le imposte. Alcuni di questi partner pagano l'autorità fiscale locale anziché Microsoft. Se si paga l'autorità fiscale locale, è necessario inviare una richiesta di ritenuta d'acconto, incluso il certificato fiscale, per cancellare l'importo fiscale dalle fatture precedenti. Questi importi cancellati vengono visualizzati nella **colonna Ultimo** pagamento nella pagina **Fatturazione** Partner Center.

Partner usati per inviare richieste di ritenuta d'acconto creando richieste di servizio (ticket di supporto partner) in Partner Center. Questo processo è stato modificato a gennaio 2020. A questo punto, i partner CSP devono inviare richieste di ritenuta d'acconto nella **pagina Fatturazione** anziché creare richieste di supporto.

> [!IMPORTANT]
> I partner possono inviare richieste di ritenuta d'acconto solo per **le** fatture a pagamento.

## <a name="submit-a-tax-withholding-request"></a>Inviare una richiesta di ritenuta d'acconto

Seguire questa procedura per inviare una nuova ritenuta d'acconto:

1. Accedi al [dashboard](https://partner.microsoft.com/dashboard/home) Centro per i partner.

2. Nel menu a sinistra scegliere **Fatturazione** e passare a Cronologia **fatturazione**.

3. Fare **clic su Invia** nuovo accanto alla fattura per cui si vuole inviare un'autorizzazione. Il collegamento invia nuovo verrà visualizzata la pagina Nuova richiesta di ritenuta **d'acconto.**

   :::image type="content" source="images/wht1.png" alt-text="Inviare una nuova ritenuta d'acconto per una fattura.":::

4. Esaminare i dettagli della fattura per assicurarsi di inviare la richiesta per la fattura corretta.

   :::image type="content" source="images/wht2.png" alt-text="Completare i dettagli della ritenuta d'acconto per una fattura.":::

5. Immettere il "Totale ritenuta d'acconto" in **Dettagli ritenuta d'acconto**. Il "Totale ritenuta d'acconto" è l'importo che si prevede verrà accreditato.

6. **Allegare** un certificato fiscale. È necessario includere una **copia digitale** del **certificato** di ritenuta d'acconto nella richiesta di ritenuta d'acconto. Questo certificato è stato ricevuto dall'agenzia fiscale locale quando si pagano le imposte all'autorità fiscale locale. L'importo dell'imposta sulla fattura nel certificato di ritenuta d'acconto deve corrispondere all'importo totale nella richiesta di ritenuta d'acconto.

   > [!IMPORTANT]
   > L'importo totale fornito dal partner deve corrispondere alla voce della fattura del certificato fiscale collegato. I file di certificato fiscale allegati devono essere in uno dei formati di file seguenti: .PDF o Solo immagine (. JPEG, .PNG e .GIF). Inoltre, i nomi dei file non devono contenere spazi o caratteri speciali. Le dimensioni dei file non possono superare 1 MB.

7. **Inviare** la richiesta di ritenuta d'acconto.

   Dopo l'invio, la richiesta verrà inviata al processo di approvazione in cui verrà approvata per il completamento o inviata all'utente se sono necessarie correzioni. Visualizzare l'ID richiesta e lo stato delle richieste e nella cronologia **di fatturazione** da cui è stata inviata la nuova richiesta.

   Se la richiesta viene inviata all'utente, sarà possibile modificare l'importo della ritenuta d'acconto e sostituire il certificato in caso di problemi.

## <a name="update-request-and-resubmit"></a>Richiesta di aggiornamento e nuovo invio

Il team di revisione potrebbe richiedere di apportare correzioni e inviare di nuovo una richiesta prima che possa essere approvata. Lo stato verrà modificato in **Azione partner in sospeso**. Per correggere e inviare nuovamente la richiesta:

1. Accedi al [dashboard](https://partner.microsoft.com/dashboard/home) Centro per i partner.

2. Nel menu a sinistra scegliere **Fatturazione**

3. Nella cronologia **di** fatturazione della pagina **Fatturazione** trovare la richiesta di ritenuta d'acconto. Le richieste che necessitano dell'attenzione avranno lo stato "Azione partner in sospeso".

4. Fare clic sull'ID della richiesta di ritenuta d'acconto e sullo stato che consente di accedere alla pagina della richiesta.

5. Selezionare **Aggiorna e invia di nuovo** in **Stato**.

6. Esaminare i commenti lasciati dai revisori evidenziando ciò che deve essere modificato.

7. Apportare le correzioni inviando nuovamente un certificato aggiornato o modificando gli importi della ritenuta d'acconto.

8. **Inviare** la richiesta.

L'invio della richiesta la invierà al team di revisione in cui approverà o chiederà altre modifiche.

### <a name="approved-requests"></a>Richieste approvate

Le richieste di ritenuta d'acconto approvate verranno eseguite sulla fattura successiva, con la disdegni dell'importo dovuto. Le richieste contrassegnate come **Completate** devono essere applicate entro 10 giorni lavorativi. 

Gli importi cancellati verranno visualizzati nella sezione **Cronologia di fatturazione della pagina di fatturazione**. Gli importi cancellati verranno visualizzati nella **colonna Ultimo** pagamento accanto alla fattura a cui è stata inviata la richiesta.

   > [!IMPORTANT]
   > Le fatture precedenti non vengono rigenerate o riemettete. L'importo clearace viene semplicemente applicato ai pagamenti dei mesi precedenti.

L'elaborazione delle richieste di ritenuta d'acconto dovrebbe richiedere due giorni, presupponendo che il certificato fiscale e l'importo siano corretti. Se sono necessarie modifiche, sarà necessario più tempo, a causa delle correzioni che devono essere apportate e reinvie.

Per domande sul processo di richiesta di ritenuta d'acconto, inviare un ticket al supporto tecnico per i partner. Per risolvere le domande, sarà necessario l'ID richiesta di ritenuta d'acconto.

## <a name="german-tax-withholding"></a>Ritenuta d'acconto per la Germania

I partner che inviano richieste di ritenuta d'acconto in Germania devono ricordare di inviare tramite posta elettronica copie hard del certificato di ritenuta d'acconto all'indirizzo seguente:

- ATTN: EOC Tax Team Marianne Gannon
- Centro operativo Microsoft EMEA
- One Microsoft Place,
- South County Business Park
- Leopards town, Dublino 18, Irlanda

### <a name="questions-and-assistance-for-tax-withholding-requests"></a>Domande e assistenza per le richieste di ritenuta d'acconto

I partner devono usare il nuovo processo descritto in dettaglio in precedenza per inviare nuove richieste e non usare più la creazione di richieste di supporto per le nuove richieste di ritenuta d'acconto. I partner con domande aggiuntive sulle richieste di ritenuta d'acconto possono [inviare richieste di supporto.](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?stage=2&topicid=9227afa6-babf-3917-acee-67db7860f5ed) Le richieste di supporto sono destinate ai partner per le richieste esistenti, quindi dovranno avere il proprio **ID** richiesta per inviare un nuovo ticket. Se i partner non possono inviare una richiesta usando il nuovo processo, devono immettere un numero (tutti e 1) nel modulo di richiesta di supporto. 

   > [!IMPORTANT]
   > I partner non devono contattare il supporto se lo stato della richiesta è **Completato.** Questo stato viene visualizzato nella cronologia **di fatturazione** accanto alla fattura per l'invio. **Gli importi** dell'ultimo pagamento accanto alla fattura devono riflettere l'importo della ritenuta d'acconto entro dieci giorni dal completamento della **richiesta.**
