---
title: Norēķini par rezervētas instances iegādi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 6cdcb5af27a475cc838eb434ff025eb18356360c
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823079"
---
# <a name="billing-for-reserved-instance-purchase"></a>Norēķini par rezervētas instances iegādi

Rezervētā gadījuma pirkums ir uzlādēts līdz maksāšanas metodei, kas ir piesaistīta abonementam, kuru atlasāt iegādes brīdī. Abonementa tipam ir jābūt uzņēmuma līgumam (piedāvājuma numurs: MS-AZR-0017P), pay-as-GO (piedāvājuma numurs: MS-AZR-0003P), Microsoft klienta līgums vai CSP.

- Enterprise abonementā maksa tiek atskaitīta no reģistrācijas naudas summas atlikuma vai apmaksāts kā pārsniegts
- Par pay-as-Go abonementu, maksa tiek izrakstīta ar kredītkarti vai rēķina apmaksas metodi abonementā

**Atcelt rezervāciju**

- Pašapkalpošanās **:** Jūs varat atcelt vai Exchange rezervētu instanci, izmantojot [Azure Portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Atlasiet rezervāciju un noklikšķiniet uz atmaksāšana vai Exchange. Ņemiet vērā, ka rezervēšanas pasūtījumā jābūt piešķirtai īpašnieka piekļuvei, lai veiktu apmaiņu vai atmaksu. Piekļuve tikai rezervācijai neļaus turpināt atmaksāšanu vai Exchange. Uzdodiet rezervēšanas pasūtījuma īpašniekam, lai piešķirtu īpašniekam piekļuvi rezervēšanas pasūtījumam
- **Exchange politika:** Jūs varat apmainīties ar rezervāciju ar citu tā paša tipa rezervāciju – **nav sodu** par rezervēšanas Exchange. Kopējās saistības ar jauno rezervāciju ir lielākas par apmainītās rezervācijas atmaksāšanas summu un nākamajiem mēneša maksājumiem (ja piemērojams)
- **Atmaksas politika:** Atmaksāšanas summa un anulētie turpmākie maksājumi nedrīkst pārsniegt $50 000 USD 12 mēnešu slīdošajā logā. Šobrīd mēs **neiekasējam sodu** par kompensācijām, bet varētu to iekasēt par turpmākām kompensācijām

**Izņēmumi:** Pašapkalpošanās Exchange un atcelšanas iespēja nav pieejama ASV valsts iestādes līgumu klientiem

- **API/PS/CLI** atbalsts nav pieejams atcelšanas un atmaksas [pašapkalpošanās apmaiņā un atmaksām Azure rezervācijām](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Pašapkalpošanās Exchange un atcelšanas iespēja nav pieejama ASV valsts iestādes līgumu klientiem. Citi ASV valdības abonementa tipi, tostarp maksātāja un CSP līdzekļi, tiek atbalstīti

Papildinformācija: [kā tiek apstrādāti atgriešanas un Exchange transakciju](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) Papildinformācija: [Exchange un atmaksas politikas](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) citi jautājumi: [apmeklēt rezervēto gadījumu dokumentus](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Esošas rezervētas instances apmaiņa (pašapkalpošanās)**

Jūs varat apmainīties ar rezervāciju ar citu tāda paša tipa rezervāciju. Jūs arī varat atmaksāt rezervāciju līdz $50 000 USD gadā, ja tas vairs nav vajadzīgs. Pašapkalpošanās Exchange un atcelšanas iespēja nav pieejama ASV valsts iestādes līgumu klientiem. Tiek atbalstīti citi ASV valsts valdības abonementa tipi, tostarp Pay-GO un CSP. Lai apmainītos vai atmaksātu esošo rezervāciju, jums ir jābūt īpašnieka piekļuvei.

Tālāk norādītās darbības palīdzēs izpildīt darbību

1. Piesakieties savā [Azure portālā](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Atlasiet rezervācijas, kuras vēlaties atmaksāt, un noklikšķiniet uz **Exchange** 2. Atlasiet VM produktu, kuru vēlaties iegādāties, un ierakstiet daudzumu. Pārliecinieties, vai jaunā pirkumu summa ir lielāka par atgriežamo kopsummu, [pirms iegādes noteikt pareizo lielumu](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3. Pārskatiet un pabeidziet transakciju

**Atmaksa rezervētā instancē**

Lai atmaksātu rezervāciju, dodieties uz **informāciju par rezervāciju** un noklikšķiniet uz **atmaksa**

**Pro-rated atmaksa:**

Līdzekļu **un minimālās prasības attiecībā uz atmaksu un apmaiņu** Sākotnējās rezervācijas piemērs:

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

**Nevar skatīt rēķinu par pēdējo norēķinu periodu**

Daži iespējamie iemesli, kāpēc jūs, iespējams, neredzat rēķinu:

- Jums ir mēneša kredīta summa ar abonementu, par kuru neesat pārsniedzis, vai jums ir bezmaksas izmēģinājums. Rēķins tiek ģenerēts tikai tad, ja esat parādā naudu
- Tas ir mazāks par 30 dienām no dienas, kad esat abonējis Azure
- Rēķins vēl nav ģenerēts. Uzgaidiet līdz norēķinu perioda beigām
- Ja neesat konta administrators, jums var nebūt pieejami vecāki rēķini

**Rēķinu lejupielāde no Azure Portal (. PDF)**

- Azure portāla lapā [abonementi](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) atlasiet savu abonementu kā [lietotājs, kuram ir piekļuve rēķiniem](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Atlasiet **rēķini**
- Lai skatītu PDF rēķina kopiju, noklikšķiniet uz **lejupielādēt rēķinu** . Ja tiek rādīts ziņojums **nav pieejams** , skatiet rakstu [Kāpēc nav redzams rēķins par pēdējo norēķinu periodu?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Rēķina saņemšana pa e-pastu (. PDF)**

- Lapā [abonementi](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) atlasiet savu abonementu. Noklikšķiniet uz **rēķini** , pēc tam e-pasts mans rēķins
- Noklikšķiniet uz **izvēlēties** un akceptējiet noteikumus. Jums būs jāpiesakās katram abonementam

Piezīme. Ja pēc darbību veikšanas nesaņemat e-pasta ziņojumu, pārliecinieties, vai jūsu e-pasta adrese ir pareiza [saziņas preferencēs savā profilā](https://account.windowsazure.com/profile)

**Savu lietojuma datu lejupielāde Azure portālā**

- Pierakstīšanās [Azure kontu centrā](https://account.windowsazure.com/Subscriptions) kā [konta administrators](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Atlasiet abonementu, kuram vēlaties izmantot rēķinu un lietojuma informāciju
- **Norēķinu vēstures** atlase
- Atlasiet **Skatīt pašreizējo priekšrakstu** , lai skatītu savu maksu novērtējumu laikā, kad tika ģenerēts novērtējums
- Atlasiet **lejupielādēt lietojumu** , lai lejupielādētu ikdienas lietojuma datus kā CSV failu. Ja redzat divas versijas, lejupielādējiet versiju 2

Citi jautājumi: [apmeklēt rezervētas instances dokumentus](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Ieteicamie dokumenti**

- [Norēķinu pamati](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Izpratne par rezervētās instances atlaides lietošanu](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure norēķinu rēķinu un dienas lietojuma datu lejupielāde vai skatīšana](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Izpratne par rezervētās instances atlaides lietošanu](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Izprotiet rezervētās instances izmantošanu jūsu pay-as-Go abonementam](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Par rezervētas instances izmantošanu uzņēmuma reģistrācijai](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Windows programmatūras izmaksas nav iekļautas rezervētajos gadījumos](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Rezervētie gadījumi partneru centrālā mākoņa risinājumu pakalpojumu sniedzēja (CSP) programmā](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)