---
title: E-pasta ziņojuma atsaukšana vai aizstāšana
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 45882b49c5c47b3e0e4519e2339e6c68110bc75aebeaeac2d0ccd009bdfa3f7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54024393"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>E-pasta ziņojuma atsaukšana vai aizstāšana programmā Microsoft 365

- Varat atsaukt **tikai tos ziņojumus, kas ir nosūtīti personām jūsu organizācijā.** Piemēram, ja ziņojums tika nosūtīts uz Gmail adresi, to nevar atsaukt.
- Varat atsaukt **tikai ziņojumus, kas nosūtīti Outlook no datora.** Ja lietotājs nosūta ziņojumu, izmantojot Outlook operētājsistēmai Mac vai Outlook tīmeklī, neatceraties to.
- Kā īrnieka administrators varat atsaukt ziņojumus lietotāju vārdā, izmantojot **PowerShell** (Papildinformāciju skatiet rakstā E-pasta ziņojumu meklēšana [un dzēšana).](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)
- Nevar atsaukt ziņojumus no administrēšanas centra. Ritiniet uz leju līdz "Meklēt un dzēst e-pasta ziņojumus jūsu organizācijā", lai iegūtu papildinformāciju.

**Nosūtīta e-pasta ziņojuma atsaukšana vai aizstāšana**

1. Mapju rūtī pa kreisi no Outlook izvēlieties mapi Nosūtītie vienumi.
2. Atveriet ziņojumu, kuru vēlaties atsaukt. Lai atvērtu ziņojumu, ir jāveic dubultklikšķis. Atlasot ziņojumu, lai tas būtu redzams lasīšanas rūtī, nevarēsit atsaukt ziņojumu.
3. Cilnē Ziņojums atlasiet Darbības **Atsaukt**  >  **šo ziņojumu**.
4. Izvēlieties **Dzēst nelasītās šī ziņojuma kopijas** vai **Dzēst nelasītās kopijas** un aizstājiet ar jaunu ziņojumu un pēc tam atlasiet **Labi**.
5. Ja sūtāt nomaiņas ziņojumu, izveidojiet ziņojumu un pēc tam atlasiet **Sūtīt**.
6. Ziņojuma atsaukšanas izdošanās vai kļūme ir atkarīga no adresāta iestatījumiem Outlook.

Papildinformāciju, tostarp par to, kā pārbaudīt atsaukums, skatiet rakstā [Nosūtītā e-pasta](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)ziņojuma atsaukšana vai aizstāšana.

***Lai meklētu un izdzēstu e-pasta ziņojumus*** savā organizācijā, visvienkāršāk varat atrast, ja esat globālais administrators. Ja neesat globālais administrators, jūsu konts ir jāpievieno e-datu atklāšanas pārvaldnieka lomu grupai vai atbilstības meklēšanas pārvaldības lomai. Lai izdzēstu ziņojumus, ir jāpievienoas organizācijas pārvaldības lomu grupai vai meklēšanas un iztīres pārvaldības lomai. Šīs lomas atļaujas tiek piešķirtas drošības [kontroles & centrā.](https://protection.office.com/)

1. [Izveidojiet satura meklēšanu,](https://docs.microsoft.com/microsoft-365/compliance/content-search) lai atrastu ziņojumu, ko izdzēst.
2. [Savienošana uz Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).

Ja izmantojat MFA (daudzfaktors autentifikāciju), skatiet sadaļu [Savienošana Microsoft 365 atbilstības & centra PowerShell, izmantojot daudzfaktors autentifikāciju.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
