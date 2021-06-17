---
title: Come vendere offerte ai clienti dell'istruzione
description: Informazioni su come creare un cliente del settore dell'istruzione e vendere offerte in Partner Center. Include la conferma dello stato di verifica per il cliente dell'istruzione.
ms.topic: how-to
ms.date: 12/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: alikhaki
ms.author: alikhaki
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9d0cff4883e084ccc0acb37d8c3119d91e3f5530
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276451"
---
# <a name="how-to-sell-offers-to-education-customers-and-how-to-create-an-education-customer-in-partner-center"></a>Come vendere offerte ai clienti dell'istruzione e come creare un cliente dell'istruzione in Partner Center

**Ruoli appropriati:** Amministratore globale | Agente amministratore | Agente di vendita

## <a name="create-an-education-customer"></a>Creazione di un cliente Education

Questo articolo illustra come creare un cliente del settore Partner Center e vendere prodotti per l'istruzione. Illustra anche come visualizzare lo stato della verifica e inviare nuovamente la richiesta di verifica, se necessario. Le offerte Education sono **attualmente disponibili solo per i** servizi basati su licenza, ad esempio Microsoft 365, Dynamics, Intune e così via. Non è disponibile per altri tipi (sottoscrizioni software, software perpetuo o prodotti Azure).

> [!IMPORTANT]
> Microsoft verifica ogni tenant del cliente education appena creato per assicurarsi che siano qualificati per le offerte di formazione.  Assicurarsi di immettere le informazioni necessarie nel modo più accurato e completo possibile per evitare ritardi nel processo di verifica.

1. Accedere al Centro per i partner.

2. Selezionare **Customers** (Clienti) e **quindi Add a customer (Aggiungi cliente).** Selezionare **Education (Istruzione)** **nell'elenco a discesa Special qualifications (Qualifiche** speciali).  Compilare il resto delle informazioni sull'account in base alle esigenze.  I campi chiave che assiste il processo di verifica includono:

   - **Nome società:** IMMETTERE IL NOME DELL'ENTITÀ LEGALE - Obbligatorio per la verifica
   - **Country/region and Address lines (Paese/area geografica e indirizzo):** IMMETTERE L'INDIRIZZO POSTALE COMPLETO DELL'ENTITÀ : obbligatorio per la verifica
   - **Indirizzo di posta elettronica:** immettere il messaggio di posta elettronica di proprietà dell'entità, non un indirizzo on.microsoft.com gratuito, necessario per la verifica
   - **Informazioni di contatto del** cliente: questi dettagli verranno usati come parte del processo di verifica
   - **Nome di dominio primario:** usato per creare l'account e gli indirizzi di posta elettronica del cliente.  Scegliere un nome simile al nome della società senza spazi o caratteri speciali.  Questo nome non può essere modificato in un secondo momento.

3. Al termine, selezionare **Rivedi**.

   :::image type="content" source="images/eduaccountinfo.png" alt-text="Account del cliente education.":::

4. Dopo la conferma **di Revisione,** si riceverà lo stato **InReview** se le informazioni inviate sono valide. 

    :::image type="content" source="images/edu/create-review.png" alt-text="Account del cliente education in revisione."lightbox="images/edu/create-review-expanded.png":::

### <a name="confirm-your-education-customers-verification-status"></a>Confermare lo stato di verifica del cliente dell'istruzione

Nella pagina Account del **cliente** vedere **Stato qualifica speciale**.
Esempi di stato:

- Se il cliente ha superato la verifica: Education

   :::image type="content" source="images/edupassedvetting.png" alt-text="La verifica dell'istruzione è riuscita.":::

- Se il cliente non ha superato la verifica: non un cliente dell'istruzione

   :::image type="content" source="images/edu/fail-reason.png" alt-text="La verifica dell'istruzione non è riuscita." lightbox="images/edu/fail-reason-expanded.png":::

- Se il cliente non è stato contrassegnato come cliente education: Nessuno

   :::image type="content" source="images/edu/account-one.png" alt-text="il cliente dell'istruzione non è contrassegnato come tale." lightbox="images/edu/account-one-expanded.png":::

- Se il cliente è in revisione come cliente di Education: In revisione

    :::image type="content" source="images/edu/in-review.png" alt-text="il cliente dell'istruzione è in revisione." lightbox="images/edu/in-review-expanded.png":::

## <a name="correct-the-customer-account-info-and-resubmit-for-verification"></a>Correggere le informazioni dell'account del cliente e inviare di nuovo per la verifica

Se il cliente non supera la verifica iniziale, è ora possibile correggere le informazioni e inviarle di nuovo.

### <a name="correct-the-customer-account-information"></a>Correggere i dati dell'account del cliente

Per aggiornare le informazioni del cliente, è necessario disporre dei privilegi di amministratore globale. Le informazioni vengono aggiornate nel portale di Office 365 perché questi dati non possono essere aggiornati dal portale Partner Center dati.

1. Nella pagina **Account** verranno visualizzate informazioni che informano che la qualifica del cliente è considerata "Non un cliente dell'istruzione".

2. Aggiornare il browser per reimpostare la pagina. Sarà presente un **pulsante Aggiorna** e lo stato delle **qualifiche speciali** è impostato su **Nessuno.**

3. Selezionare **Aggiorna**. Nella pagina **Gestione dei** servizi selezionare **Office 365**.

4. Si verrà reindirizzati all'interfaccia di amministrazione di Office 365 in una nuova scheda del browser. Potrebbe essere richiesto di accedere con le proprie credenziali.

5. Selezionare **Impostazioni**.

6. Selezionare la **scheda Profilo organizzazione** nella parte superiore della schermata e quindi Informazioni **sull'organizzazione**. È ora possibile aggiornare i dettagli del cliente.

7. Selezionare **Salva modifiche** nella parte inferiore della barra laterale.  

### <a name="resubmit-for-verification"></a>Inviare di nuovo per la verifica

1. Passare alla scheda Partner Center e alla pagina **Account** cliente. Aggiornare il browser e verificare che la pagina Società sia stata aggiornata alle nuove informazioni. Selezionare **il pulsante** Aggiorna per richiedere di nuovo la verifica dell'istruzione.

2. Se i dettagli aggiornati del cliente sono idonei per le offerte Education, verranno visualizzati i requisiti **speciali** aggiornati a **Education.** Se viene ancora visualizzato **Non un cliente di Education,** contattare il supporto tecnico per la verifica manuale.

## <a name="next-steps"></a>Passaggi successivi

- [Vendere in settori specializzati](get-special-pricing-for-offers.md)

- [Aggiungere un nuovo cliente](add-a-new-customer.md)

- [Vendere le sottoscrizioni Minecraft: Education Edition ai clienti del settore istruzione](minecraft-subscriptions.md)
