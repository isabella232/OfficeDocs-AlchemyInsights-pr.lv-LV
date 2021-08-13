---
title: Outlook Darbvirsmas atsaukšana vai e-pasta ziņojuma aizstāšana
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 33fe7ebd53d7ff11dbab54ce589aaf58e68c633be4d83a3cdfb00edc7752430e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918402"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>E-pasta Outlook atsaukšana vai aizstāšana

- Kā administrators varat atsaukt **ziņojumus lietotāju vārdā, izmantojot PowerShell**. Nevar atsaukt ziņojumus no administrēšanas centra.
- Varat atsaukt **tikai tos ziņojumus, kas ir nosūtīti personām jūsu organizācijā.** Ja ziņojums tika nosūtīts, piemēram, uz Gmail adresi, to nevar atsaukt.
- Pc datorā **varat atsaukt tikai no Outlook 2016 sūtītus ziņojumus.** Ja lietotājs nosūta ziņojumu, izmantojot Outlook operētājsistēmai Mac vai Outlook tīmeklī, neatceraties to.

Lai atsauktu vai aizstātu e-pasta ziņojumu:

1. Mapju rūtī pa kreisi no jaunā Outlook atlasiet mapi Nosūtītie vienumi.
1. Lai atvērtu ziņojumu, kuru vēlaties atsaukt, veiciet dubultklikšķi uz tā.
1. Atlasiet cilni **Ziņojums** un pēc tam atlasiet Darbības   >  **Atsaukt šo ziņojumu.**
1. Atlasiet **Dzēst nelasītās šī ziņojuma kopijas** vai **Dzēst nelasītās kopijas** un aizstājiet ar jaunu ziņojumu un pēc tam atlasiet **Labi**.
1. Ja sūtāt nomaiņas ziņojumu, izveidojiet ziņojumu un pēc tam atlasiet **Nosūtīt**.
1. Ziņojuma atsaukšanas izdošanās vai kļūme ir atkarīga no adresāta iestatījumiem Outlook. Lai uzzinātu, kā pārbaudīt atsaukšanas darbību, skatiet [šo rakstu.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)

E-pasta ziņojumu meklēšana un dzēšana organizācijā

- Ja neesat globālais administrators, jūsu konts ir jāpievieno e-datu atklāšanas pārvaldnieka lomai vai atbilstības meklēšanas pārvaldības lomai, lai meklētu ziņojumus. Lai izdzēstu ziņojumus, ir jāpievienoas organizācijas pārvaldības lomu grupai vai meklēšanas un iztīres pārvaldības lomai. Šo lomu atļaujas tiek piešķirtas drošības [un atbilstības centrā.](https://go.microsoft.com/fwlink/?linkid=2083731)
- [Izveidojiet satura meklēšanu,](https://docs.microsoft.com/microsoft-365/compliance/content-search) lai atrastu ziņojumu, ko izdzēst.
- [Savienošana uz drošības un atbilstības centra PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Ja izmantojat daudzfaktors autentifikāciju, skatiet rakstu Savienošana Microsoft 365 un atbilstības centra [PowerShell izmantošana, izmantojot daudzpakāpju autentifikāciju.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)