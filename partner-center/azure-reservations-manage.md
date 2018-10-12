---
title: Gestire le prenotazioni di Azure per conto del cliente | Centro per i partner
Description: Purchasing and managing Azure reservations on behalf of your customers.
author: v-petand
keywords: Azure, prenotazioni, gestire, fatturazione, acquisto
ms.localizationpriority: medium
ms.openlocfilehash: 6b3fb1aed57b39976556851c007590743a805671
ms.sourcegitcommit: 1321f23b1a5be48a0a5dae6d52fd123ec9bacee2
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/12/2018
ms.locfileid: "4562273"
---
# <a name="manage-microsoft-azure-reservations-on-behalf-of-your-customers"></a>Gestire le prenotazioni di Microsoft Azure per conto del cliente

**Ambito di applicazione:**

-  Centro per i partner
-  Portale di Microsoft Azure
-  Partner di CSP

Per gestire gli post-acquisti di prenotazioni di Azure dei tuoi clienti, verrà seleziona il cliente e la prenotazione che desideri gestire nel centro per i Partner e quindi apportare le modifiche alla prenotazione nel portale di Azure. 

1. Per iniziare, seleziona **clienti** dal menu del centro per i Partner e quindi seleziona il cliente di cui si desidera gestire le prenotazioni. 

2. Dal menu della pagina dei dettagli del cliente seleziona **prenotazioni di Azure** e quindi seleziona la prenotazione specifica che desideri gestire.  

3. In **Azioni** seleziona **Gestisci** per passare al record della prenotazione del cliente nel portale di Azure. Nella pagina dei dettagli della prenotazione segui i passaggi qui sotto per completare le attività.  

| **Seleziona**   | **Per**    |
|:-----------------------------|:-----------------|
| **Panoramica**   | Visualizzare i dettagli della prenotazione di un cliente, inclusi i dati di utilizzo, l'ambito e la data di scadenza. **NOTA:** seleziona **Rimborsa** per creare una richiesta di supporto per un rimborso proporzionale. Selezionare **Cambio** per creare una richiesta di supporto in vista del cambio del periodo di prenotazione non utilizzato.  
| **Controllo di accesso (IAM)**   | Gestire l'accesso alle informazioni sulla prenotazione del cliente.|
| **Configurazione**   | Modificare l'ambito della prenotazione e/o la sottoscrizione di Azure a cui è associata la prenotazione.    |
| **Proprietà**   | Visualizzare le proprietà della prenotazione e copiare negli Appunti l'ID della prenotazione e l'ID dell'ordine di prenotazione. **NOTA:** quando chiedi supporto per conto di un cliente, ti potrebbero essere richiesti l'ID della prenotazione e l'ID dell'ordine di prenotazione.    |
| **Nuova richiesta di supporto**    | Richiedere assistenza al Supporto tecnico Microsoft.   |
 
## <a name="cancel-or-exchange-a-reservation"></a>Annullare o cambiare una prenotazione 
In seguito al cambiamento delle esigenze aziendali, i tuoi clienti potrebbero voler annullare una prenotazione o modificare l'importo del rimborso proporzionale per pagare una nuova prenotazione. 

**Come funzionano gli annullamenti**

I clienti possono annullare una prenotazione in qualsiasi momento (fino a $ 50.000 all'anno). L'annullamento consente al cliente di restituire i mesi rimanenti di una prenotazione di Azure a Microsoft dietro il pagamento di una quota per la risoluzione anticipata. Il saldo proporzionale rimanente, al netto della quota versata per la risoluzione anticipata, verrà rimborsato al cliente. 

Vedi di seguito per tariffe e i dettagli di annullamento.

|**Data annullamento**<br> (giorni)   |**Usage**    |**Credito**  |**Prematuramente.**<br> aziendale    |**Rimborsa terminazione** | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|Meno di 5                       | No          | 100%       | No                              | $50.000 USD   |
|Meno di 5                       | Sì         | Ripartizione  | No                              | $50.000 USD   |
|Più di 5                        | No          | Ripartizione  | 12%                             | $50.000 USD   |
|Più di 5                        | Sì         | Ripartizione  | 12%                             | $50.000 USD   |


**Come funzionano gli scambi** 

Uno scambio consente al cliente di ricevere un rimborso proporzionale sulla base della durata restante della prenotazione e di utilizzare l'importo del rimborso per una nuova prenotazione.   

## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>Richiedere un rimborso o un cambio per conto di un cliente 

Per archiviare una richiesta di supporto per un rimborso o un cambio per conto dei clienti, scoprirai seleziona il cliente e la prenotazione nel centro per i Partner e quindi creare la richiesta di supporto nel portale di Azure. 

>[!NOTE]
>Gli agenti del Supporto tecnico Microsoft potrebbero richiedere l'ID della prenotazione e l'ID dell'ordine di prenotazione. Puoi trovare queste informazioni nella pagina **Proprietà** della prenotazione nel portale di Azure. 

1. Per iniziare, seleziona **i clienti** nel menu del centro per i Partner e quindi seleziona il cliente che desidera un rimborso. 

2. Nella pagina dei dettagli del cliente, seleziona **Prenotazioni di Azure**, quindi seleziona la prenotazione specifica che il cliente desidera farsi rimborsare.  

3. Nel riquadro **Azioni**seleziona **rimborso** per passare al record della prenotazione del cliente nel portale di Azure e avviare una richiesta di supporto.  

4. Nella pagina **Nuova richiesta di supporto** attieniti alla procedura seguente per richiedere un rimborso. Seleziona **Avanti** dopo ogni passaggio. 

|**Passaggio**   |**Selezioni**    |
|:-----------------------------|:-----------------|
|**1 Informazioni di base**   |Tipo di problema: fatturazione  |
|**2 Problema**   |Tipo di problema: gestione della prenotazione. Categoria: scambi e rimborsi |
|**3 Informazioni sul contatto**   |Seleziona le preferenze e immetti le informazioni necessarie. Al termine, seleziona **Crea**.   |

## <a name="azure-reservations-resources"></a>Risorse sulle prenotazioni di Azure
|**Per informazioni su**   |**Leggi**    |
|:-----------------------------|:-----------------|
|Panoramica delle prenotazioni di Azure in CSP  | [Vendere istanze prenotate Microsoft Azure](azure-reservations.md) |
|Acquisto di prenotazioni di Azure per i clienti nel centro per i Partner   |[Acquistare prenotazioni di Azure](azure-reservations-buying.md) |
|Determinare le dimensioni corrette della macchina virtuale e verificare l'utilizzo di macchine virtuali da parte dei clienti   |[Ridimensionamento della macchina virtuale per un utilizzo ottimale delle prenotazioni di Azure](azure-usage.md)   |
|Acquisto di prenotazioni di Azure mediante l'API del Centro per i partner | [Acquisto di istanze di macchina virtuale riservate di Azure](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) nella documentazione per sviluppatori del Centro per i partner

