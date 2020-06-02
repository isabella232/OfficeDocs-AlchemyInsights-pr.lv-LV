---
title: Outlook darbvirsmas atsaukšana vai aizstājiet e-pasta ziņojumu
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: bb84363ae7d3c91750d5de789c091c7cebbbedc2
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502326"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Outlook e-pasta ziņojuma atsaukšana vai aizstāšana

- Kā admin, jūs varat **Atsaukt ziņojumus vārdā lietotājiem, izmantojot PowerShell**. Ziņojumus nevar atsaukt administrēšanas centrā.
- Varat **atsaukt tikai tos ziņojumus, kas nosūtīti personām jūsu organizācijā**. Piemēram, ja ziņojums ir nosūtīts uz Gmail adresi, to nevar atsaukt.
- **No datora var tikai atsaukt ziņojumus, kas nosūtīti no programmas Outlook 2016**. Ja lietotājs nosūta ziņojumu, izmantojot Outlook Mac vai Outlook Web, to nevar atsaukt.

Lai atsauktu vai aizstātu e-pasta ziņojumu:

1. Mapju rūtī, kas atrodas Outlook loga kreisajā pusē, atlasiet mapi Nosūtītie vienumi.
1. Veiciet dubultklikšķi uz ziņojuma, kuru vēlaties atsaukt, lai to atvērtu.
1. Atlasiet cilni **ziņojums** un pēc tam atlasiet **darbības**  >  **Atsaukt šo ziņojumu**.
1. Atlasiet **Dzēst šī ziņojuma nelasītās kopijas** vai **Dzēst nelasītās kopijas un aizstāt ar jaunu ziņojumu**un pēc tam atlasiet **Labi**.
1. Ja sūtāt ziņojumu ar aizstājējziņu, Sastādiet ziņojumu un pēc tam atlasiet **Sūtīt**.
1. Ziņojumu atsaukšanas izdošanās vai neveiksme ir atkarīga no adresāta iestatījumiem programmā Outlook. Lai pārbaudītu atsaukuma darbības, skatiet [šo rakstu](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

E-pasta ziņojumu meklēšana un dzēšana organizācijā

- Ja neesat globālais administrators, jūsu konts ir jāpievieno lomai eDiscovery Manager loma vai atbilstības meklēšanas pārvaldība, lai meklētu ziņojumus. Lai dzēstu ziņojumus, ir jāpievienojas organizācijas pārvaldības lomu grupai vai lomai meklēšanas un tīrīšanas pārvaldība. Šo lomu atļaujas tiek piešķirtas [drošības un atbilstības centrā](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Izveidojiet satura meklēšanu](https://docs.microsoft.com/microsoft-365/compliance/content-search) , lai atrastu dzēšamo ziņojumu.
- [Izveidot savienojumu ar drošības un atbilstības centra PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Ja izmantojat vairāku faktoru autentifikāciju, skatiet [izveidot savienojumu ar Microsoft 365 drošības un atbilstības centrs PowerShell, izmantojot vairāku faktoru autentifikācija](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).