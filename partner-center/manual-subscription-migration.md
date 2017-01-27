---
title: Migrazione delle sottoscrizioni Dynamics AX a Dynamics 365 | Centro
description: "Microsoft introduce Dynamics 365, la nuova generazione di applicazioni aziendali intelligenti che consentono l&quot;espansione, evoluzione e trasformazione della tua organizzazione per soddisfare le esigenze dei clienti esistenti e acquisire nuove opportunità."
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: MaggiePucciEvans
translationtype: Human Translation
ms.sourcegitcommit: cb3523dffbd017aa5c40e6899e1cb37be1f2a726
ms.openlocfilehash: f19e46da31a7e479ebd3b1cd368ca7646c3c55b7

---

# Migrazione delle sottoscrizioni Dynamics AX a Dynamics 365

**Si applica a**

-  Centro per i partner

Microsoft introduce Dynamics 365, la nuova generazione di applicazioni aziendali intelligenti che consentono l'espansione, evoluzione e trasformazione della tua organizzazione per soddisfare le esigenze dei clienti esistenti e acquisire nuove opportunità. Nell'ambito del nuovo prodotto, Microsoft ha introdotto nuovi piani di sottoscrizione per Microsoft Dynamics per i clienti dal 1 novembre 2016, simili ma non identici ai piani correnti.

Le istruzioni in questo documento descrivono in che modo i provider indiretti possono eseguire il passaggio delle sottoscrizioni esistenti di Microsoft Dynamics AX dei clienti ai nuovi piani per Microsoft Dynamics 365. Le istruzioni si applicano anche agli altri prodotti Microsoft aggiornati a nuove versioni, per i quali è necessario che i provider eseguano la migrazione delle sottoscrizioni dei clienti a un nuovo SKU.

**Modifiche delle licenze per Microsoft Dynamics AX**

La linea di prodotti Microsoft Dynamics AX è stata ritirata a partire dal 1 novembre 2016. Per altre informazioni sulle nuove opzioni di licenza per Dynamics 365, consulta la nuova guida per le licenze, di prossima pubblicazione. Fai riferimento alla tabella seguente per altri dettagli sul mapping delle licenze:

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Licenza di Dynamics AX ritirata</strong></p></td>
<td><p><strong>Licenza di Dynamics 365</strong></p></td>
</tr>
<tr class="even">
<td><p>Dynamics AX Enterprise</p></td>
<td><p>Dynamics 365 Edizione Enterprise Plan 2</p>
<p>oppure Dynamics 365 for Operations</p></td>
</tr>
<tr class="odd">
<td><p>Dynamics AX Task</p></td>
<td><p>Dynamics 365 for Team Member</p></td>
</tr>
<tr class="even">
<td><p>Dynamics AX Functional</p></td>
<td><p>Dynamics 365 for Team Member</p></td>
</tr>
<tr class="odd">
<td><p>Dynamics AX Device</p></td>
<td><p>Dynamics 365 for Operations Device</p></td>
</tr>
</tbody>
</table>

 

**Microsoft Dynamics CRM Online**

Il piano corrente Microsoft Dynamics CRM Online è stato ritirato a partire dal 1 novembre 2016. Vedi le [informazioni importanti per i clienti di CRM Online](https://go.microsoft.com/fwlink/?linkid=831667) per scoprire di più sulle nuove opzioni per le licenze.

## Transizione dei clienti ai nuovi piani per i prodotti


Microsoft offre continuamente nuovi prodotti e servizi a rivenditori e provider. In questi casi, un rivenditore potrebbe avere la necessità di aggiornare i clienti ai nuovi servizi o di eseguire la migrazione delle loro sottoscrizioni da SKU destinati a essere ritirati. La migrazione dei clienti da SKU precedenti a quelli più recenti richiede la sequenza seguente:

-   [Acquistare la nuova sottoscrizione](#manual-subscription-migration-purchasenewsubsc);
-   [Riassegnare le licenze utente correnti](#manual-subscription-migration-reassignlicenses);
-   [Annullare la sottoscrizione precedente](#manual-subscription-migration-cancelsubscriptions).

Le procedure seguenti illustrano come eseguire la migrazione di un cliente da Dynamics AX7 Enterprise a Dynamics 365 for Operations.

<a href="" id="purchasenewsubsc"></a>
Il rivenditore deve eseguire la migrazione di un cliente con una sottoscrizione esistente per Dynamics AX Enterprise a Dynamics 365 for Operations. Il primo passaggio consiste nell'acquistare Dynamics 365 for Operations.

**Acquistare la nuova sottoscrizione**

1.  Nel menu **Dashboard** seleziona **Clienti**, seleziona il cliente di cui eseguire la migrazione e quindi scegli **Aggiungi sottoscrizioni**.
2.  Seleziona la sottoscrizione che vuoi acquistare dal catalogo (in questo caso Dynamics 365 for Operations, Enterprise Edition), immetti il numero di licenze e scegli **Invia**.

    Il cliente a questo punto dovrebbe avere sia la sottoscrizione nuova che quella precedente, in questo esempio la vecchia sottoscrizione Dynamics AX Enterprise e la nuova sottoscrizione di destinazione, Dynamics 365 for Operations, Enterprise Edition.

<a href="" id="reassignlicenses"></a>
Il passaggio successivo consiste nel riassegnare tutte le licenze utente esistenti alla nuova sottoscrizione.

**Riassegnare le licenze utente**

1.  Nel menu **Dashboard** seleziona **Clienti**, seleziona il cliente di cui eseguire la migrazione e quindi scegli **Utenti e licenze**. Viene aperta la pagina Utenti e licenze del cliente.
2.  Per riassegnare le licenze utente, seleziona l'utente da riassegnare e quindi seleziona **Gestisci licenze**.
3.  Nella pagina **Gestisci licenze** deseleziona la casella di controllo della licenza **Dynamics AX Enterprise** e seleziona la licenza **Dynamics 365 for Operations**.
4.  Seleziona **Invia**. Le nuove assegnazioni di licenza vengono visualizzate in una pagina di conferma.
5.  Ripeti la stessa procedura per tutti gli utenti del cliente per cui è necessaria la riassegnazione della licenza.

<a href="" id="cancelsubscriptions"></a>
Dopo aver spostato le licenze utente al nuovo servizio, puoi tranquillamente annullare la sottoscrizione precedente al livello principale del cliente.

**Annullare la sottoscrizione precedente**

1.  Nel menu **Dashboard** seleziona **Clienti**, seleziona il cliente di cui eseguire la migrazione e quindi seleziona la sottoscrizione che vuoi annullare.
2.  Nella pagina dei dettagli della sottoscrizione imposta lo **Stato** della sottoscrizione su **Sospeso**.
3.  Seleziona **Invia**.

La sottoscrizione precedente viene sospesa e la nuova sottoscrizione diventa attiva. Per la sottoscrizione sospesa verrà eseguito automaticamente l'annullamento del provisioning dopo 120 giorni. Il cliente non dovrà sostenere alcun costo aggiuntivo per la sottoscrizione precedente.

## Considerazioni aggiuntive


Se il cliente passa dal canale Open al programma per i servizi cloud per il provisioning di altre sottoscrizioni, dovrai eseguire anche la migrazione delle sottoscrizioni esistenti:

-   Se il cliente ha ricevuto la sottoscrizione precedente tramite il canale Open, il passaggio al programma CSP per il nuovo SKU è semplice.
-   Se il cliente non è ancora classificato come tuo cliente, puoi invitarlo. Per informazioni, vedi l'argomento della Guida [Richiedere una relazione con un cliente](https://msdn.microsoft.com/en-us/library/partnercenter/mt750320.aspx).

Dopo che il cliente ti accetta come provider indiretto, la procedura per il provisioning è fondamentalmente la stessa descritta in precedenza, ovvero devi acquistare la nuova sottoscrizione e quindi assegnare le licenze utente. L'unica differenza riguarda l'annullamento delle sottoscrizioni precedenti. Un nuovo provider non può annullare/sospendere sottoscrizioni acquisite tramite altri canali. Se il cliente ha acquisito le sottoscrizioni precedenti tramite un altro canale di vendita, come il canale Open, il cliente dovrà annullare autonomamente tali sottoscrizioni tramite il canale originale.

 

 






<!--HONumber=Jan17_HO2-->


