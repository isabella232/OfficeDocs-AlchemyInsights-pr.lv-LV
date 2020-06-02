---
title: 'AIP: politikas nav uzvedas kā gaidīts'
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
- "4780"
ms.openlocfilehash: 527556fcb02525eb88ea992c38a2ddfcba6f9453
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506565"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: politikas nav uzvedas kā gaidīts

Azure informācijas aizsardzība: politikas nav uzvedas kā paredzēts, skatiet šo ieteicamās vadlīnijas dažādiem politikas jautājumiem:

1. Ja jums ir problēmas ar vizuālām atzīmēm, lūdzu, pārskatiet, [kad tiek lietoti vizuālie marķējumi](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Ja rodas problēmas ar automātisku marķēšanu, lūdzu, pārskatiet, [kā konfigurēt nosacījumus automātiskai un ieteicamajai klasifikācijai Azure informācijas aizsardzībai](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) un [kāda veida sensitīvo informācijas tipu meklē](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. Ja rodas problēmas ar vietējo/Pfile aizsardzību, lūdzu, pārskatiet [failu API konfigurāciju](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Pārbaudiet, ja izmantojat ietverti politikas, kas nav konfigurēti pareizi: [kā konfigurēt Azure informācijas aizsardzības politika noteiktiem lietotājiem, izmantojot ietverti politikas](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Ja automātiskā marķēšana nedarbojas Outlook, pievienojot dokumentu ar apzīmējumu, pārbaudiet, vai DRMEncryptProperty nav definēts kā aprakstīts šeit: [IRM reģistra iestatījumus drošībai](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Ja jums joprojām ir radušās problēmas, lūdzu, apkopojiet Azure informācijas aizsardzības klienta žurnālus un pievienojiet eksportētos žurnālus šai biļetei.

1. Atveriet Office dokumentu vai izveidojiet jaunu e-pastu programmā Outlook.
2. Noklikšķiniet uz **aizsargāt/jutīguma**  >  **Palīdzība un atsauksmes**.
3. Noklikšķiniet uz **Eksportēt žurnālus**.
4. Saglabājiet žurnālus savā izvēlētā atrašanās vietā un pievienojiet tos šim pakalpojuma pieprasījumam.

Papildu resursi:

- [Kā konfigurēt Visual marķējums etiķete Azure informācijas aizsardzība](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Azure informācijas aizsardzības dokumentācijas pārskatīšana](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Jutības iezīmju izmantošana Office lietojumprogrammās](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

