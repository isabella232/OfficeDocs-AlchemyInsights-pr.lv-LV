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
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353513"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>E-pasta ziņojuma atsaukšana vai aizstāšana programmā Microsoft 365

- Varat **tikai atsaukt ziņojumus, kas tiek nosūtīti lietotājiem jūsu organizācijā**. Piemēram, ja ziņojums tika nosūtīts uz Gmail adresi, to nevar atsaukt.
- **No datora Outlook sūtītos ziņojumus varat atsaukt**. Ja lietotājs nosūta ziņojumu, izmantojot programmu Outlook darbam ar Mac vai Outlook tīmeklī, to nevar atsaukt.
- Kā nomnieka administrators varat **Atsaukt ziņojumus lietotāju vārdā, izmantojot PowerShell** (Papildinformācija atrodama rakstā [e-pasta ziņojumu meklēšana un dzēšana](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).
- Jūs nevarat atsaukt ziņojumus no administrēšanas centra. Lai iegūtu papildinformāciju, ritiniet uz leju līdz opcijai meklēt un izdzēst e-pasta ziņojumus jūsu organizācijā.

**Nosūtīta e-pasta ziņojuma atsaukšana vai aizstāšana**

1. Mapju rūtī, kas atrodas pa kreisi no Outlook loga, izvēlieties mapi Nosūtītie vienumi.
2. Atveriet ziņojumu, kuru vēlaties atsaukt. Lai atvērtu ziņojumu, veiciet uz tā dubultklikšķi. Atlasiet ziņojumu, lai tas tiktu parādīts lasīšanas rūtī, Neļaujiet atsaukt ziņojumu.
3. Cilnē ziņojums atlasiet **darbības**  >  **Šī ziņojuma atsaukšana**.
4. Izvēlieties **Dzēst šī ziņojuma nelasītās kopijas** vai **Dzēst nelasītās kopijas un aizstāt ar jaunu ziņojumu un** pēc tam atlasiet **Labi**.
5. Ja sūtāt aizstāšanas ziņojumu, izveidojiet ziņojumu un pēc tam atlasiet **Sūtīt**.
6. Ziņojuma atsaukšanas sekmīgs vai neizdošanās ir atkarīgs no adresātu iestatījumiem programmā Outlook.

Papildinformāciju par atsaukšanu skatiet rakstā [e-pasta ziņojuma atsaukšana vai aizstāšana](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

**_Lai meklētu un izdzēstu e-pasta ziņojumus savā organizācijā_**, ir vienkāršāk, ja esat globālais administrators. Ja neesat globālais administrators, jūsu konts ir jāpievieno e-datu atklāšanas pārvaldnieka lomu grupai vai atbilstības meklēšanas pārvaldības lomai. Lai izdzēstu ziņojumus, ir jāpievienojas organizācijas pārvaldības lomu grupai vai meklēšanas un iztīrīšanas pārvaldības lomai. Atļaujas šīm lomām tiek piešķirtas [drošības & atbilstības centrā](https://protection.office.com/).

1. [Izveidojiet satura meklēšanu](https://docs.microsoft.com/microsoft-365/compliance/content-search) , lai atrastu dzēšamo ziņojumu.
2. [Savienojuma izveide ar drošības & atbilstības centra PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).

Ja izmantojat MFA (daudzfaktoru autentifikācija), skatiet rakstu [savienojuma izveide ar Microsoft 365 Security & atbilstības centra PowerShell, izmantojot daudzfaktoru autentifikāciju](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).
