---
title: Creare account utente e impostare le autorizzazioni | Centro partner
description: L'amministratore crea un account utente per ogni dipendente del partner che deve accedere al Centro per i partner.
ms.assetid: 75D805AE-9922-4CFD-9427-196047D70963
author: MaggiePucciEvans
ms.openlocfilehash: 842071dad94251ee498c9dee3e8b689e2e036485
ms.sourcegitcommit: c2a12d6a18b9631916f6dd8301a4752ecc03296b
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 06/19/2017
---
# <a name="create-user-accounts-and-assign-permissions"></a>Creare account utente e assegnare le autorizzazioni

**Si applica a**

-  Centro per i partner

Creare gli account utente per i dipendenti che richiedono l'accesso al Centro per i partner. Queste attività devono essere eseguite da un amministratore con autorizzazioni di amministratore per la gestione degli utenti. 

## <a name="add-a-new-user"></a>Aggiungere un nuovo utente

1. Dal menu **Dashboard** seleziona **Impostazioni account > Gestione degli utenti**.

2.  Seleziona **Aggiungi utente**.

3.  Immetti il nome completo e l'indirizzo di posta elettronica univoco dell'utente.

4.  Seleziona il tipo di agente e il tipo di amministratore. L'accesso al Centro per i partner è basato sui ruoli, pertanto puoi assegnare autorizzazioni per personalizzare la visualizzazione dell'utente in modo da mostrargli solo le funzionalità utili per completare le attività specifiche. Per altre informazioni sulle operazioni possibili con ciascun ruolo, vedi [Assegnare le autorizzazioni utente](#assignuserpermissions).

5.  Seleziona **Aggiungi** per creare l'account utente. Verifica i dettagli dell'utente nella pagina successiva.

>**Importante**<br>
Prendi nota delle informazioni di accesso del nuovo utente visualizzate in questa pagina. Copiale e inviale al nuovo utente perché dopo non potrai più accedervi. <br>

>L'utente dovrà accedere al Centro per i partner con il nome utente e la password temporanea. Quando l'utente accede al Centro per i partner per la prima volta, gli viene chiesto di modificare la password.    


### <a href="" id="assignuserpermissions"></a>Assegnare le autorizzazioni utente

L'accesso al Centro per i partner è basato sui ruoli, pertanto puoi assegnare autorizzazioni per personalizzare la visualizzazione dell'utente in modo da mostrargli solo le funzionalità utili per completare le attività specifiche. 

Per ogni utente devi selezionare due livelli di autorizzazione:

-   Le autorizzazioni dell'agente controllano il tipo di dati dei clienti e le informazioni sull'account che l'utente può visualizzare e modificare.

-   Le autorizzazioni di amministratore controllano il livello di accesso che l'utente ha alle funzionalità del Centro per i partner. Questa impostazione ha un impatto al di fuori del Centro per i partner, in quanto un amministratore della fatturazione può accedere alle fatture per tutti i servizi Microsoft (anche quelle che non riguardano CSP) e un amministratore globale può accedere agli account utente e dei clienti, anche a quelli per servizi diversi da CSP.

>**Importante** L'impostazione predefinita deve sempre essere **Non amministratore**, a meno che il ruolo dell'utente non richieda un accesso aggiuntivo per completare attività e supportare i clienti.

La tabella seguente illustra le operazioni che ogni ruolo può eseguire nel Centro per i partner.

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Ruolo del Centro per i partner</strong></p></td>
<td><p><strong>Operazioni consentite</strong></p></td>
<td><p><strong>Operazioni non consentite</strong></p></td>
</tr>
<tr class="even">
<td><p><strong>Agente amministratore</strong></p></td>
<td><ul>
<li><p>Gestione dei clienti</p></li>
<li><p>Aggiunta dell'elenco dei dispositivi al Centro per i partner</p></li>
<p><li>Creazione e applicazione di profili ai dispositivi</p></li>
<li><p>Gestione delle sottoscrizioni</p></li>
<li><p>Assistenza alle richieste di integrità e di servizio per i clienti</p></li>
<li><p>Richiesta dei privilegi di amministrazione delegati</p></li>
<li><p>Visualizzazione dei prezzi e delle offerte</p></li>
<li><p>Fatturazione</p></li>
<li><p>Amministrazione per conto di un cliente</p></li>
<li><p>Registrazione di un rivenditore a valore aggiunto</p></li>
</ul></td>
<td><ul>
<li><p>Gestione degli utenti</p></li>
<li><p>Richieste di servizio per il Centro per i partner</p></li>
</ul></td>
</tr>
<tr class="odd">
<td><p><strong>Agente di vendita</strong></p></td>
<td><ul>
<li><p>Gestione dei clienti</p></li>
<li><p>Aggiunta dell'elenco dei dispositivi al Centro per i partner</p></li>
<li><p>Gestione delle sottoscrizioni</p></li>
<li><p>Visualizzazione dei ticket di supporto</p></li>
<li><p>Richiesta di una relazione con un cliente</p></li>
<li><p>Gestione dei lead dei clienti</p></li>
<li><p>Visualizzazione del contratto per il cliente</p></li>
<li><p>Registrazione di un rivenditore a valore aggiunto</p></li>
</ul></td>
<td><ul>
<li><p>Creazione di richieste di assistenza per problemi con il Centro per i partner</p></li>
<li><p>Risoluzione dei ticket di supporto</p></li>
<li><p>Visualizzazione dell'integrità del servizio</p></li>
<li><p>Visualizzazione di prezzi e offerte</p></li>
<li><p>Fatturazione</p></li>
<li><p>Amministrazione per conto di un cliente</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>Agente help desk</strong></p></td>
<td><ul>
<li><p>Ricerca e visualizzazione di un cliente</p></li>
<li><p>Modifica dei dettagli dei clienti</p></li>
<li><p>Integrità servizio</p></li>
<li><p>Richiesta di supporto per conto dei clienti (Nota: è necessario essere un agente amministratore per completare questa attività per gli abbonamenti a Office 365)</p></li>
<li><p>Gestione delle sottoscrizioni e dei servizi per conto dei clienti (Nota: è necessario essere un agente amministratore per completare questa attività per gli abbonamenti di Office 365)</p></li>
</ul></td>
<td><ul>
<li><p>Visualizzazione dei profili dei partner</p></li>
<li><p>Creazione di un nuovo account cliente</p></li>
<li><p>Modifica delle info di fatturazione dei clienti</p></li>
<li><p>Gestione delle sottoscrizioni</p></li>
<li><p>Richiesta di una relazione con un cliente</p></li>
<li><p>Gestione dei lead dei clienti</p></li>
<li><p>Visualizzazione di prezzi e offerte</p></li>
<li><p>Visualizzazione del contratto per il cliente</p></li>
<li><p>Fatturazione</p></li>
<li><p>Registrazione di un rivenditore a valore aggiunto</p></li>
</ul></td>
</tr>
<tr class="odd">
<td><p><strong>Amministratore globale</strong></p></td>
<td><ul>
<li><p>Accesso a tutti gli account/servizi Microsoft con privilegi completi</p></li>
<li><p>Creazione di ticket di supporto per il Centro per i partner</p></li>
<li><p>Visualizzazione di contratti, listini prezzi e offerte</p></li>
<li><p>Fatturazione</p></li>
<li><p>Visualizzazione, creazione e gestione di utenti partner</p></li>
</ul></td>
<td></td>
</tr>
<tr class="even">
<td><p><strong>Amministratore fatturazione</strong></p></td>
<td><ul>
<li><p>Accesso a tutte le fatture di Microsoft con privilegi completi</p></li>
<li><p>Visualizzazione di contratti, listini prezzi e offerte</p></li>
<li><p>Fatturazione</p></li>
</ul></td>
<td></td>
</tr>
<tr class="odd">
<td><p><strong>Amministratore gestione utenti</strong></p></td>
<td><ul>
<li><p>Visualizzazione, creazione e gestione di utenti</p></li>
<li><p>Visualizzazione di tutti i profili dei partner</p></li>
</ul></td>
<td></td>
</tr>
</tbody>
</table>

 

 

 



