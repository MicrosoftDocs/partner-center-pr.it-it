---
title: Non è possibile accedere a Partner Center
ms.topic: troubleshooting
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 'Risolvere le possibili cause e ottenere informazioni sulle soluzioni per quando non è possibile accedere a Partner Center: altre informazioni sulla reimpostazione delle password, il controllo dei ruoli e il controllo delle credenziali.'
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2b67201355e748f9280d28413a8737a9b07db5c6
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431493"
---
# <a name="troubleshoot-sign-in-issues-for-partner-center"></a>Risolvere i problemi di accesso per Partner Center

**Ruoli appropriati:** tutti i partner interessati a Partner Center

Questo articolo contiene soluzioni per problemi di accesso comuni per Partner Center.

## <a name="youve-forgotten-your-password-for-partner-center"></a>È stata dimenticata la password per Partner Center

Se la password è stata dimenticata e non è possibile accedere Partner Center, contattare il supporto tecnico. Trovare il contatto appropriato in [Supporto per i prodotti aziendali.](/microsoft-365/admin/contact-support-for-business-products)

Se si è un partner Microsoft Partner Network (MPN), chiedere all'amministratore globale di creare una nuova password. Se si è un rivenditore indiretto Cloud Solution Provider (CSP), chiedere al provider indiretto di creare un nuovo amministratore globale nel tenant di Azure Active Directory (AD) o creare una nuova password usando i privilegi di amministratore delegato.

Per altre informazioni su come reimpostare la password e ottenere nuovamente l'accesso all'account aziendale, vedere Reimpostare la password aziendale o dell'istituto di [istruzione usando le informazioni di sicurezza.](/azure/active-directory/user-help/active-directory-passwords-update-your-own-password#how-to-change-your-password)

## <a name="you-cant-view-or-manage-the-expected-pages-or-capabilities-in-partner-center"></a>Non è possibile visualizzare o gestire le pagine o le funzionalità previste Partner Center

L'accesso alle Partner Center è controllato dai ruoli assegnati. Per controllare i ruoli assegnati, in Partner Center selezionare l'icona Impostazioni, selezionare **Impostazioni** account e quindi in Impostazioni account selezionare **Gestione utenti.** In Cerca digitare il nome e quindi visualizzare i risultati.

Se non è possibile visualizzare o gestire le competenze, i clienti, gli incentivi o gli utenti previsti, provare le soluzioni seguenti:

- Per accedere alle funzionalità di MPN, CSP e Segnalazioni, contattare l'amministratore globale o l'amministratore dell'account. Per altre informazioni sui ruoli e sulle attività abilitate in Partner Center, vedere Assegnare ruoli & [autorizzazioni agli utenti](permissions-overview.md).
- Per accedere alle funzionalità del Marketplace commerciale e dei programmi per sviluppatori Windows & Xbox, Office Store, Microsoft Edge e Hardware, contattare la persona nel ruolo Proprietario o Manager dell'organizzazione. Per altre informazioni su ruoli e autorizzazioni, vedere [Come gestire un account del marketplace](/azure/marketplace/partner-center-portal/manage-account#define-user-roles-and-permissions)commerciale in Microsoft Partner Center .

## <a name="you-cant-see-your-offer-or-benefits-in-partner-center"></a>Non è possibile visualizzare l'offerta o i vantaggi in Partner Center

Verificare di usare le credenziali corrette per l'accesso. Ad esempio, gli account aziendali e personali possono avere lo stesso aspetto ( ad esempio ), ma uno può essere un account personale creato e un altro può essere un account aziendale configurato per abc@contoso.com conto dell'utente. In questo caso, se è stato eseguito l'accesso, ma non è possibile visualizzare le funzionalità previste correlate a MPN, CSP, Marketplace commerciale, provare a selezionare l'account aziendale.

## <a name="next-steps"></a>Passaggi successivi

- [Verificare le informazioni sull'account](verification-responses.md)
- [Reimpostare la password personale](reset-my-pasword.md)
- [Reimpostare una password utente](reset-a-user-password.md)