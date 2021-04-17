---
title: 'AIP: politikas nedarbojas, kā paredzēts'
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
- "4780"
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821634"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: politikas nedarbojas, kā paredzēts

Azure informācijas aizsardzība: politikas nedarbojas, kā paredzēts, skatiet tālāk sniegtās vadlīnijas dažādām politikas problēmām.

1. Ja rodas problēmas ar vizuāliem atzīmēm, lūdzu, [pārskatiet, kad tiek lietoti vizuālie apzīmējumi.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)
2. Ja rodas problēmas ar automātisko etiķetēšanu, lūdzu, pārskatiet kā konfigurēt automātiskās un ieteicamās [Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) informācijas aizsardzības klasifikācijas nosacījumus un Ko meklē [sensitīvās informācijas tipi](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. Ja rodas problēmas ar vietējo/Pfile aizsardzību, lūdzu, pārskatiet [failu API konfigurāciju.](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)
4. Pārbaudiet, vai izmantojat nepareizi konfigurētas tvēruma politikas: Kā konfigurēt Azure informācijas aizsardzības politiku konkrētiem lietotājiem, [izmantojot tvēruma politikas.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)
5. Ja automātiskā marķēšana nedarbojas programmā Outlook, pievienojot marķētu dokumentu, pārliecinieties, vai DRMEncryptProperty nav definēts šeit: [IRM](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)reģistra iestatījumi drošībai .

Ja joprojām pastāv problēmas, lūdzu, apkopojiet Azure informācijas aizsardzības klienta žurnālus un pievienojiet eksportētos žurnālus šai biļetei.

1. Atveriet Office dokumentu vai izveidojiet jaunu e-pasta ziņojumu programmā Outlook.
2. Noklikšķiniet **uz Aizsargāt/jūtīgumu**  >  **palīdzība un atsauksmes.**
3. Noklikšķiniet **uz Eksportēt žurnālus.**
4. Saglabājiet žurnālus savā atrašanās vietā un pievienojiet tos šim pakalpojuma pieprasījumam.

Papildu resursi:

- [Kā konfigurēt etiķeti vizuāliem apzīmējumiem Azure informācijas aizsardzībai](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Azure informācijas aizsardzības dokumentācijas pārskatīšana](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Sensitivitātes etiķešu izmantošana Microsoft 365 programmās](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

