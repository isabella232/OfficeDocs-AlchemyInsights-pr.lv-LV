---
title: Norēķini rezervētas instances pirkumam
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
ms.openlocfilehash: 9d71554d2089a6d9e5d4850149d113959f3d43c0
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820329"
---
# <a name="billing-for-reserved-instance-purchase"></a>Norēķini rezervētas instances pirkumam

Rezervētais instances pirkums tiek iekasēts no maksāšanas metodes, kas saistīts ar iegādes brīdī atlasītu abonementu. Abonementa veidam jābūt uzņēmuma līgumam (piedāvājuma numurs: MS-AZR-0017P), Pay-As-You-Go (piedāvājuma numurs: MS-AZR-0003P), Microsoft klienta līgumam vai CSP.

- Ja izmantojat uzņēmuma abonementu, izmaksas tiek iekasētas no reģistrācijas finanšu saistību atlikuma vai tiek iekasētas kā pārpildība
- Ja izmantojat abonementu Pay-As-You-Go, maksa tiek piemērota kredītkartei vai rēķina maksāšanas metodei abonementā.

**Notiek rezervācijas atcelšana**

- **Pašapkalpošanās:** Varat atcelt vai apmainīt rezervēto instanci pats, izmantojot [Azure portālu.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Atlasiet rezervāciju un noklikšķiniet uz atmaksas vai maiņas vienuma. Ņemiet vērā, ka jums ir jābūt īpašnieka piekļuvei rezervācijas pasūtījumā, lai veiktu apmaiņu vai atmaksu. Piekļuve tikai rezervācijai neļauj turpināt ar atmaksu vai apmaiņu. Lūdziet rezervācijas pasūtījuma īpašniekam piešķirt jums īpašniekam piekļuvi rezervācijas pasūtījumam
- **Exchange politika:** Varat veikt rezervāciju citai tāda paša tipa rezervācijai — rezervēšanas apmaiņas **gadījumā nav** atrunas. Kopējām saistībām ar jaunu rezervāciju jābūt lielākām par apmainīto rezervāciju atmaksas summu un turpmākajiem ikmēneša maksājumiem (ja tādi ir)
- **Atmaksas politika:** Atmaksas summa un atceltie turpmākie maksājumi nevar pārsniegt 50 000 ASV dolārus 12 mēnešu slīdošā logā. Mēs pašlaik **neie iekasējam maksu atmaksas** gadījumā, bet mēs varētu iekasēt maksu par turpmākām atmaksām

**Izņēmumi:** Self-service exchange and cancel capability isn't available for US Government Enterprise Agreement customers

- **API/PS/CLI atbalsts** nav pieejams atcelšanai un atmaksai pašapkalpošanās apmaiņa un atmaksa [Azure rezervācijai](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Self-service exchange and cancel capability isn't available for US Government Enterprise Agreement customers. Tiek atbalstīti citi ASV valsts iestāžu abonementu tipi, tostarp Pay-As-You-Go un CSP.

Papildinformācija: [Kā tiek apstrādātas atgriešanas un](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) apmaiņas transakcijas. Papildinformācija: Exchange un [atmaksas politikas](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) Citi jautājumi: apmeklējiet [rezervētos instanci dokumentus](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Esošas rezervētas instances apmaiņa (pašapkalpošanās)**

Varat veikt rezervāciju citai tāda paša tipa rezervācijai. Varat arī atmaksāt rezervāciju līdz pat 50 000 USD gadā, ja tas vairs nav nepieciešams. Self-service exchange and cancel capability isn't available for US Government Enterprise Agreement customers. Tiek atbalstīti citi ASV valsts iestāžu abonementu tipi, tostarp Pay-As-You-Go un CSP. Lai apmainītos vai atmaksātu esošu rezervāciju, jums ir jābūt īpašnieka piekļuvei rezervācijas pasūtījumā.

Tālāk norādītās darbības sniegs norādījumus par transakcijas pabeigšanas procedūru.

1.Piesakieties savā [Azure portālā](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Atlasiet rezervāciju, kuru vēlaties atmaksāt, un noklikšķiniet uz **Exchange** 2.Atlasiet VM produktu, kuru vēlaties iegādāties, un ierakstiet daudzumu. Pārliecinieties, vai jaunā pirkuma kopsumma pārsniedz atgriežamā apjoma vērtību Pirms iegādes [nosakiet pareizo lielumu.](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3.Pārskatiet un pabeidziet transakciju

**Atmaksa rezervētai instancei**

Lai atmaksātu rezervāciju, dodieties uz **sadaļu Rezervācijas informācija** un noklikšķiniet uz **Atmaksa**

**Pro-rated refund:**

**Pro-ration and minimum requirement examples for refund and exchange** Iepriekš veikta rezervācijas piemērs:

- Jūs iegādājaties viena gada termiņu RI par 120 USD 1. janvārī
- 7. aprīlī jūs vēlaties atmaksāt vai apmainīt šo rezervāciju
- Tā kā rezervācija tika veikta 97 dienas, jūs saņemsiet (1-97/365) * 120 EUR atpakaļ. (piemēram, 88,1 EUR). Šobrīd atmaksas gadījumā nav pieejams
- Apmaiņas gadījumā jūsu jaunajam pirkumam vajadzētu būt lielākam par 88,1 USD
- Šobrīd atmaksa nav pieejama

**Norēķinu plāna rezervēšanas piemērs:**

- Jūs iegādājaties viena gada termiņu RI par 10 USD mēnesī
- 7. aprīlī jūs vēlaties atmaksāt vai apmainīt šo rezervāciju
- Tā kā pēdējais maksājums tika veikts 7 dienas, jūs saņemsiet (1-7/31) * 10 EUR atpakaļ. (t.i., 7,74 $)
- Atceltie turpmākie maksājumi būs 80 EUR. Šobrīd atmaksas gadījumā nav pieejams
- Šī atcelšana no jums saņems 87,74 ASV dolārus par 50 000 USD atmaksas ierobežojumu
- Ja jaunu pirkumu kopsummai vajadzētu būt lielākai par 87,74 USD

**Nevar skatīt rēķinu par pēdējo norēķinu periodu**

Daži iespējamie iemesli, kāpēc neredzat rēķinu:

- Abonementam jums ir ikmēneša kredīta summa, ko nepārsniedzat vai jums ir bezmaksas izmēģinājumversija. Rēķins tiek ģenerēts tikai tad, ja no jums ir parādāmā nauda
- Ir mazāk nekā 30 dienas pēc Azure abonementa abonementa dienas
- Rēķins vēl nav ģenerēts. Uzgaidiet līdz norēķinu perioda beigām
- Ja neesat konta administrators, iespējams, jums nebūs pieejami vecāki rēķini

**Lejupielādējiet rēķinu no Azure portāla (.pdf)**

- Atlasiet savu abonementu abonementu [lapā](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) Azure portālā kā lietotājs [ar piekļuvi rēķiniem](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Select **Invoices**
- Noklikšķiniet **uz Lejupielādēt rēķinu,** lai skatītu sava PDF rēķina kopiju. Ja ir **rakstīts Nav** pieejams, [skatiet rakstu Kāpēc nav redzams rēķins par pēdējo norēķinu periodu?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

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

Citi jautājumi: [Apmeklējiet rezervētos instances dokumentus](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Ieteiktie dokumenti**

- [Norēķinu pamati](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Izpratne par to, kā tiek lietota rezervētas instances atlaide](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure norēķinu rēķina un dienas lietojuma datu lejupielāde vai skatīšana](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Izpratne par to, kā tiek lietota rezervētas instances atlaide](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Izprast rezervēto instanci lietojumu jūsu Pay-As-You-Go abonementam](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Saprotiet rezervēto instanci lietojumu jūsu Enterprise reģistrācijai](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Windows programmatūras izmaksas, kas nav iekļautas rezervēto instanču gadījumā](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Rezervētas instances partneru centrālā mākoņrisinājumu nodrošinātāja (Csp) programmā](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)