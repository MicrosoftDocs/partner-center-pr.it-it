---
title: Non è possibile accedere al centro per i partner
ms.topic: troubleshooting
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 'Risolvere le possibili cause e ottenere informazioni sulle soluzioni per i casi in cui non è possibile accedere al centro per i partner: ulteriori informazioni sulla reimpostazione delle password, il controllo dei ruoli e il controllo delle credenziali.'
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 17087727afcaf3dbcf47801f8668388c370758e7
ms.sourcegitcommit: 9b04509f3830462628c1bb6af2ca41ed68b52619
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/09/2021
ms.locfileid: "107266572"
---
# <a name="troubleshoot-sign-in-issues-for-partner-center"></a>Risolvere i problemi di accesso per il centro per i partner

**Ruoli appropriati**

- Tutti i partner interessati al centro per i partner

Questo articolo contiene le soluzioni per i problemi di accesso comuni per il centro per i partner.

## <a name="youve-forgotten-your-password-for-partner-center"></a>La password per il centro per i partner è stata dimenticata

Se la password è stata dimenticata e non è possibile accedere al centro per i partner, contattare il supporto tecnico. Trova il contatto appropriato al [supporto tecnico per i prodotti aziendali](/microsoft-365/admin/contact-support-for-business-products).

Se sei un partner MPN, Chiedi all'amministratore globale di creare una nuova password. Se si è un rivenditore indiretto CSP, chiedere al provider indiretto di creare un nuovo amministratore globale nel tenant di Azure AD o di creare una nuova password per l'utente usando i privilegi di amministratore delegato.

Per altre informazioni su come è possibile reimpostare la password e riottenere l'accesso all'account aziendale, vedere [reimpostare la password aziendale o dell'Istituto di istruzione usando le info di sicurezza](/azure/active-directory/user-help/active-directory-passwords-update-your-own-password#how-to-change-your-password).

## <a name="you-cant-view-or-manage-the-expected-pages-or-capabilities-in-partner-center"></a>Non è possibile visualizzare o gestire le pagine o le funzionalità previste nel centro per i partner

L'accesso alle pagine del centro per i partner è controllato dai ruoli assegnati. Per verificare quali ruoli sono assegnati, in centro per i partner selezionare l'icona Impostazioni, selezionare **Impostazioni account**, quindi in Impostazioni account selezionare **Gestione utenti**. In Cerca digitare il nome e quindi visualizzare i risultati.

Se non si è in grado di visualizzare o gestire le competenze, i clienti, gli incentivi o gli utenti previsti, provare le soluzioni seguenti:

- Per l'accesso alle funzionalità di MPN, CSP e riferimenti, contattare l'amministratore globale o l'amministratore dell'account. Per altre informazioni sui ruoli e sulle attività da essi abilitate nel centro per i partner, vedere [assegnare ruoli & autorizzazioni agli utenti](permissions-overview.md).
- Per l'accesso alle funzionalità del Marketplace commerciale e dei programmi di Windows & Xbox, Office Store, Microsoft Edge e per sviluppatori hardware, contattare la persona nel ruolo proprietario o responsabile dell'organizzazione. Per ulteriori informazioni su ruoli e autorizzazioni, vedere [come gestire un account del Marketplace commerciale nel centro per i partner Microsoft](/azure/marketplace/partner-center-portal/manage-account#define-user-roles-and-permissions).

## <a name="you-cant-see-your-offer-or-benefits-in-partner-center"></a>Non è possibile visualizzare l'offerta o i vantaggi nel centro per i partner

Assicurarsi di usare le credenziali corrette per accedere. Ad esempio, gli account aziendali e personali potrebbero avere lo stesso aspetto (ad esempio abc@contoso.com ), ma uno può essere un account personale creato e un altro potrebbe essere un account aziendale configurato per conto dell'utente. In questo caso, se è stato eseguito l'accesso, ma non è possibile visualizzare le funzionalità previste relative a MPN, CSP, Marketplace commerciale, provare a selezionare l'account aziendale.

## <a name="next-steps"></a>Passaggi successivi

- [Verificare le informazioni sull'account](verification-responses.md)
- [Reimpostare la password personale](reset-my-pasword.md)
- [Reimpostare una password utente](reset-a-user-password.md)