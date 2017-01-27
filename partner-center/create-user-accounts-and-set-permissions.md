---
title: Creare account utente e impostare le autorizzazioni | Centro partner
description: L&quot;amministratore crea un account utente per ogni dipendente del partner che deve accedere al Centro per i partner.
ms.assetid: 75D805AE-9922-4CFD-9427-196047D70963
author: MaggiePucciEvans
translationtype: Human Translation
ms.sourcegitcommit: e1825890f208a90b9b5694f4000ac06687ac87ab
ms.openlocfilehash: a755c9375c7bd5e61345d7d7e1ab27e00af3fe4d

---

# Creare account utente e impostare le autorizzazioni

**Si applica a**

-  Centro per i partner

L'amministratore crea un account utente per ogni dipendente del partner che deve accedere al Centro per i partner. Queste attività devono essere eseguite da un amministratore con le autorizzazioni **Amministratore globale** o **Amministratore gestione utenti**. In **Impostazioni account** &gt; **Gestione utenti** puoi aggiungere account e impostare o aggiornare le autorizzazioni.

**Aggiungere un nuovo utente**

1.  Nel Centro per i partner vai al menu Dashboard &gt; **Impostazioni account** &gt; **Gestione utenti**.
2.  Scegli **Aggiungi utente**.

3.  Digita il nome completo dell'utente e crea un indirizzo e-mail univoco.

4.  Seleziona il tipo di agente e il tipo di amministratore. L'accesso al Centro per i partner è basato sui ruoli, pertanto le selezioni effettuate in questo passaggio consentono di personalizzare la visualizzazione dell'utente affinché visualizzi solo le funzionalità necessarie. Per altre informazioni sulle operazioni possibili con ciascun ruolo, vedi [Impostare le autorizzazioni utente](#setuserpermissions).

5.  Aggiungi l'utente. Verrà visualizzata una schermata di conferma con una password temporanea per il nuovo account di accesso. Copialo e invialo al nuovo utente perché non sarà più accessibile quando lascerai la schermata. In fase di accesso, all'utente verrà richiesto di aggiornare la password.

### <a href="" id="setuserpermissions"></a>Impostare le autorizzazioni utente

L'accesso al Centro per i partner è basato su ruoli. Ciò significa che puoi personalizzare la visualizzazione utente in modo che includa solo le funzionalità che serviranno all'utente per il proprio lavoro. Per ogni utente devi selezionare sue impostazioni:

-   L'impostazione **agente** controlla il tipo di dati del cliente e le informazioni Microsoft che l'utente può visualizzare.

-   L'impostazione **amministratore** determina il livello di controllo che l'utente avrà sull'ambiente del Centro per i partner e su tutti gli altri servizi Microsoft (account, profili e ticket di supporto). Questa impostazione ha un impatto al di fuori del Centro per i partner, in quanto un amministratore della fatturazione può accedere a tutte le fatture per tutti i servizi Microsoft (anche quelle che non riguardano CSP) e un amministratore globale può accedere agli account utente e dei clienti, anche a quelli per servizi diversi da CSP.

    L'impostazione predefinita deve sempre essere **Non amministratore**, a meno che il ruolo dell'utente non richieda accesso aggiuntivo per completare attività e supportare i clienti.

La tabella seguente illustra tutte le attività che ogni ruolo può eseguire nel Centro per i partner.

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
<li><p>Gestione degli abbonamenti</p></li>
<li><p>Integrità del servizio e richieste di servizio per i clienti</p></li>
<li><p>Richiesta di privilegi di amministrazione delegati</p></li>
<li><p>Visualizzazione di prezzi e offerte</p></li>
<li><p>Fatturazione</p></li>
<li><p>Amministrazione per conto di un utente</p></li>
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
<li><p>Gestione degli abbonamenti</p></li>
<li><p>Visualizzazione dei ticket di supporto</p></li>
<li><p>Richiesta di una relazione</p></li>
<li><p>Gestione dei lead dei clienti</p></li>
<li><p>Visualizzazione del contratto per il cliente</p></li>
<li><p>Registrazione di un rivenditore a valore aggiunto</p></li>
</ul></td>
<td><ul>
<li><p>Creazione di ticket di supporto per i servizi o il Centro per i partner</p></li>
<li><p>Risoluzione dei ticket di supporto</p></li>
<li><p>Visualizzazione dell'integrità del servizio</p></li>
<li><p>Visualizzazione di prezzi e offerte</p></li>
<li><p>Fatturazione</p></li>
<li><p>Amministrazione per conto di un utente</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>Agente help desk</strong></p></td>
<td><ul>
<li><p>Ricerca e visualizzazione di un cliente</p></li>
<li><p>Modifica dei dettagli dei clienti</p></li>
<li><p>Servizio integrità</p></li>
<li><p>Creazione di ticket di supporto per i clienti</p></li>
<li><p>Gestione dei servizi per conto dei clienti</p></li>
</ul></td>
<td><ul>
<li><p>Visualizzazione dei profili dei partner</p></li>
<li><p>Creazione di un nuovo elenco clienti</p></li>
<li><p>Modifica delle info di fatturazione dei clienti</p></li>
<li><p>Gestione degli abbonamenti</p></li>
<li><p>Richiesta di una relazione</p></li>
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

 

 

 






<!--HONumber=Jan17_HO2-->


