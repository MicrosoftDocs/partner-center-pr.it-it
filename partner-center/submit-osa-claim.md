---
title: Creare un'associazione cliente
ms.topic: article
ms.date: 10/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: Creare associazioni dei clienti con il modello Claiming Partner of Record (CPOR). Consente di gestire vendite, utilizzo e incentivi per Microsoft 365 & clienti di Dynamics 365.
author: MalloryPrincipe
ms.author: mallp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9526a47d0b6d734bde48f403c11fa84d734511c1
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856101"
---
# <a name="customer-associations-via-the-claimed-partner-of-record-cpor-model-for-microsoft-365-and-dynamics-365"></a>Associazioni dei clienti tramite il modello Partner of Record richiesto (CPOR) per Microsoft 365 e Dynamics 365


**Ruoli appropriati:** Amministratore incentivi

Il 1° ottobre 2019 Microsoft ha iniziato a usare il modello Claiming Partner of Record (CPOR) per gestire le associazioni con i clienti di Microsoft 365 e Dynamics 365 in relazione agli incentivi online services advisory (OSA) Sell, Online Services Usage (OSU) -Microsoft 365 e OSU-Business Application.

>[!Important]
> Le attestazioni CPOR (Customer Association) si applicano solo ai programmi di incentivi Online Services Advisory (OSA) Sell, Online Services Usage (OSU) -Microsoft 365 e OSU-Business Application. Se si invia un'attestazione co-op per un altro programma, ad esempio Cloud Solution Provider, Managed Reseller, Hosting o Surface, fare riferimento al processo di attestazioni co-op descritto qui. <br><br>Quando si invia l'attestazione, Microsoft la convalida. A questo punto è possibile richiedere altre informazioni. Invieremo anche una notifica al cliente della richiesta di associazione. I clienti hanno cinque giorni lavorativi per rifiutare esplicitamente. Se non rifiutano esplicitamente, l'associazione con questo tenant e carico di lavoro specifici sarà ufficiale. A questo punto si ha accesso ai dati di utilizzo del cliente. 

Per completare un'attestazione, sono necessarie le informazioni seguenti:

- ID **MPN per** l'entità che effettua l'attestazione

- Nome di dominio **del cliente Trovare** [questo](find-ids-and-domain-names.md)

- ID directory o **ID** **tenant del cliente** Trovare [questo](find-ids-and-domain-names.md)

- Area **della soluzione**, ad esempio Business Applications o Microsoft 365

- Attività **eseguita** e tipo di attestazione da effettuare, ad esempio associazione pre-vendita, utilizzo o ricavi

- Nome, titolo e indirizzo di **posta elettronica** del contatto del cliente

- Per Dynamics 365, è anche necessario  specificare il nome, il titolo e l'indirizzo di posta elettronica del contatto tecnico del cliente

- Nome e indirizzo di posta elettronica del **contatto dell'azienda**

- Si creerà un nome **per** questa attestazione

- I **prodotti o i** carichi di lavoro che si stanno rivendicando

- **Proof of Execution (PoE),** ad esempio un'istruzione di lavoro firmata dal cliente. È anche possibile scaricare un modello PoE da usare.

- Solo per i partner che dichiarano l'associazione di ricavi: nome del venditore della soluzione **Dynamics,** **Nome cliente** e Nome **del prodotto/soluzione ISV.** 

È anche necessario comprendere i punti seguenti:

- Se sono già Microsoft 365 clienti, è necessario riassumere l'associazione con quelli che si vogliono continuare a ottenere incentivi OSU usando questo processo.

- Se sono esistenti associazioni con i clienti dynamics 365 o Power BI, queste associazioni rimarranno valide fino alla scadenza delle sottoscrizioni.

- Un cliente può avere più partner, ma ogni carico di lavoro (per OSU-Microsoft 365) o sottoscrizione (per le applicazioni OSA-Sell e OSU-Business) può essere associato a un solo partner.

## <a name="create-a-customer-association"></a>Creare un'associazione cliente

1. Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard/).

2. Selezionare la **scheda Incentivi,** selezionare **Panoramica** e quindi Selezionare **Associazioni clienti**.

3. Nella parte superiore della pagina Associazioni dei clienti selezionare **+ Associazione clienti**.

4. Selezionare l'**ID MPN** della località partner da associare al cliente, quindi aggiungere il nome di dominio e l'ID directory del cliente. [Trova questo](find-ids-and-domain-names.md)

5. Selezionare **Continua**.

6. Selezionare **l'area Soluzione** e **l'attività**. 

   >[!Note]
   >
   >Se si seleziona Business Applications, selezionare Utilizzo **e/o Pre-vendita** o Associazione **ricavi** e quindi **selezionare Continua.** 
   <br><br>Se si seleziona Associazione ricavi, verranno richieste informazioni leggermente diverse da quelle elencate di seguito.

7. Immettere le informazioni appropriate nella pagina **Associa cliente** e quindi selezionare **Crea attestazione**.

8. Selezionare i prodotti associati a questa associazione di clienti e quindi **selezionare Continua.**

9. Completare le informazioni di contatto del cliente e le informazioni di contatto della società. Tutti i campi sono obbligatori. 

   >[!NOTE]
   >Se il prodotto è Dynamics 365 e il prodotto scelto ha più sottoscrizioni per questo particolare cliente, è anche necessario immettere l'ID sottoscrizione.

10. Fornire la prova di esecuzione (PoE). È possibile trascinarla nella casella, passare alla propria documentazione di supporto o usare un modello selezionando **Scarica modello**. 

11. Aggiungere e salvare i commenti se lo si desidera, quindi selezionare **Invia attestazione**. Invieremo un messaggio di posta elettronica al cliente per richiedere l'approvazione dell'associazione del cliente.

   >[!NOTE]
   >Dopo aver inviato l'associazione del cliente, non è possibile modificarla.

Lo stato dell'associazione del cliente viene visualizzato nel campo **stato**.

Selezionare **Cronologia** per visualizzare la cronologia di un'associazione del cliente.

## <a name="next-steps"></a>Passaggi successivi

- [Gestire le associazioni del cliente](incentives-manage-customer-associations.md)