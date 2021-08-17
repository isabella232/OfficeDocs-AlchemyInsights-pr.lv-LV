---
title: MC210173 — SharePoint Designer jaunā pielāgoto veidlapu līdzekļa novecošana
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
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: f72d6ce6931b39d5d4a4835cee0ed2952407b13187213cca5bd483acb1e192bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54077671"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a>MC210173 — SharePoint Designer jaunā pielāgoto veidlapu līdzekļa novecošana

Mēs atklājām problēmu, kas ietekmē SharePoint Designer [pielāgoto veidlapu izveides](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) funkcionalitāti pakalpojumā SharePoint Online. Pēc rūpīgas pārbaudes, mēs nonācām pie secinājuma, ka šai problēmai nav zināma labojuma, un tāpēc mēs nolēmām atspējot pielāgoto veidlapu izveides līdzekli sākot ar 2020. gada 25. aprīli plkst. 03.00 UTC laika joslā. Šīs izmaiņas neietekmēs iespēju rediģēt iepriekš izveidotās veidlapas vai citus SharePoint Online noformētāja esošos līdzekļus.

Pēc šo izmaiņu veikšanas, lietotājiem jaunu veidlapu izveides laikā var tikt parādīts kļūdas paziņojums: “Neizdevās saglabāt saraksta izmaiņas serverī”.

Lietotāji, kas iepriekš izmantoja SharePoint Designer, lai veidotu pielāgotas veidlapas, tagad šim mērķim var izmantot [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form).

PowerApps ir vienkāršs, bet spēcīgs rīks, kas ļauj lietotājiem izmantot SharePoint Online Modern, lai pārlūkprogrammas logā veidotu vai rediģētu pielāgotās veidlapas SharePoint sarakstiem un dokumentu bibliotēkām. PowerApps nav nepieciešamas papildu kodēšanas zināšanas vai papildu lietojumprogrammu lejupielāde, piemēram, InfoPath.

**Piezīme**: SharePoint Online Classic versijas lietotājiem būs īslaicīgi jāpāriet uz Modern versiju, lai piekļūtu un izmantotu PowerApps. Visas PowerApps izveidotās pielāgotās veidlapas ir pieejamas arī SharePoint Online Classic versijas lietotājiem.
