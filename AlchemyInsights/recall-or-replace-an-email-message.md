---
title: E-pasta ziņojuma atsaukšana vai aizstāšana
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: e541620a499b02a7206579ffcc505ceb4e632a4c
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742762"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Atsaukt vai aizstāt e-pasta ziņojumu Microsoft 365

- Varat **atsaukt tikai tos ziņojumus, kas nosūtīti personām jūsu organizācijā**. Piemēram, ja ziņojums ir nosūtīts uz Gmail adresi, to nevar atsaukt.
- **No datora var tikai atsaukt ziņojumus, kas nosūtīti no programmas Outlook 2016**. Ja lietotājs nosūta ziņojumu, izmantojot Outlook Mac vai Outlook Web, to nevar atsaukt.
- Ja esat administrators, varat **atsaukt ziņojumu lietotāju vārdā, izmantojot PowerShell**. Ziņojumus nevar atsaukt administrēšanas centrā. Lai iegūtu papildinformāciju, ritiniet lejup līdz "meklēt un dzēst e-pasta ziņojumus jūsu organizācijā".

**Nosūtīta e-pasta ziņojuma atsaukšana vai aizstāšana**

1. Mapju rūtī, kas atrodas Outlook loga kreisajā pusē, izvēlieties mapi Nosūtītie vienumi.
2. Atveriet ziņojumu, kuru vēlaties atsaukt. Lai atvērtu ziņojumu, ir jāveic dubultklikšķis. Ziņojuma atlasīšana tā, lai tas parādītos lasīšanas rūtī, neļaus atsaukt ziņojumu.
3. Cilnē ziņojums atlasiet **darbības** > **Atsaukt šo ziņojumu**.
4. Izvēlieties **Dzēst šī ziņojuma nelasītās kopijas** vai **Dzēst nelasītās kopijas un aizstāt ar jaunu ziņojumu un**pēc tam atlasiet **Labi**.
5. Ja sūtāt ziņojumu ar aizstājējziņu, Sastādiet ziņojumu un pēc tam atlasiet **Sūtīt**.
6. Ziņojuma atsaukšanas veiksme vai kļūme ir atkarīga no adresātu iestatījumiem programmā Outlook.

Papildinformāciju, tostarp informāciju par to, kā pārbaudīt atsaukto, skatiet sadaļā [jūsu nosūtītās e-pasta ziņojuma atsaukšana vai aizstāšana](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***E-pasta ziņojumu meklēšana un dzēšana organizācijā*** Lai meklētu un izdzēstu e-pasta ziņojumus jūsu organizācijā, visvienkāršāk ir, ja esat globāls administrators. Ja neesat globālais administrators, jūsu konts ir jāpievieno lomu grupai eDiscovery Manager vai atbilstības meklēšanas pārvaldības lomai. Lai dzēstu ziņojumus, ir jāpievienojas organizācijas pārvaldības lomu grupai vai lomai meklēšanas un tīrīšanas pārvaldība. Šo lomu atļaujas tiek piešķirtas [drošības & atbilstības centrā](https://protection.office.com/).

1. [Izveidojiet satura meklēšanu](https://docs.microsoft.com/office365/securitycompliance/content-search) , lai atrastu dzēšamo ziņojumu.
2. [Izveidot savienojumu ar drošības & atbilstības centra PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps). 

Ja izmantojat MFA, skatiet [izveidot savienojumu ar Microsoft 365 drošības & atbilstības centrs PowerShell, izmantojot vairāku faktoru autentifikācija](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 
