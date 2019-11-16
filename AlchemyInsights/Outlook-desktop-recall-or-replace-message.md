---
title: Outlook darbvirsmas atsaukšana vai aizstājiet e-pasta ziņojumu
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d3a6c253317137b7069a978b907c97d61bf7313
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 11/15/2019
ms.locfileid: "36496118"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Outlook e-pasta ziņojuma atsaukšana vai aizstāšana

- Kā admin, jūs varat **Atsaukt ziņojumus vārdā lietotājiem, izmantojot PowerShell**. Ziņojumus nevar atsaukt administrēšanas centrā.
- Varat **atsaukt tikai tos ziņojumus, kas nosūtīti personām jūsu organizācijā**. Piemēram, ja ziņojums ir nosūtīts uz Gmail adresi, to nevar atsaukt.
- **No datora var tikai atsaukt ziņojumus, kas nosūtīti no programmas Outlook 2016**. Ja lietotājs nosūta ziņojumu, izmantojot Outlook Mac vai Outlook Web, to nevar atsaukt.

Lai atsauktu vai aizstātu e-pasta ziņojumu:

1. Mapju rūtī, kas atrodas Outlook loga kreisajā pusē, atlasiet mapi Nosūtītie vienumi.
1. Veiciet dubultklikšķi uz ziņojuma, kuru vēlaties atsaukt, lai to atvērtu.
1. Atlasiet cilni **ziņojums** un pēc tam atlasiet **darbības** > **Atsaukt šo ziņojumu**.
1. Atlasiet **Dzēst šī ziņojuma nelasītās kopijas** vai **Dzēst nelasītās kopijas un aizstāt ar jaunu ziņojumu**un pēc tam atlasiet **Labi**.
1. Ja sūtāt ziņojumu ar aizstājējziņu, Sastādiet ziņojumu un pēc tam atlasiet **Sūtīt**.
1. Ziņojumu atsaukšanas izdošanās vai neveiksme ir atkarīga no adresāta iestatījumiem programmā Outlook. Lai pārbaudītu atsaukuma darbības, skatiet [šo rakstu](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

E-pasta ziņojumu meklēšana un dzēšana organizācijā

- Ja neesat globālais administrators, jūsu konts ir jāpievieno lomai eDiscovery Manager loma vai atbilstības meklēšanas pārvaldība, lai meklētu ziņojumus. Lai dzēstu ziņojumus, ir jāpievienojas organizācijas pārvaldības lomu grupai vai lomai meklēšanas un tīrīšanas pārvaldība. Šo lomu atļaujas tiek piešķirtas [drošības un atbilstības centrā](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Izveidojiet satura meklēšanu](https://docs.microsoft.com/office365/securitycompliance/content-search) , lai atrastu dzēšamo ziņojumu.
- [Izveidot savienojumu ar drošības un atbilstības centra PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Ja izmantojat vairāku faktoru autentifikāciju, skatiet [izveidot savienojumu ar Office 365 drošības un atbilstības centrs PowerShell, izmantojot vairāku faktoru autentifikācija](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).