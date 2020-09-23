---
title: Iniziare a passare al piano di Azure
description: Scopri cosa è necessario sapere sull'uso del piano di Azure con pagamento in base al consumo, incluse le operazioni preliminari, le precauzioni di sicurezza e le procedure per iniziare.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.custom: SEOAPR.20
ms.localizationpriority: High
ms.date: 12/02/2019
ms.openlocfilehash: 5ad7bd7c99d7caa044877c98aac6dc5e3ce69420
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000575"
---
# <a name="begin-using-pay-as-you-go-rates-with-the-azure-plan"></a>Inizia a usare tariffe con pagamento in base al consumo con il piano di Azure

Microsoft ha introdotto una nuova esperienza commerciale nel Centro per i partner.  Con questa nuova esperienza commerciale e in base al Contratto Microsoft Partner, i partner potranno accedere ai servizi di Azure a tariffe con pagamento in base al consumo per i clienti.

Questo piano semplifica l'esperienza di acquisto consentendo di avere più sottoscrizioni di Azure in un piano di Azure. Non dovrai più inviare un ordine separato per ogni sottoscrizione di Azure. In questa nuova esperienza commerciale per Azure si siamo allineati a un unico principio globale in materia di prezzi che consente ai partner CSP di offrire Azure ai prezzi pubblicati.

Le esigenze di trasformazione digitale dei clienti richiedono nuove competenze da parte dei partner. Molti clienti richiedono ai partner di fornire servizi che vanno ben oltre le transazioni per poter sfruttare il cloud senza difficoltà e usare i servizi di Azure in modo efficiente. I partner Microsoft svolgono un ruolo fondamentale in tutte le fasi del ciclo di vita del cliente. I servizi di questo tipo da parte dei partner sono in continua evoluzione e includono il monitoraggio dell'ambiente Azure, la gestione dei criteri e della governance, le operazioni di configurazione e ottimizzazione, il supporto tecnico e un'ampia gamma di altri servizi. Questi servizi richiedono ai partner un'elevata familiarità con l'ambiente Azure del cliente, nonché governance e controllo continui e appropriati sulle risorse sottostanti gestite. I partner di fatturazione che forniscono servizi di gestione delle operazioni cloud 24 ore su 24 e 7 giorni su 7 saranno idonei per un **credito ottenuto dai partner per i servizi gestiti**.

## <a name="make-sure-your-customers-have-signed-the-microsoft-customer-agreement"></a>Verificare che i clienti abbiano firmato il contratto del cliente Microsoft

Dal 1° ottobre 2019 è disponibile il contratto del cliente Microsoft, un contratto perpetuo che semplifica l'esperienza di acquisto del cliente con un processo completamente digitale. Tutti i clienti che vogliono sfruttare la nuova esperienza commerciale in CSP per Azure devono firmare il contratto del cliente Microsoft.

I partner che vogliono eseguire transazioni con il nuovo piano di Azure e creare un nuovo ordine devono confermare l'accettazione del contratto del cliente Microsoft usando l'API e il dashboard Centro per i partner nell'ambiente di produzione.

Dal 1° febbraio 2020 il Contratto Microsoft Cloud esistente viene rimosso dal programma CSP. Successivamente, la conferma del partner (attestazione) dell'accettazione del nuovo contratto del cliente Microsoft sarà necessaria per tutte le altre offerte, tra cui Microsoft 365, Dynamics 365 e l'offerta Azure esistente. I partner del programma CSP non potranno creare un nuovo ordine per il cliente senza l'attestazione del contratto del cliente Microsoft.

Per informazioni dettagliate, leggi [Confermare l'accettazione del contratto del cliente Microsoft da parte di un cliente](confirm-customer-agreement.md).

## <a name="security-and-access-control-practices"></a>Procedure di sicurezza e controllo di accesso

Per la sicurezza di partner e clienti, viene introdotto un set di requisiti di sicurezza obbligatori per gli advisor, i fornitori di pannelli di controllo e i partner che partecipano al programma Cloud Solution Provider.

I partner che non implementano i requisiti di sicurezza obbligatori non potranno eseguire transazioni nel programma Cloud Solution Provider o gestire i tenant dei clienti usando i diritti di amministratore delegato quando verranno applicati tali requisiti. È in corso il processo di identificazione di una data di applicazione tecnica per i requisiti. I partner riceveranno una notifica con tale data e informazioni dettagliate.

## <a name="actions-to-take-to-implement-mfa"></a>Azioni da intraprendere per implementare l'autenticazione a più fattori

Considerati i privilegi elevati della condizione di partner, dobbiamo garantire che ogni utente disponga di una richiesta di autenticazione a più fattori per ogni singola autenticazione. Questo risultato può essere ottenuto in uno dei modi seguenti:

- Implementazione di Azure AD Premium e verifica che l'autenticazione a più fattori venga applicata per ogni utente
- Implementazione delle [impostazioni predefinite per la sicurezza Azure AD](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)
- Implementazione di una soluzione di terze parti e verifica che l'autenticazione a più fattori venga applicata per ogni utente

Dal 1° agosto 2019 tutti i partner sono tenuti a implementare l'autenticazione a più fattori per tutti gli utenti, inclusi gli account di servizio, nel tenant partner. Per informazioni dettagliate su questi requisiti di sicurezza, vedi [Requisiti di sicurezza per i partner](partner-security-requirements.md).

Microsoft consiglia ai partner di usare il controllo degli accessi in base al ruolo prestando la massima attenzione e seguendo le procedure consigliate abilitate tramite [Risorse di Azure Active Directory Privileged Identity Management](/azure/active-directory/privileged-identity-management/pim-configure).

## <a name="read-more-about-the-azure-plan"></a>Scopri di più sul piano di Azure

- [Acquistare il piano di Azure](purchase-azure-plan.md)

- [Confrontare le offerte di Azure](compare-azure-offers.md)

- [Credito ottenuto dai partner - Panoramica](partner-earned-credit.md)

- I calcoli relativi ai crediti ottenuti dai partner e i ruoli e le autorizzazioni idonei per ottenere tali crediti sono disponibili nel listino prezzi riportato nel dashboard del Centro per i partner (informazioni di accesso obbligatorie).

## <a name="next-steps"></a>Passaggi successivi 

- [Come viene calcolato il credito ottenuto dai partner - Dettagli](partner-earned-credit-explanation.md)
- [Listino prezzi del piano di Azure - Descrizione](azure-plan-price-list.md)
- [Eseguire la transizione dei clienti al piano di Azure](azure-plan-transition.md)
- [Gestire sottoscrizioni e risorse nel piano di Azure](azure-plan-manage.md)
- [Elenco completo di Paesi/aree geografiche in cui è disponibile il piano di Azure](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QN0x)