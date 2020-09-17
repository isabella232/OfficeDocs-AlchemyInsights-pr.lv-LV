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
ms.openlocfilehash: 2e711679e7db7293d9e7e6f68d0662f03047c23d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799211"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>E-pasta ziņojuma atsaukšana vai aizstāšana programmā Microsoft 365

- Varat **tikai atsaukt ziņojumus, kas tiek nosūtīti lietotājiem jūsu organizācijā**. Ja ziņojums tika nosūtīts uz Gmail adresi, piemēram, varat to atsaukt.
- Varat **atsaukt no programmas Outlook 2016 sūtītos ZIŅOJUMUS datorā**. Ja lietotājs nosūta ziņojumu, izmantojot programmu Outlook darbam ar Mac vai Outlook tīmeklī, to nevar atsaukt.
- Ja esat administrators, varat **Atsaukt ziņojumus lietotāju vārdā, izmantojot PowerShell**. Jūs nevarat atsaukt ziņojumus no administrēšanas centra. Lai iegūtu papildinformāciju, ritiniet uz leju līdz opcijai meklēt un izdzēst e-pasta ziņojumus jūsu organizācijā.

**Nosūtīta e-pasta ziņojuma atsaukšana vai aizstāšana**

1. Mapju rūtī, kas atrodas pa kreisi no Outlook loga, izvēlieties mapi Nosūtītie vienumi.
2. Atveriet ziņojumu, kuru vēlaties atsaukt. Lai atvērtu ziņojumu, veiciet uz tā dubultklikšķi. Atlasiet ziņojumu, lai tas tiktu parādīts lasīšanas rūtī, Neļaujiet atsaukt ziņojumu.
3. Cilnē ziņojums atlasiet **darbības**  >  **Šī ziņojuma atsaukšana**.
4. Izvēlieties **Dzēst šī ziņojuma nelasītās kopijas** vai **Dzēst nelasītās kopijas un aizstāt ar jaunu ziņojumu un**pēc tam atlasiet **Labi**.
5. Ja sūtāt aizstāšanas ziņojumu, izveidojiet ziņojumu un pēc tam atlasiet **Sūtīt**.
6. Ziņojuma atsaukšanas sekmīgs vai neizdošanās ir atkarīgs no adresātu iestatījumiem programmā Outlook.

Papildinformāciju par atsaukšanu skatiet rakstā [e-pasta ziņojuma atsaukšana vai aizstāšana](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***E-pasta ziņojumu meklēšana un dzēšana savā organizācijā*** Lai meklētu un izdzēstu e-pasta ziņojumus savā organizācijā, ir vienkāršāk, ja esat globālais administrators. Ja neesat globālais administrators, jūsu konts ir jāpievieno e-datu atklāšanas pārvaldnieka lomu grupai vai atbilstības meklēšanas pārvaldības lomai. Lai izdzēstu ziņojumus, ir jāpievienojas organizācijas pārvaldības lomu grupai vai meklēšanas un iztīrīšanas pārvaldības lomai. Atļaujas šīm lomām tiek piešķirtas [drošības & atbilstības centrā](https://protection.office.com/).

1. [Izveidojiet satura meklēšanu](https://docs.microsoft.com/microsoft-365/compliance/content-search) , lai atrastu dzēšamo ziņojumu.
2. [Savienojuma izveide ar drošības & atbilstības centra PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps). 

Ja izmantojat MFA, skatiet rakstu [savienojuma izveide ar Microsoft 365 security & atbilstības centra PowerShell, izmantojot daudzfaktoru autentifikāciju](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 
