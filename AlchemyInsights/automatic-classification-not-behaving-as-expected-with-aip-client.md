---
title: Automātiska klasifikācija nav uzvedas kā gaidīts ar AIP Client
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4373"
ms.openlocfilehash: 95a994d6a49ee8737a6ebcb196314f92776d8482
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/26/2020
ms.locfileid: "44493176"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Automātiska klasifikācija nav uzvedas kā gaidīts ar AIP Client

Automātiskā klasifikācija nav uzvedas kā paredzēts, izmantojiet šādas ieteicamās vadlīnijas:

1. Ja rodas problēmas ar automātisko marķēšanu, skatiet sadaļu [kā konfigurēt nosacījumus automātiskai un ieteicamajai klasifikācijai Azure informācijas aizsardzībai](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) un [kāda veida sensitīvo informācijas tipu meklē](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).
2. Pārbaudiet, ja izmantojat ietverti politikas, kas nav konfigurēti pareizi: [kā konfigurēt Azure informācijas aizsardzības politika noteiktiem lietotājiem, izmantojot ietverti politikas](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Ja automātiskā marķēšana nedarbojas Outlook, pievienojot dokumentu ar etiķeti, pārbaudiet, vai tas `DRMEncryptProperty` nav definēts kā aprakstīts šeit: [IRM reģistra iestatījumus drošībai](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Ja Azure informācijas aizsardzības politikai izmantojāt [iebūvētos informācijas tipus](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) , pārbaudiet, vai saturs atbilst paredzamam formātam.
5. Pārbaudiet, vai etiķete ir atbilstoši konfigurēta **automātiskai** vai **ieteicamajai**lietošanai. (**Automātiskā** marķēšana ir pieejama visām Office programmām, bet **ieteicams** ir pieejama visām Office lietojumprogrammām, izņemot Outlook.)
6. Dokumentu un e-pasta ziņojumiem, kas iepriekš bija manuāli apzīmēti vai iepriekš automātiski apzīmēti ar augstāku klasifikāciju, nevar izmantot automātisko klasifikāciju.  Papildinformāciju skatiet: [kā tiek lietotas automātiskās vai ieteicamās etiķetes](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. Ja joprojām rodas problēmas, lūdzu, apkopojiet Azure informācijas aizsardzības klienta žurnālus un pievienojiet eksportētos žurnālus atbalsta biļetei. Lai eksportētu Azure informācijas aizsardzības žurnālus:
    - Atveriet Office dokumentu vai izveidojiet jaunu e-pastu programmā Outlook.
    - Noklikšķiniet uz **aizsargāt/jutīguma**  >  **Palīdzība un atsauksmes**.
    - Noklikšķiniet uz **Eksportēt žurnālus**.
    - Saglabājiet žurnālus savā izvēlētā atrašanās vietā un pievienojiet tos pakalpojuma pieprasījumam.

Lai iegūtu papildu informāciju, skatiet:

- [Kā konfigurēt Azure informācijas aizsardzības automātiskās un ieteicamo klasifikācijas nosacījumi](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Norādījumi par vispārējiem scenārijiem, kas izmanto Azure informācijas aizsardzību](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Azure informācijas aizsardzības dokumentācijas pārskatīšana](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Pārskatiet Azure informācijas aizsardzības abonementus un līdzekļus](https://azure.microsoft.com/pricing/details/information-protection)
- [Prasības Azure informācijas aizsardzība](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Ātri sākt apmācība Azure informācijas aizsardzība](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Lejupielādēt Azure informācijas aizsardzības klients](https://www.microsoft.com/download/details.aspx?id=53018)
