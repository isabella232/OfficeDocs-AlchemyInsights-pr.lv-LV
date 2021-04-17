---
title: Rezervācijas atcelšana
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003552"
- "6817"
ms.openlocfilehash: 6b27344b43aa5c20d64d148ff164be805f3b5ef8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819699"
---
# <a name="cancelling-reservation"></a>Rezervācijas atcelšana

- **Patstāvīgi izpildāms:** jūs varat atcelt vai mainīt rezervēto instanci pats, izmantojot [Azure portālu](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Atlasiet rezervāciju un noklikšķiniet uz atmaksāt vai mainīt. Ņemiet vērā, ka jums ir jābūt īpašnieka piekļuvei rezervācijas pasūtījumam, lai to mainītu vai veiktu atmaksu. Tikai piekļuve rezervācijai neļaus jums veikt atmaksu vai maiņu. Lūdziet rezervācijas pasūtījuma īpašnieku piešķirt jums īpašnieka piekļuvi rezervācijas pasūtījumam.
- **Maiņās politika:** jūs varat mainīt rezervāciju pret citu tāda paša tipa rezervāciju – par rezervāciju maiņu **sodi netiek piemēroti**. Jaunās rezervācijas kopsummai ir jābūt lielākai par mainītās rezervācijas atmaksājamo summu un plānotajiem mēneša maksājumiem (ja attiecināms)
- **Atmaksas politika:** atmaksas un atcelto tālāko maksājumu kopsumma nedrīkst pārsniegt 50 000 ASV dolāru 12 mēnešu periodā. Mēs **pašlaik nepiemērojam soda naudas** atmaksai, bet tas var mainīties nākotnē  
    **Izņēmumi:** patstāvīgi izpildāmās maiņas un atcelšanas funkcijas nav pieejamas ASV valdības Enterprise līguma klientiem
- **API / PS / CLI** atbalstu nav iespējams atcelt un atmaksāt, [patstāvīgi veicot Azure rezervāciju maiņu un atmaksu](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Patstāvīgi izpildāmās maiņas un atcelšanas funkcijas nav pieejamas ASV valdības Enterprise līguma klientiem. Tiek atbalstīti citi ASV valdības abonementu veidi, tai skaitā Pay-As-You-Go un CSP

Papildinformācija: [Kā tiek apstrādāti atgriešanas un maiņas pieprasījumi](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Papildinformācija: [Maiņas un atmaksas politikas](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Citi jautājumi: [Rezervēto lietojumprogrammu dokumentu skatīšana](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Esošās rezervētās lietojumprogrammas maiņa (patstāvīga izpilde)**

Jūs varat mainīt rezervāciju pret tāda paša tipa rezervāciju. Ja rezervācija jums vairs nav nepieciešama, jūs varat saņemt naudas atmaksu līdz 50 000 ASV dolāru gadā. Patstāvīgi izpildāmās maiņas un atcelšanas funkcijas nav pieejamas ASV valdības Enterprise līguma klientiem. Tiek atbalstīti citi ASV valdības abonementu veidi, tai skaitā Pay-As-You-Go un CSP. Jums ir jābūt īpašnieka piekļuvei rezervācijas pasūtījumam, lai mainītu esošo rezervāciju vai veiktu atmaksu.

Tālāk aprakstītās darbības palīdzēs jums veikt atbilstošo procedūru.

1. Pierakstieties savā [Azure portālā](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Atlasiet rezervāciju, par kuru vēlaties saņemt atmaksu, un noklikšķiniet uz **Mainīt**
2. Atlasiet VM produktu, kuru vēlaties iegādāties, un ierakstiet daudzumu. Pārliecinieties par to, ka jaunā pirkuma summa ir lielāka par atmaksājamo summu. [Nosakiet īsto daudzumu pirms pirkuma veikšanas](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. Pārskatiet un pabeidziet darījumu

**Rezervētas lietojumprogrammas atmaksa**

Lai saņemtu atmaksu par rezervāciju, atveriet **Rezervācijas detalizētā informācija** un noklikšķiniet uz **Atmaksāt**

**Novērtētā atmaksa:**

**Atmaksas un maiņas novērtējuma un minimālo prasību piemēri**  
Tiešās rezervācijas piemērs:

- 1. janvārī jūs uz gadu iegādājāties RI par 120 ASV dolāriem 
- 7. aprīlī jūs nolēmāt atmaksāt vai mainīt šo rezervāciju
- Ņemot vērā, ka šī rezervācija bija aktīva 97 dienas, jūs saņemsiet atmaksu (1-97/365) * 120 $ apmērā. (t.i. 88,10 $). Pašlaik atmaksai sodi netiek piemēroti.
- Veicot maiņu, jaunās rezervācijas vērtībai ir jābūt lielākai par 88,10 $.
- Pašlaik atmaksai sodi netiek piemēroti

**Rezervācijas maksājumu plāna piemērs:**

- Jūs uz gadu iegādājāties RI ar mēneša maksājumu 10 ASV dolāru apmērā
- 7. aprīlī jūs nolēmāt atmaksāt vai mainīt šo rezervāciju
- Ņemot vērā, ka pēdējais maksājums tika veikts pirms 7 dienām, jūs saņemsiet atmaksu (1-7/31) * 10 $ apmērā. (t.i. 7,74 $).
- Atcelto nākotnes maksājumu summa ir 80 $. Pašlaik atmaksai sodi netiek piemēroti.
- Šīs atcelšanas rezultātā jūsu atmaksas limits 50 000 ASV dolāru apmērā tiks samazināts par 87,74 ASV dolāriem
- Veicot maiņu, jaunās rezervācijas vērtībai ir jābūt lielākai par 87,74 $.

**Ieteiktie dokumenti**

- [Kā tiek apstrādāti atgriešanas un maiņas pieprasījumi](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Maiņas un atmaksas politikas](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)