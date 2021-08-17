---
title: Rezervētās instances pirkuma norēķini
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 00565470de388165e64c45879c22fd5064b4adc695151edaf58878f38a481ff2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104027"
---
# <a name="billing-for-reserved-instance-purchase"></a>Rezervētās instances pirkuma norēķini

Maksa par rezervētās instances pirkumu tiks iekasēta no maksāšanas metodes, kas saistīta abonementu, kuru atlasāt iegādes brīdī. Abonementa tipam ir jābūt uzņēmuma līgumam (piedāvājuma numurs: MS-AZR-0017P), priekšapmaksas līgumam (piedāvājuma numurs: MS-AZR-0003P), Microsoft klienta līgumam vai Microsoft mākoņrisinājumu nodrošinātājam.

- Maksa par uzņēmuma abonementu tiek iekasēta no reģistrācijas finanšu saistību atlikuma vai arī kā pārsnieguma maksa
- Ja izmantojat priekšapmaksas abonementu, maksa tiek iekasēta no abonementa kredītkartes vai rēķina maksāšanas metodes

**Rezervācijas atcelšana**

- **Patstāvīgi izpildāms:** jūs varat atcelt vai mainīt rezervēto instanci pats, izmantojot [Azure portālu](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Atlasiet rezervāciju un noklikšķiniet uz atmaksāt vai mainīt. Ņemiet vērā, ka jums ir jābūt īpašnieka piekļuvei rezervācijas pasūtījumam, lai to mainītu vai veiktu atmaksu. Tikai piekļuve rezervācijai neļaus jums veikt atmaksu vai maiņu. Lūdziet rezervācijas pasūtījuma īpašnieku piešķirt jums īpašnieka piekļuvi rezervācijas pasūtījumam.
- **Maiņās politika:** jūs varat mainīt rezervāciju pret citu tāda paša tipa rezervāciju – par rezervāciju maiņu **sodi netiek piemēroti**. Jaunās rezervācijas kopsummai ir jābūt lielākai par mainītās rezervācijas atmaksājamo summu un plānotajiem mēneša maksājumiem (ja attiecināms)
- **Atmaksas politika:** atmaksas un atcelto tālāko maksājumu kopsumma nedrīkst pārsniegt 50 000 ASV dolāru 12 mēnešu periodā. Mēs **pašlaik nepiemērojam soda naudas** atmaksai, bet tas var mainīties nākotnē

**Izņēmumi:** patstāvīgi izpildāmās maiņas un atcelšanas funkcijas nav pieejamas ASV valdības Enterprise līguma klientiem

- **API / PS / CLI** atbalstu nav iespējams atcelt un atmaksāt, [patstāvīgi veicot Azure rezervāciju maiņu un atmaksu](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Patstāvīgi izpildāmās maiņas un atcelšanas funkcijas nav pieejamas ASV valdības Enterprise līguma klientiem. Tiek atbalstīti citi ASV valdības abonementu veidi, tai skaitā Pay-As-You-Go un CSP

Papildinformācija. [Kā tiek apstrādātas atgriešanas](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) un apmaiņas transakcijas Papildinformācija: Exchange [atmaksas](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) politikas un Atmaksas politikas Citi jautājumi: Apmeklējiet [rezervētos instanci dokumentus](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Esošās rezervētās lietojumprogrammas maiņa (patstāvīga izpilde)**

Jūs varat mainīt rezervāciju pret tāda paša tipa rezervāciju. Ja rezervācija jums vairs nav nepieciešama, jūs varat saņemt naudas atmaksu līdz 50 000 ASV dolāru gadā. Patstāvīgi izpildāmās maiņas un atcelšanas funkcijas nav pieejamas ASV valdības Enterprise līguma klientiem. Tiek atbalstīti citi ASV valdības abonementu veidi, tai skaitā Pay-As-You-Go un CSP. Jums ir jābūt īpašnieka piekļuvei rezervācijas pasūtījumam, lai mainītu esošo rezervāciju vai veiktu atmaksu.

Tālāk aprakstītās darbības palīdzēs jums veikt atbilstošo procedūru.

1.Piesakieties savā [Azure portālā](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Atlasiet rezervāciju, kuru vēlaties atmaksāt, un **noklikšķiniet uz Exchange** 2.Atlasiet VM produktu, kuru vēlaties iegādāties, un ierakstiet daudzumu. Pārliecinieties, vai jaunā pirkuma kopsumma pārsniedz atgriežamā apjoma vērtību Pirms iegādes [nosakiet pareizo lielumu.](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3.Pārskatiet un pabeidziet transakciju

**Rezervētas lietojumprogrammas atmaksa**

Lai saņemtu atmaksu par rezervāciju, atveriet **Rezervācijas detalizētā informācija** un noklikšķiniet uz **Atmaksāt**

**Novērtētā atmaksa:**

**Pro-ration and minimum requirement examples for refund and exchange** Iepriekš veikta rezervācijas piemērs:

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

**Nevar skatīt rēķinu par pēdējo norēķinu periodu**

Daži iespējamie iemesli, kāpēc neredzat rēķinu:

- Abonementam jums ir ikmēneša kredīta summa, ko nepārsniedzat vai jums ir bezmaksas izmēģinājumversija. Rēķins tiek ģenerēts tikai tad, ja no jums ir parādāmā nauda
- Ir mazāk nekā 30 dienas pēc Azure abonementa abonementa dienas
- Rēķins vēl nav ģenerēts. Uzgaidiet līdz norēķinu perioda beigām
- Ja neesat konta administrators, iespējams, jums nebūs pieejami vecāki rēķini

**Lejupielādēt rēķinu no Azure portāla (.pdf)**

- Atlasiet savu abonementu abonementu [lapā](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) Azure portālā kā lietotājs [ar piekļuvi rēķiniem](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Select **Invoices**
- Noklikšķiniet uz **Lejupielādēt rēķinu**, lai skatītu sava PDF rēķina kopiju. Ja tiek parādīts ziņojums **Nav pieejams**, skatiet rakstu [Kāpēc es neredzu rēķinu par pēdējo norēķinu periodu?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Rēķina saņemšana e-pasta ziņojumā (.pdf)**

- Lapā Abonementi atlasiet [savu](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) abonementu. Noklikšķiniet uz **Rēķini, pēc** tam uz Nosūtīt rēķinu e-pastā
- Noklikšķiniet **uz Piekrist** un piekrītiet noteikumiem. Jums būs jāpiesakās katram abonementam, kas jums pieder.

Piezīme. Ja pēc darbību veikšanas nesaņemsiet e-pasta ziņojumu, pārliecinieties, vai jūsu e-pasta adrese ir pareiza saziņas [preferencēs jūsu profilā.](https://account.windowsazure.com/profile)

**Lietojuma datu lejupielāde no Azure portāla**

- Sign into the [Azure Account Center](https://account.windowsazure.com/Subscriptions) as the Account [Admin](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Atlasiet abonementu, par kuru vēlaties saņemt informāciju par rēķinu un lietojumu
- Atlasiet **Norēķinu vēsture**
- Atlasiet **Skatīt pašreizējo priekšrakstu,** lai redzētu jūsu izmaksu novērtējumu brīdī, kad tika ģenerēts aprēķins
- Atlasiet **Lejupielādēt lietojumu,** lai lejupielādētu dienas lietojuma datus kā CSV failu. Ja ir redzamas divas pieejamās versijas, lejupielādējiet 2. versiju

Citi jautājumi: [Rezervēto lietojumprogrammu dokumentu skatīšana](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Ieteiktie dokumenti**

- [Norēķinu pamati](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Izpratne par to, kā tiek lietota rezervētas instances atlaide](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure norēķinu rēķina un dienas lietojuma datu lejupielāde vai skatīšana](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Izpratne par to, kā tiek lietota rezervētas instances atlaide](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Izprast rezervēto instanci lietojumu jūsu Pay-As-You-Go abonementam](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Saprotiet rezervēto instanci lietojumu jūsu Enterprise reģistrācijai](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Windows programmatūras izmaksas, kas nav iekļautas rezervēto instanču komplektācijā](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Rezervētas instances partneru centrālās Microsoft mākoņrisinājumu nodrošinātājs (CSP) programmā](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)