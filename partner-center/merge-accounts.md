---
title: Unire l'account partner con un altro account partner
description: Le aziende che sono partner Microsoft attivi nel centro per i partner possono unire i propri account.
ms.topic: article
author: parthpandyaMSFT
ms.author: parthp
ms.custom: seodec18
ms.date: 06/12/2020
ms.openlocfilehash: 6c2ac5560b77528766a4d0aa068f231e0aa0bc99
ms.sourcegitcommit: e1c8bea4aaf807aebe99c125cb1fb6dc8fdfa210
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/30/2020
ms.locfileid: "87444957"
---
# <a name="merge-your-partner-account-with-another-partner-account"></a>Unire l'account partner con un altro account partner

**Ruoli applicabili**

- Amministratore degli account

Due o più società che sono partner Microsoft attivi e dispongono di account nel centro per i partner possono scegliere di unire i propri account.

## <a name="what-happens-when-two-partners-elect-to-merge-their-partner-center-accounts"></a>Cosa accade quando due partner scelgono di unire gli account del centro per i partner

- L'organizzazione partner che avvia l'Unione sarà l'account globale del partner (PGA).

- Il PGA dell'organizzazione invitata diventa una sede della società iniziale.

- Tutte le posizioni dell'account di merge diventano posizioni nel PGA.

- Una volta completata la fusione dell'account, vengono visualizzati i dettagli dell'account, ad esempio località e utenti all'interno del profilo PGA. Non è possibile annullare questo processo.

- Tutti gli ID MPN per le posizioni vengono conservati durante questo consolidamento.

- I ruoli dell'utente vengono riportati. Se, ad esempio, un utente è stato l'amministratore di incentivi per una località specifica, avrà ancora tale ruolo dopo la fusione e potrà visualizzare gli incentivi che hanno visto prima della fusione.

- Azure AD tenant e gli account CSP non vengono Uniti e non hanno alcun effetto.

- Sono mantenute le offerte pubblicate e i dati della pipeline di co-selling associati a entrambe le aziende

### <a name="view-of-merged-accounts"></a>Visualizzazione degli account Uniti

:::image type="content" source="images/merge-accounts/account-merge.png" alt-text="Unione degli account":::

## <a name="what-to-expect-if-you-have-been-invited-to-merge-your-partner-center-account-with-another-partner-center-account"></a>Cosa aspettarsi se si è stati invitati a unire l'account del centro per i partner con un altro account del centro per i partner

Se si decide di accettare l'invito per l'Unione degli account: · Gli ID e le località MPN verranno uniti nel PGA dell'account partner che ha invitato l'utente.

- Gli utenti verranno portati nell'account Unito con i loro ruoli intatti.

- I vantaggi e le competenze esistenti verranno conservati per entrambe le aziende dopo la fusione fino al rinnovo. Al rinnovo, gli account verranno considerati come una società e verranno applicate le regole di rinnovo standard.

## <a name="understand-the-impacts-to-programs-and-benefits-when-partners-elect-to-merge-accounts"></a>Informazioni sugli effetti sui programmi e sui vantaggi quando i partner scelgono di unire gli account

- Tutte le competenze esistenti (Gold/Silver), gli acquisti (ad esempio Microsoft Action Pack) e i vantaggi associati vengono conservati durante il consolidamento. Se entrambe le aziende hanno la stessa competenza ma una è l'oro e l'altra Silver, verranno concesse le competenze con il livello di competenza più elevato e i partner avranno un set di vantaggi Silver e un set di vantaggi Gold per tale competenza fino al successivo rinnovo. 

- La data di anniversario più elevata per Microsoft Action Pack verrà mantenuta dopo la fusione. Se, ad esempio, la data di anniversario per la società 1 è il 2020 giugno per Action Pack rinnovo e la data di anniversario per Action Pack rinnovo per la società 2 è ottobre 2020, Microsoft utilizzerà la data di ottobre 2020 come nuova data di anniversario per la società unita.

- Durante la fusione degli account e fino al successivo rinnovo, ogni account manterrà i vantaggi Action Pack e/o le competenze. Al rinnovo, si applicano le regole di rinnovo di Action Pack e competenze standard.

- Al momento del rinnovo, i vantaggi inclusi nel raggiungimento delle competenze e Action Pack vengono implementati per l'account globale del partner della società partner:

  - Microsoft Action Pack: la società partner sarà in grado di acquistare una Action Pack per ogni account globale del partner.

  - Competenza: la società partner riceverà un pacchetto di vantaggi di base, associato al raggiungimento più elevato, oltre a vantaggi specifici per la competenza, il partner è idoneo per l'account globale per partner.

- Tutti i vantaggi sono soggetti alla [Guida all'utilizzo di Microsoft Partner Network benefits](https://aka.ms/partner-benefits-use-guide). Ad esempio, un token O365 E3 attivato è funzionante per dodici (12) mesi dopo l'attivazione. Una volta che un token è stato attivato per le licenze in un tenant, tali licenze potrebbero non essere spostate in un altro tenant.

- Le associazioni MCP ID per entrambe le aziende verranno mantenute e associate all'ID MPN PGA.

- I vantaggi tecnici e go-to-Market sono offerti come vantaggio di base per le competenze. Dopo l'Unione, è consigliabile controllare le informazioni sulla banca e sull'imposta per garantire la precisione.

- Se la società si trova nel programma MSP di Azure Expert, i vantaggi vengono conservati fino al rinnovo.

- Se la società ha ottenuto specializzazioni avanzate, vengono conservate in entrambi gli account.

- Tutti i voucher Software Assurance vengono conservati in entrambi gli account. 

## <a name="invite-a-company-to-merge-their-partner-center-account-with-your-partner-center-account"></a>Invita una società a unire il proprio account del centro per i partner con l'account del centro per i partner

>[!Note]
>Per eseguire la fusione degli account, è necessario essere l' **amministratore dell'account** per l'azienda.

1. Selezionare **Impostazioni** dal dashboard del centro per i partner. 

2. Selezionare **merge account**.

3. Aggiungere l'ID MPN che si trova nel **profilo partner** dell'account che si vuole invitare a unire. È necessario usare l'ID MPN globale del partner. Non è possibile usare un ID MPN della località.

4. Quando si seleziona **merge**, viene inviato un invito alla società partner. Quando accettano la richiesta, è possibile avviare l'Unione degli account nel centro per i partner. Se la società rifiuta la richiesta di Unione degli account, può spiegare perché ha rifiutato la richiesta. Un elenco di tutte le unioni di account è disponibile nella **cronologia di merge**.

## <a name="next-steps"></a>Passaggi successivi

- [Assegnare autorizzazioni e ruoli utente](permissions-overview.md)

- [Verificare le informazioni del profilo partner](update-your-partner-profile.md)

- [Consente di aggiungere servizi condivisi di Azure partner per consentire ai partner di acquistare sottoscrizioni di Azure per uso personale](shared-services.md)
