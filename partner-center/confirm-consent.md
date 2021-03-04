---
title: Confermare l'accettazione del Contratto del cliente Microsoft da parte di un cliente
description: Scopri come confermare l'accettazione del contratto del cliente Microsoft da parte di un cliente. Questa operazione potrebbe essere necessaria per ordinare prodotti e servizi Microsoft per i clienti.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/02/2021
ms.openlocfilehash: ab2f5be77f6480b4a8b47bef0e0fd5096f7c1776
ms.sourcegitcommit: a7897284b79abb1ceeee79deb3a87b72d59900dc
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/04/2021
ms.locfileid: "102029917"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a>Confermare l'accettazione del contratto del cliente Microsoft da parte di un cliente


**Ruoli appropriati**

- Agente amministratore
- Agente di vendita

> [!NOTE]
> La risorsa Contratto è attualmente supportata dal Centro per i partner solo nel cloud pubblico Microsoft. Non è applicabile a:
> * Centro per i partner gestito da 21Vianet
> * Centro per i partner per Microsoft Cloud Germania
> * Centro per i partner per Microsoft Cloud for US Government


In qualità di partner, devi ottenere l'accettazione del Contratto del cliente Microsoft da parte di un cliente prima di poter ordinare prodotti e servizi Microsoft per tale cliente. Per aiutare meglio i partner a soddisfare i requisiti di conformità, Microsoft richiede ai partner di confermare l'accettazione fornendo i seguenti dettagli riguardanti la persona che ha accettato il contratto:

- Nome

- Cognome

- Indirizzo di posta elettronica

- Numero di telefono (facoltativo)

- Data di accettazione

I partner con fatturazione diretta e i provider indiretti devono confermare che un cliente ha accettato il Contratto del cliente Microsoft durante l'esecuzione della transazione tramite il Centro per i partner o la relativa API. La conferma è *obbligatoria*.

>[!NOTE]
>A partire dal 31 gennaio 2020, tutti i clienti (sia nuovi che già esistenti) devono firmare il nuovo Contratto del cliente Microsoft. Per altre informazioni, vedi [Confermare l'accettazione del Contratto del cliente Microsoft da parte di un cliente](confirm-customer-agreement.md).

Se non viene fornita la conferma per un determinato cliente:

- Non sarai in grado di creare nuovi ordini per il cliente.

- Non sarà possibile modificare il numero di licenze degli abbonamenti esistenti basati su licenze per il cliente.

La conferma dell'accettazione da parte del cliente può essere eseguita tramite il Centro per i partner o la relativa API. Per eseguire questa operazione tramite l'API del Centro per i partner, vedi i seguenti argomenti:

- [Ottenere la conferma del consenso del cliente](/partner-center/develop/get-confirmation-of-customer-consent)

- [Ottenere i metadati del contratto](/partner-center/develop/get-agreement-metadata)

- [Confermare il consenso del cliente](/partner-center/develop/confirm-customer-consent)

Questo vale sia per gli ambienti di produzione che per quelli sandbox.

## <a name="confirm-customer-acceptance-for-a-new-customer"></a>Confermare l'accettazione da parte di un nuovo cliente

Usa la procedura seguente per confermare l'accettazione da parte del cliente durante la creazione di un nuovo tenant cliente nel Centro per i partner. Devi essere un agente amministratore o di vendita per eseguire questa operazione.

1. Seleziona **Clienti**, quindi **Nuovo cliente** e infine **Info account**.

2. Immetti le informazioni nei campi **Società** e **Contatto principale**.

   :::image type="content" source="images/mca/mca1.png" alt-text="Informazioni sulla società":::

3. In **Microsoft customer agreement** (Contratto del cliente Microsoft) seleziona **The customer has accepted the latest Microsoft customer agreement** (Il cliente ha accettato il Contratto del cliente Microsoft più recente).

4. In **Agreement acceptance date** (Data di accettazione del contratto) immetti la data appropriata. Non puoi impostare questo campo su una data futura.

5. Immetti i dettagli dell'utente che ha fornito l'accettazione.

   :::image type="content" source="images/mca/MCA3.png" alt-text="Aggiunta della data di accettazione":::

   Per impostazione predefinita, vengono visualizzate le informazioni utente relative al contatto principale. Se queste informazioni non sono corrette, fai clic su **Aggiorna**, quindi riempi i campi **Nome**, **Cognome**, **Indirizzo e-mail** e **Numero di telefono* (facoltativo) della persona che ha accettato il contratto.

6. Scegli **Avanti** per continuare con i passaggi rimanenti per la creazione del tenant del cliente.

## <a name="confirm-customer-acceptance-for-an-existing-customer"></a>Confermare l'accettazione da parte di un cliente esistente

Devi essere un agente amministratore o di vendita per eseguire questa operazione.

1. Seleziona **Clienti** e quindi individua e seleziona il cliente che vuoi visualizzare.

2. Seleziona **Informazioni sull'account**.

3. In **Microsoft customer agreement** (Contratto del cliente Microsoft) fai clic su **Aggiorna**.

   :::image type="content" source="images/mca/mca4.png" alt-text="Aggiornamento":::

4. Riempi i campi **Nome**, **Cognome**, **Indirizzo e-mail** e **Numero di telefono** (facoltativo) dell'utente che ha accettato il contratto.

5. In **Agreement acceptance date** (Data di accettazione del contratto) immetti la data appropriata. Non puoi impostare questo campo su una data futura.

6. Fai clic su **Salva e continua**.

## <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>Confermare l'accettazione da parte del cliente durante la creazione di un nuovo ordine per un cliente esistente

Se si tenta di creare un nuovo ordine per un cliente esistente non confermato prima, si riceverà la richiesta di completare la conferma. Utilizzare la procedura seguente per eseguire questa operazione.

1. Riempi i campi **Nome**, **Cognome**, **Indirizzo e-mail** e **Numero di telefono** (facoltativo) dell'utente che ha accettato il contratto.

2. In **Agreement acceptance date** (Data di accettazione del contratto) immetti la data appropriata. Non puoi impostare questo campo su una data futura.

3. Fai clic su **Salva e continua**.

## <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>Recuperare la conferma dell'accettazione da parte di un cliente esistente

Puoi recuperare la conferma dell'accettazione da parte di un cliente esistente che hai fornito in precedenza usando la procedura seguente. Devi essere un agente amministratore o di vendita per eseguire questa operazione.

1. Seleziona **Clienti** e quindi individua e seleziona il cliente che vuoi visualizzare.

2. Seleziona **Informazioni sull'account**.

3. In **Microsoft customer agreement** (Contratto del cliente Microsoft) potrai vedere se la conferma è stata fornita o meno per tale cliente.

## <a name="next-steps"></a>Passaggi successivi

- [Conferma dell'accettazione del contratto del cliente Microsoft da parte di un cliente nel programma per i partner CSP](confirm-customer-agreement.md)

- [Attestare l'accettazione del Contratto del cliente Microsoft per conto di un cliente](attest-acceptance-customer-agreement.md)