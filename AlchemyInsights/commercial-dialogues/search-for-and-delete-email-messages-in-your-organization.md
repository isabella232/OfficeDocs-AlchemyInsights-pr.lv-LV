---
title: E-pasta ziņojumu meklēšana un dzēšana organizācijā
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: bd25d9bb2af8114786503e129de105c9a0f602c98b206f01770605d1957e3a1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53948890"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>E-pasta ziņojumu meklēšana un dzēšana organizācijā

Izpildiet tālāk norādītās darbības.

1. Ja neesat globālais administrators, lai meklētu ziņojumus, jūsu konts ir jāpievieno **e-datu atklāšanas** pārvaldnieka lomu grupai vai atbilstības meklēšanas **pārvaldības lomai.** Lai izdzēstu ziņojumus, ir jāpievienoas organizācijas pārvaldības **lomu grupai** vai **meklēšanas un iztīres pārvaldības lomai**. Šīs lomas atļaujas tiek piešķirtas drošības [& centrā.](https://protection.office.com)
2. [Izveidojiet satura meklēšanu,](https://docs.microsoft.com/office365/securitycompliance/content-search) lai atrastu ziņojumu, ko izdzēst.
3. [Savienošana uz Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell). Ja izmantojat MFA, skatiet šos norādījumus: Savienošana uz drošības & [centra PowerShell, izmantojot daudzpakāpju autentifikāciju](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Izdzēsiet ziņojumu: izpildiet `New-ComplianceSearchAction` cmdlet, lai izdzēstu ziņojumu. Izdzēstie ziņojumi tiek pārvietoti uz lietotāja mapi Atkopjamie vienumi. Komandas piemēru skatiet [3. darbībā. Izdzēsiet ziņojumu.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
