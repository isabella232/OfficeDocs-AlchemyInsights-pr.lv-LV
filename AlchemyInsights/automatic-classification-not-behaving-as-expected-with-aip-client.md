---
title: Izmantojot AIP klientu, automātiskā klasifikācija nedarbojas, kā paredzēts
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
- "9002266"
- "4373"
ms.openlocfilehash: b7ab09fe8430a54dacf2cd1ba076414a5f562541
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820905"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Izmantojot AIP klientu, automātiskā klasifikācija nedarbojas, kā paredzēts

Automātiskā klasifikācija nedarbojas, kā paredzēts; izmantojiet šīs ieteicamās vadlīnijas:

1. Ja rodas problēmas ar automātisko etiķešu pievienošanu, skatiet rakstu [Kā konfigurēt pakalpojuma Azure informācijas aizsardzība automātiskās un ieteicamās klasifiācijas nosacījumus](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) un [Kādus sensitīvas informācijas tipus meklēt](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
2. Pārbaudiet, vai neizmantojat tvēruma politikas, kas nav pareizi konfigurētas: [Kā konfigurēt pakalpojuma Azure informācijas aizsardzība politiku konkrētiem lietotājiem, izmantojot tvēruma politikas](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Ja, pievienojot dokumentu ar tam pievienotu etiķeti, programmā Outlook nedarbojas automātiskā etiķešu pievienošana, pārliecinieties, vai `DRMEncryptProperty` nav definēts, kā aprakstīts šeit: [IRM reģistra iestatījumi drošībai](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Ja savai pakalpojuma Azure informācijas aizsardzība politikai izmantojāt [iebūvētos tipus](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b), pārbaudiet, vai jūsu saturs atbilst sagaidāmajam formātam.
5. Pārliecinieties, vai etiķete ir pareizi konfigurēta **automātiskajai** vai **ieteicamajai** etiķešu pievienošanai. (**Automātiskā** etiķešu pievienošana ir pieejama visām Microsoft 365 programmām, bet **ieteicamā** etiķešu pievienošana ir pieejama visām Microsoft 365 programmām, izņemot Outlook.)
6. Jūs nevarat izmantot automātisko klasifikāciju dokumentiem un e-pasta ziņojumiem, kas iepriekš bija manuāli atzīmēti ar etiķeti vai iepriekš automātiski atzīmēti ar augstākas klasifikācijas etiķeti.  Papildinformāciju skatiet rakstā [Kā tiek lietotas automātiskās vai ieteicamās etiķetes](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. Ja problēmas joprojām pastāv, lūdzu, apkopojiet pakalpojuma Azure informācijas aizsardzība klienta žurnālus un pievienojiet šos eksportētos žurnālus savai atbalsta biļetei. Lai eksportētu pakalpojuma Azure informācijas aizsardzība žurnālus:
    - Atveriet Office dokumentu vai izveidojiet jaunu e-pasta ziņojumu programmā Outlook.
    - Noklikšķiniet uz **Aizsargāt/sensitivitāte** > **Palīdzība un atsauksmes**.
    - Noklikšķiniet uz **Eksportēt žurnālus**.
    - Saglabājiet žurnālus paša izvēlētā atrašanās vietā un pievienojiet tos savam pakalpojuma pieprasījumam.

Lai iegūtu papildinformāciju, skatiet:

- [Kā konfigurēt pakalpojuma Azure informācijas aizsardzība automātiskās un ieteicamās klasifikācijas nosacījumus](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Detalizēti norādījumi vispārējiem scenārijiem, kuros tiek izmantots pakalpojums Azure informācijas aizsardzība](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Pakalpojuma Azure informācijas aizsardzība dokumentācijas pārskatīšana](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Pakalpojuma Azure informācijas aizsardzība abonementu un līdzekļu pārskatīšana](https://azure.microsoft.com/pricing/details/information-protection)
- [Pakalpojuma Azure informācijas aizsardzība prasības](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Pakalpojuma Azure informācijas aizsardzība ātrās sākšanas apmācība](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Pakalpojuma Azure informācijas aizsardzība klienta lejupielāde](https://www.microsoft.com/download/details.aspx?id=53018)
