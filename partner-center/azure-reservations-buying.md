---
title: Acquistare Microsoft Azure prenotazioni per i clienti
description: Informazioni su come acquistare o acquistare prenotazioni di Azure per conto dei clienti in Partner Center. Elenca anche i mercati in cui le prenotazioni di Azure non sono disponibili.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.date: 08/06/2020
ms.openlocfilehash: cd8a78edab25b94e678aafd61ca96e61a625fb07
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149537"
---
# <a name="buy-microsoft-azure-reservations-on-behalf-of-your-customers-in-partner-center"></a>Acquistare Microsoft Azure prenotazioni per conto dei clienti in Partner Center

**Ruoli appropriati:** agente di amministrazione | Amministratore globale | Agente del supporto | Agente di vendita | Amministratore gestione utenti

Questo articolo illustra come acquistare o acquistare prenotazioni di Azure per conto dei clienti in Partner Center. Identifica anche i mercati in cui le prenotazioni di Azure non sono disponibili.
 
> [!NOTE]
> Questo articolo si applica solo ai partner del Cloud Solution Provider (CSP). I clienti che usano altri tipi di sottoscrizioni (ad esempio, sottoscrizioni con pagamento in base al go, singole, Contratto del cliente Microsoft o Contratto Enterprise) devono invece leggere la documentazione sulle prenotazioni [di Azure.](/azure/cost-management-billing/reservations)

## <a name="before-you-begin"></a>Prima di iniziare

Prima di acquistare prenotazioni di Azure per conto dei clienti, esaminare le informazioni importanti riportate di seguito. Si vuole che i clienti siano in grado di acquistare le proprie prenotazioni di Azure da una sottoscrizione di Azure precedente acquistata per loro? Vedere [Concedere ai clienti l'autorizzazione per acquistare le proprie prenotazioni di Azure.](give-customers-permission.md#give-customers-permission-to-buy-their-own-azure-reservations)

- Se e quando il cliente firma il nuovo Contratto del cliente Microsoft (vedere Confermare l'accettazione del Contratto del cliente Microsoft [da](confirm-customer-agreement.md)parte del cliente), è necessario acquistare prenotazioni di Azure nel piano di Azure. Per altre informazioni, vedere [Acquistare un piano di Azure.](purchase-azure-plan.md)

- I clienti devono avere già una sottoscrizione di Azure attiva prima di poter acquistare prenotazioni per loro conto
  
- I costi delle sottoscrizioni software, ad esempio il database SQL o il software SUSE Linux, non sono inclusi nei prezzi delle prenotazioni di Azure

- I prezzi commerciali di Microsoft non includono le imposte, a meno che la località non sia il Brasile. Se la località è il Brasile, il prezzo commerciale include le imposte appropriate

- Gli agenti di vendita e help desk necessitano dell'accesso esplicito alla sottoscrizione di Azure in modo che possano acquistarla o gestirla nel portale di Azure e menti le richieste di supporto, inclusi scambi e rimborsi, per conto del cliente  

- Se si è un provider indiretto e si acquistano prenotazioni di Azure tramite il portale di Azure, il Partner of Record (rivenditore indiretto) viene ereditato dalla sottoscrizione Azure CSP selezionata.

- Il Partner of Record per le prenotazioni di Azure non può essere modificato dopo l'acquisto. È possibile annullare la prenotazione esistente e acquistarne una nuova con il nuovo Partner of Record.

- Se un cliente vuole trasferire una sottoscrizione di Azure da Direct o EA a CSP, le prenotazioni non vengono trasferite.

## <a name="azure-reservations-unavailable-markets"></a>Mercati non disponibili per prenotazioni di Azure

> [!IMPORTANT]
> Le prenotazioni di Azure **non sono** disponibili nei mercati seguenti:  
>  
> **Mercati non disponibili (in ordine alfabetico)**
>
> |Da A a Gi   | Da Gr a Pal  | Da Pap a Z |
> |--------------------------------|-----------------------------------|------------------------------------------|
> | Isole Åland     | Groenlandia     | Papua Nuova Guinea     |
> | Samoa Americane     | Grenada     | Isole Pitcairn     |
> | Andorra     | Guadalupa     | Riunione     |
> | Anguilla     | Guam     | Saba   |
> | Antartide     | Guernsey     | Saint Barthélemy   |
> | Antigua e Barbuda       | Guinea     | Saint Lucia   |
> | Aruba       | Guinea-Bissau     | Saint Martin   |
> | Azerbaigian       | Guyana     | Saint Pierre e Miquelon   |
> | Benin     | Haiti       | Saint Vincent e Grenadine     |
> | Bhutan     | Heard e McDonald       | Samoa     |
> | Bonaire     | Isola di Man     | San Marino     |
> | Isola Bouvet     | Jan Mayen     | São Tomé e Príncipe   |
> | Territorio britannico dell'Oceano Indiano       | Jersey     | Seychelles   |
> | Isole Vergini Britanniche     | Kiribati       | Sierra Leone   |
> | Burkina Faso     | Kosovo     | Sint Eustatius     |
> | Burundi     | Laos     | Sint Maarten     |
> | Cambogia     | Lesotho     | Isole Salomone     |
> | Repubblica Centrafricana     | Liberia     | Somalia     |
> | Ciad     | Madagascar     | Georgia del Sud e Isole Sandwich Australi     |
> | Cina     | Malawi     | Sud Sudan     |
> | Isola Christmas     | Maldive     | Sant'Elena, Ascensione, Tristan da Cunha     |
> | Isole Cocos (Keeling)     | Mali     | Suriname     |
> | Comore     | Marshall     | Svalbard     |
> | Congo     | Martinica     | Swaziland     |
> | Repubblica democratica del Congo     | Mauritania     | Timor-Leste   |
> | Isole Cook     | Mayotte     | Togo   |
> | Gibuti     | Micronesia     | Tokelau   |
> | Dominica     | Montserrat     | Tonga   |
> | Guinea Equatoriale     | Mozambico     | Turks e Caicos, Isole   |
> | Eritrea     | Myanmar     | Tuvalu   |
> | Isole Falkland     | Nauru     | Stati Uniti Altre isole americane del Pacifico   |
> | Guayana Francese     | Nuova Caledonia     | Vanuatu   |
> | Polinesia Francese     | Niger     | Città del Vaticano   |
> | Terre australi francesi     | Niue     | Wallis e Futuna   |
> | Gabon     | Norfolk     | Yemen   |
> | Gambia     | Marianne Settentrionali     |    |
> | Gibilterra     | Palau       |    |

## <a name="purchase-azure-reservations"></a>Acquistare prenotazioni di Azure

Seguire questa procedura per acquistare Microsoft Azure prenotazioni per conto dei clienti in Partner Center. Si vuole che i clienti siano in grado di acquistare le proprie prenotazioni di Azure da una sottoscrizione di Azure precedente acquistata per loro? Vedere [Concedere ai clienti l'autorizzazione per acquistare le proprie prenotazioni di Azure.](give-customers-permission.md)

1. Selezionare **Clienti** dal menu Partner Center.  

2. Nella pagina **Clienti** trovare il cliente che vuole acquistare prenotazioni di Azure e quindi selezionare la freccia rivolta verso il basso per espandere la riga del cliente.  

3. Seleziona **Aggiungi prodotti** e quindi **Azure**. 

    a. Scegli il segmento di mercato del cliente dall'elenco **Segmento**.

    b. Scegliere **Prenotazioni dall'elenco** **Tipo di** prodotto.

    c. Scegli il tipo di prenotazione desiderata dal cliente dall'elenco **Tipo di prenotazione**.

4. Le prenotazioni di Azure devono essere associate a una sottoscrizione di Azure attiva. Scegliere la sottoscrizione del cliente a cui si vogliono aggiungere prenotazioni di Azure **dall'elenco Sottoscrizione** cliente. 

   >[!IMPORTANT]
   >Se il cliente non ha già una sottoscrizione di Azure attiva, selezionare **Azure** per aggiungerne una ora. 

5. Usare i filtri per trovare le prenotazioni di Azure nelle macchine virtuali che soddisfano i requisiti del cliente.  

6. Dopo aver trovato le prenotazioni da acquistare, immettere il numero di istanze riservate necessarie per il cliente in **Quantity** e quindi selezionare **Aggiungi al carrello.**  

7. Ripetere i passaggi 5 e 6 fino a quando non sono stati aggiunti tutti gli elementi necessari all'ordine. Seleziona **Rivedi** per verificare che il tuo ordine sia corretto.  

8. Nella **pagina Rivedi gli** ordini è possibile: 

    - Verificare o modificare la quantità di istanze riservate.

    - Selezionare l'ambito della prenotazione. L'ambito della prenotazione può coprire una o più sottoscrizioni (ambito condiviso). Se si applica l'ambito della prenotazione a una singola sottoscrizione, lo sconto per la prenotazione viene applicato solo a questa sottoscrizione. Se si seleziona condiviso, lo sconto per la prenotazione viene applicato a tutte le sottoscrizioni all'interno del contesto di fatturazione del cliente. 

      >[!NOTE] 
      >Se si sceglie di limitare l'ambito della prenotazione a una singola sottoscrizione di Azure, potrebbe essere necessario aumentare la quota di vCPU della sottoscrizione. Per aumentare la quota di vCPU della sottoscrizione, è necessario creare una richiesta di supporto nel portale di Azure. Seguire le istruzioni [in questo argomento](/azure/azure-supportability/resource-manager-core-quotas-request) per creare la richiesta. 

      >[!NOTE]   
      >Se il cliente è nell'ambito del piano di Azure, **l'ambito** verrà impostato su **Condiviso.** 

    - Se si è un partner provider, selezionare il rivenditore da associare al prodotto.
    
    - Se la prenotazione di Azure supporta l'opzione Piano di fatturazione, è possibile selezionare la frequenza di fatturazione mensile dal menu a discesa. 
    - Se la prenotazione di Azure non supporta l'opzione Piano di fatturazione, per impostazione predefinita la frequenza di fatturazione viene impostata sulla fatturazione una sola volta. 

9. Selezionare **Acquista per** acquistare l'ordine. I dettagli dell'ordine, incluso il numero di ordine, vengono visualizzati nella **pagina Conferma.** Seleziona **Fatto** per passare alla pagina **Cronologia ordini**. 

10. Per gestire la prenotazione del cliente nell'portale di Azure,  trovare il cliente nella pagina Clienti e quindi selezionare la freccia rivolta verso il basso per espandere la riga del cliente. Selezionare **portale di gestione di Microsoft Azure** per aprire il record del cliente nella portale di Azure.

## <a name="next-steps"></a>Passaggi successivi

|**Per informazioni su**   |**Leggi**    |
|:-----------------------------|:-----------------|
|Panoramica delle prenotazioni di Azure in CSP  | [Vendere Microsoft Azure istanze riservate](azure-reservations.md) |
|Gestione delle prenotazioni di Azure in Partner Center | [Gestione delle prenotazioni di Azure in Partner Center](azure-reservations-manage.md)
|Determinare le dimensioni corrette della macchina virtuale e verificare l'utilizzo della macchina virtuale del cliente   |[Ridimensionamento delle macchine virtuali per l'utilizzo massimo delle prenotazioni di Azure](azure-usage.md)   |
|Acquisto di prenotazioni di Azure tramite l'API Partner Center azure | [Acquistare istanze di macchine virtuali riservate di Azure](/partner-center/develop/purchase-azure-reservations) nella documentazione Partner Center per sviluppatori   |
|Concedere ai clienti l'autorizzazione per acquistare le proprie prenotazioni di Azure  | [Concedere ai clienti l'autorizzazione per acquistare le proprie prenotazioni di Azure](give-customers-permission.md)  |