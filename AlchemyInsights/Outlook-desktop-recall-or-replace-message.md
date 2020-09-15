---
title: Outlook datora atsaukšana vai aizstāšana e-pasta ziņojums
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
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663997"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Outlook e-pasta ziņojuma atsaukšana vai aizstāšana

- Kā administrators varat **Atsaukt ziņojumus lietotāju vārdā, izmantojot PowerShell**. Jūs nevarat atsaukt ziņojumus no administrēšanas centra.
- Varat **tikai atsaukt ziņojumus, kas tiek nosūtīti lietotājiem jūsu organizācijā**. Ja ziņojums tika nosūtīts uz Gmail adresi, piemēram, varat to atsaukt.
- Jūs varat **no datora sūtīt ziņojumus tikai no Outlook 2016**. Ja lietotājs nosūta ziņojumu, izmantojot programmu Outlook darbam ar Mac vai Outlook tīmeklī, to nevar atsaukt.

Lai atsauktu vai aizstātu e-pasta ziņojumu:

1. Mapju rūtī, kas atrodas pa kreisi no Outlook loga, atlasiet mapi Nosūtītie vienumi.
1. Veiciet dubultklikšķi uz ziņojuma, ko vēlaties atsaukt, lai to atvērtu.
1. Atlasiet cilni **ziņojums** un pēc tam atlasiet **darbības**, lai  >  **atsauktu šo ziņojumu**.
1. Atlasiet **Dzēst šī ziņojuma nelasītās kopijas** vai **Dzēst nelasītās kopijas un aizstāt ar jaunu ziņojumu**un pēc tam atlasiet **Labi**.
1. Ja sūtāt aizstāšanas ziņojumu, izveidojiet ziņojumu un pēc tam atlasiet **Sūtīt**.
1. Ziņojuma atsaukšanas sekmīgs vai neizdošanās ir atkarīgs no adresāta iestatījumiem programmā Outlook. Lai uzzinātu, kādas darbības ir jāveic, skatiet [šo rakstu](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

E-pasta ziņojumu meklēšana un dzēšana savā organizācijā

- Ja neesat globālais administrators, jūsu kontam jābūt pievienotai e-datu atklāšanas pārvaldnieka lomai vai atbilstības meklēšanas pārvaldības lomai, lai meklētu ziņojumus. Lai izdzēstu ziņojumus, ir jāpievienojas organizācijas pārvaldības lomu grupai vai meklēšanas un iztīrīšanas pārvaldības lomai. Šo lomu atļaujas ir piešķirtas [drošības un atbilstības centrā](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Izveidojiet satura meklēšanu](https://docs.microsoft.com/microsoft-365/compliance/content-search) , lai atrastu dzēšamo ziņojumu.
- [Savienojuma izveide ar drošības un atbilstības centra PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Ja izmantojat daudzfaktoru autentifikāciju, skatiet rakstu [savienojuma izveide ar Microsoft 365 Security un Compliance Center PowerShell, izmantojot daudzfaktoru autentifikāciju](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).