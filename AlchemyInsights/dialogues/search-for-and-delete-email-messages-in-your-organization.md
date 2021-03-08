---
title: E-pasta ziņojumu meklēšana un dzēšana savā organizācijā
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
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525434"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>E-pasta ziņojumu meklēšana un dzēšana savā organizācijā

Izpildiet tālāk norādītās darbības.

1. Ja neesat globālais administrators, varat meklēt ziņojumus, kas jūsu kontam ir jāpievieno **e-datu atklāšanas pārvaldnieka lomu grupai** vai **atbilstības meklēšanas pārvaldības lomai**. Lai izdzēstu ziņojumus, ir jāpievienojas **organizācijas pārvaldības lomu grupai** vai **meklēšanas un iztīrīšanas pārvaldības lomai**. Atļaujas šīm lomām tiek piešķirtas [drošības & atbilstības centrā.](https://protection.office.com)
2. [Izveidojiet satura meklēšanu](https://docs.microsoft.com/office365/securitycompliance/content-search) , lai atrastu dzēšamo ziņojumu.
3. [Savienojuma izveide ar drošības & atbilstības centra PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell). Ja izmantojat MFA, skatiet šos norādījumus: savienojuma izveide [ar drošības & atbilstības centra PowerShell, izmantojot daudzfaktoru autentifikāciju](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Dzēst ziņojumu: palaidiet `New-ComplianceSearchAction` cmdlet, lai izdzēstu ziņojumu. Izdzēstie ziņojumi tiek pārvietoti uz lietotāja atkopto vienumu mapi. Lai iegūtu komandu piemērs, skatiet sadaļu [3. darbība: ziņojuma dzēšana.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
