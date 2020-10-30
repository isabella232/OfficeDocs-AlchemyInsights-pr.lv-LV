---
title: Atcelt rezervāciju
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003552"
- "6817"
ms.openlocfilehash: 04875e33f07c6d0a4306b3579ef81f2d28c7f506
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807569"
---
# <a name="cancelling-reservation"></a>Atcelt rezervāciju

- Pašapkalpošanās **:** Jūs varat atcelt vai Exchange rezervētu instanci, izmantojot [Azure Portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Atlasiet rezervāciju un noklikšķiniet uz atmaksāšana vai Exchange. Ņemiet vērā, ka rezervēšanas pasūtījumā jābūt piešķirtai īpašnieka piekļuvei, lai veiktu apmaiņu vai atmaksu. Piekļuve tikai rezervācijai neļaus turpināt atmaksāšanu vai Exchange. Uzdodiet rezervēšanas pasūtījuma īpašniekam, lai piešķirtu īpašniekam piekļuvi rezervēšanas pasūtījumam
- **Exchange politika:** Jūs varat apmainīties ar rezervāciju ar citu tā paša tipa rezervāciju – **nav sodu** par rezervēšanas Exchange. Kopējās saistības ar jauno rezervāciju ir lielākas par apmainītās rezervācijas atmaksāšanas summu un nākamajiem mēneša maksājumiem (ja piemērojams)
- **Atmaksas politika:** Atmaksāšanas summa un anulētie turpmākie maksājumi nedrīkst pārsniegt $50 000 USD 12 mēnešu slīdošajā logā. Šobrīd mēs **neiekasējam sodu** par kompensācijām, bet varētu to iekasēt par turpmākām kompensācijām  
    **Izņēmumi:** Pašapkalpošanās Exchange un atcelšanas iespēja nav pieejama ASV valsts iestādes līgumu klientiem
- **API/PS/CLI** atbalsts nav pieejams atcelšanas un atmaksas [pašapkalpošanās apmaiņā un atmaksām Azure rezervācijām](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Pašapkalpošanās Exchange un atcelšanas iespēja nav pieejama ASV valsts iestādes līgumu klientiem. Citi ASV valdības abonementa tipi, tostarp maksātāja un CSP līdzekļi, tiek atbalstīti

Papildinformācija: [kā tiek apstrādāti atdošanas un Exchange transakciju](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Papildinformācija: [Exchange un atmaksas politikas](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Citi jautājumi: [apmeklēt rezervētas instances dokumentus](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Esošas rezervētas instances apmaiņa (pašapkalpošanās)**

Jūs varat apmainīties ar rezervāciju ar citu tāda paša tipa rezervāciju. Jūs arī varat atmaksāt rezervāciju līdz $50 000 USD gadā, ja tas vairs nav vajadzīgs. Pašapkalpošanās Exchange un atcelšanas iespēja nav pieejama ASV valsts iestādes līgumu klientiem. Tiek atbalstīti citi ASV valsts valdības abonementa tipi, tostarp Pay-GO un CSP. Lai apmainītos vai atmaksātu esošo rezervāciju, jums ir jābūt īpašnieka piekļuvei.

Tālāk norādītās darbības palīdzēs izpildīt darbību

1. Piesakieties savā [Azure portālā](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Atlasiet rezervācijas, kuras vēlaties atmaksāt, un noklikšķiniet uz **Exchange**
2. Atlasiet VM produktu, kuru vēlaties iegādāties, un ierakstiet daudzumu. Pārliecinieties, vai jaunā pirkšanas summa ir lielāka par atgriežamo kopsummu [pirms iegādes noteikt pareizo lielumu](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. Darījuma pārskatīšana un Pabeigšana

**Atmaksa rezervētā instancē**

Lai atmaksātu rezervāciju, dodieties uz **informāciju par rezervāciju** un noklikšķiniet uz **atmaksa**

**Pro-rated atmaksa:**

**Līdzekļu un minimālās prasības attiecībā uz atmaksu un apmaiņu**  
Sākotnējās rezervācijas piemērs:

- Jūs iegādājaties vienu gadu ilgu termiņu RI $120 janvārī 1
- 7. aprīlī jūs vēlaties atmaksāt vai apmainīt šo rezervāciju
- Tā kā rezervējums ir nodzīvots 97 dienas, jūs saņemsit (1-97/365) * $120 atpakaļ. (piemēram, $88,1). Par kompensācijām pašlaik nav soda
- Ja apmaināties, jaunajam pirkumam jābūt lielākam par $88,1
- Pašlaik nav soda par kompensācijām

**Norēķinu plāna rezervēšanas piemērs:**

- Jūs iegādājaties vienu gadu ilgu termiņu RI $10 mēnesī
- 7. aprīlī jūs vēlaties atmaksāt vai apmainīt šo rezervāciju
- Tā kā pēdējais maksājums ir noticis 7 dienas, jūs iegūstat (1-7/31) * $10 atpakaļ. (piemēram, $7,74)
- Turpmākie maksājumi anulēti ir $80. Par kompensācijām pašlaik nav soda
- Šis atsaukums atskaitīs $87,74 no jūs esat $50 000 atmaksas limits
- Ja apmaināties, jaunā pirkuma kopējā vērtība ir lielāka par $87,74

**Ieteicamie dokumenti**

- [Kā tiek apstrādāti atdošanas un Exchange darījumi](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Exchange un atmaksas politikas](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)