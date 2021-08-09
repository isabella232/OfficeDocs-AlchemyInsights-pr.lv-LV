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
ms.openlocfilehash: 90448bf57297ce59ba222efd1927b5de588bfbfdb1206b6403764d7f43fed690
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934300"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: politikas nedarbojas, kā paredzēts

Azure informācijas aizsardzība: politikas nedarbojas, kā paredzēts, skatiet tālāk sniegtās vadlīnijas dažādām politikas problēmām.

1. Ja rodas problēmas ar vizuāliem atzīmēm, lūdzu, [pārskatiet, kad tiek lietoti vizuālie apzīmējumi.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)
2. Ja rodas problēmas ar automātisko etiķetēšanu, lūdzu, pārskatiet kā konfigurēt automātiskās un ieteicamās [Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) informācijas aizsardzības klasifikācijas nosacījumus un Ko meklē [sensitīvās informācijas tipi](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. Ja rodas problēmas ar vietējo/Pfile aizsardzību, lūdzu, pārskatiet [failu API konfigurāciju.](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)
4. Pārbaudiet, vai neizmantojat tvēruma politikas, kas nav pareizi konfigurētas: [Kā konfigurēt pakalpojuma Azure informācijas aizsardzība politiku konkrētiem lietotājiem, izmantojot tvēruma politikas](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Ja automātiskā marķēšana nedarbojas programmā Outlook, kad pievienojat marķētu dokumentu, pārliecinieties, vai DRMEncryptProperty nav definēts šeit: [IRM](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)reģistra iestatījumi drošībai .

Ja joprojām pastāv problēmas, lūdzu, apkopojiet Azure informācijas aizsardzības klienta žurnālus un pievienojiet eksportētos žurnālus šai biļetei.

1. Atveriet Office dokumentu vai izveidojiet jaunu e-pasta ziņojumu programmā Outlook.
2. Noklikšķiniet uz **Aizsargāt/sensitivitāte** > **Palīdzība un atsauksmes**.
3. Noklikšķiniet uz **Eksportēt žurnālus**.
4. Saglabājiet žurnālus savā atrašanās vietā un pievienojiet tos šim pakalpojuma pieprasījumam.

Papildu resursi:

- [Kā konfigurēt etiķeti vizuāliem apzīmējumiem Azure informācijas aizsardzībai](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Pakalpojuma Azure informācijas aizsardzība dokumentācijas pārskatīšana](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Sensitivitātes etiķešu izmantošana Microsoft 365 programmās](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

