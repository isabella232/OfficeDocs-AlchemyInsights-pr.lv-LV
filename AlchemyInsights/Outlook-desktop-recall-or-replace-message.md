---
title: Programma Outlook darbvirsmas atcerēties vai aizstāt e-pasta ziņojumu
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496118"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Atsauktu vai aizstātu Outlook e-pasta ziņojumu

- Kā administrators, varat **Atsaukt ziņojumus, izmantojot programmu PowerShell lietotāju vārdā**. Ziņas no admin center nevar atsaukt.
- Jūs varat **tikai atsaukt ziņojumus, kas nosūtīti cilvēkiem jūsu organizācijā**. Ja ziņojums tika nosūtīts Gmail adresi, piemēram, nevaru atcerēties to.
- Jūs varat **tikai atsaukt ziņojumus, kas nosūtīti no Outlook 2016 uz PC**. Ja lietotājs nosūta īsziņu, izmantojot Mac programmu Outlook vai Outlook Web, to nevar atsaukt.

Lai atsauktu vai aizstātu e-pasta ziņojumu:

1. Mapju rūtī Outlook loga kreisajā pusē, izvēlieties mapi Nosūtītie vienumi.
1. Veiciet dubultklikšķi uz ziņojuma, kuru vēlaties atsaukt, lai to atvērtu.
1. Atlasiet cilni **ziņojums** un pēc tam atlasiet **darbību** > **Atsaukt šo ziņojumu**.
1. Atlasiet **Dzēst šī ziņojuma nelasītās kopijas** vai **Dzēst nelasītās kopijas un aizstāt ar jaunu ziņojumu**un pēc tam **Labi**.
1. Ja sūtāt ziņojumu Nomaiņa, sastādīt ziņojumu un pēc tam atlasiet **nosūtīt**.
1. Ziņojuma atsaukšanas izdošanās vai neizdošanās ir atkarīga no adresāta iestatījumus programmā Outlook. Darbības, lai pārbaudītu par atsaukšanu, skatiet [šajā rakstā](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Meklēt un dzēst e-pasta ziņojumus savā uzņēmumā

- Ja jūs neesat globālās administrēšanas, jūsu kontā jābūt pievienotiem eDiscovery Manager lomu vai atbilstības meklēšanas pārvaldības loma, lai meklētu ziņojumus. Lai izdzēstu ziņas, jums pievienoties uzņēmuma pārvaldības lomu grupas vai meklēšanas un iztīrīs pārvaldības lomu. Atļaujas šīs lomas tiek piešķirtas [drošības un saskaņotības centrs](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Izveidošana satura meklēšanu](https://docs.microsoft.com/office365/securitycompliance/content-search) , lai atrastu ziņai un izdzēsiet.
- [Drošības un atbilstības centrā PowerShell savienojumu](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Ja jūs izmantojat vairāku faktoru autentifikaciju, skatiet [Office 365 drošību un atbilstību centra PowerShell savienojuma izveide, izmantojot vairāku faktoru autentifikaciju](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).