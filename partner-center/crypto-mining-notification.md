---
title: Notifica per l'attività di data mining
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su ciò che significa quando viene visualizzata una notifica relativa al potenziale data mining criptovalute (o Crypto mining) in una o più sottoscrizioni di Azure.
author: aarzh-AaronZhang
ms.author: v-aarzh
robots: noindex, nofollow
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d691ef30bf01fcb25d686649291e92cfec47f100
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/17/2020
ms.locfileid: "86435200"
---
# <a name="partner-center-notification-for-cryptocurrency-mining-activity"></a>Notifica del centro partner per l'attività di data mining criptovalute

**Si applica a**

-  Centro per i partner
-  Partner CSP

È possibile che sia stata ricevuta la seguente notifica al centro per i partner di criptovalute mining:

:::image type="content" source="images/crypto1.png" alt-text="Immagine della notifica di sicurezza nel centro per i partner":::

Lo scopo di questa notifica è informare che è stata rilevata la criptovalute mining in una o più sottoscrizioni di Azure nell'ultima settimana. Criptovalute mining non è necessariamente uguale all'attività fraudolenta. Tuttavia, è insolito perché il costo di esecuzione di criptovalute mining in Azure tende a superare i potenziali premi finanziari.

## <a name="checklist"></a>Elenco di controllo

Per la protezione da frodi finanziarie che potrebbero influisca sull'utente o sul cliente, tenere presente i passaggi seguenti:

1. Verificare e verificare che l'account del cliente sia in grado di essere valido. È possibile accedere direttamente alla sottoscrizione facendo clic sulla notifica.

2. Esaminare i modelli di utilizzo di Azure per la sottoscrizione. I picchi improvvisi possono suggerire attività impreviste.

3. Contattare il cliente per verificare che l'attività sia prevista.

   Se è prevista l'attività, tornare alla pagina dei dettagli della sottoscrizione di Azure del cliente e verificare che il criptovalute mining sia legittimo.

   :::image type="content" source="images/crypto2.png" alt-text="Immagine della pagina dei dettagli della sottoscrizione di Azure del cliente":::

## <a name="steps-for-unexpected-activity"></a>Passaggi per un'attività imprevista

Se l'attività è imprevista, tenere presente quanto segue:

1. Verificare che le risorse di Azure per il data mining criptovalute non siano necessarie ed eliminarle per evitare ulteriori addebiti per Azure.

2. Comprendere il modo in cui le risorse sono state create in precedenza. Potrebbe essere necessario esaminare i log di Azure Resource Manager per le attività di provisioning delle risorse.

3. Se è necessario scoprire chi ha creato la sottoscrizione, esaminare i log attività del centro per i partner.

Il rilevamento delle attività di data mining criptovalute è basato su euristica e non può essere accurato al 100%. Assicurarsi di disporre di sistemi di governance e monitoraggio sul posto per proteggersi da attività fraudolente o da altre attività non consentite. Per ulteriori informazioni, vedere [non pagamento, frode o utilizzo improprio](https://docs.microsoft.com/partner-center/non-payment--fraud--or-misuse).

## <a name="contact-support-if-needed"></a>Se necessario, contattare il supporto tecnico

In caso di domande o dubbi sulla notifica, è possibile utilizzare la procedura seguente per aprire una richiesta di supporto.

1. Nel centro per i partner selezionare **supporto** e quindi selezionare **le richieste del centro**per i partner.

2. Selezionare **nuova richiesta**. 

3. Nel menu a discesa **tipo di problemi** selezionare **aggiunta o gestione clienti**.

4. Nel menu a discesa **Impact** selezionare **moderata**.

5. Nel campo **titolo** , immettere **notifica di data mining**.

6. Nel campo **Descrizione** immettere il nome della sottoscrizione interessata insieme ad altre domande o problemi.

7. Immettere le informazioni di contatto.

8. Selezionare **Submit** (Invia).
