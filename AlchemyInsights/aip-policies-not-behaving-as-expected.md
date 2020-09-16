---
title: 'AIP: politikas nedarbojas, kā paredzēts'
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
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663196"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: politikas nedarbojas, kā paredzēts

Azure informācijas aizsardzība: politikas nedarbojas, kā paredzēts, skatiet tālāk norādītās ieteikumi par dažādām politikas problēmām:

1. Ja rodas problēmas ar vizuāliem marķējumiem, lūdzu, pārskatiet, [kad tiek lietots vizuālais marķējums](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Ja jums rodas problēmas ar automātisko etiķetēšanu, lūdzu, pārskatiet, [kā konfigurēt nosacījumus automātiskajai un ieteicamajai klasifikācijai Azure informācijas aizsardzībai](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) un [kā izskatās sensitīvie informācijas tipi](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. Ja rodas problēmas ar vietējo/Pfile aizsardzību, lūdzu, pārskatiet [failu API konfigurāciju](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Pārbaudiet, vai izmantojat aptvertās politikas, kas nav pareizi konfigurētas: [kā konfigurēt Azure informācijas aizsardzības politiku konkrētiem lietotājiem, izmantojot aptvertās politikas](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Ja, pievienojot ar etiķeti dokumentu, automātiskā etiķešu izveide nedarbojas programmā Outlook, pārbaudiet, vai DRMEncryptProperty nav definēts, kā aprakstīts šeit: [IRM reģistra iestatījumi drošībai](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Ja joprojām rodas problēmas, lūdzu, apkopojiet Azure Information Protection klienta žurnālus un pievienojiet eksportētos žurnālus šajā biļetē.

1. Atveriet Office dokumentu vai izveidojiet jaunu e-pasta ziņojumu programmā Outlook.
2. Noklikšķiniet uz **aizsargāt/jutīg**  >  **palīdzību un atsauksmes**.
3. Noklikšķiniet uz **Eksportēt žurnālus**.
4. Saglabājiet žurnālus savā atrašanās vietā un pievienojiet tos šim pakalpojuma pieprasījumam.

Papildu resursi:

- [Kā konfigurēt etiķetes vizuālo datu aizsardzībai vizuālajiem marķējumiem](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Azure informācijas aizsardzības dokumentācijas pārskatīšana](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Jutības uzlīmju lietošana Microsoft 365 lietojumprogrammās](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

