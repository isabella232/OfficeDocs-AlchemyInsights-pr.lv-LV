---
title: Datu noņemšana un ierīču tīrīšana no Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439646"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Datu noņemšana un ierīču tīrīšana no Intune

Ierīces pārtraukšanas un ierīces tīrīšanas attālās darbības var izmantot, lai noņemtu uzņēmuma datus, kurus pārvalda Intune, vai lai veiktu rūpnīcas atiestatīšanu un atgrieztu ierīces noklusējuma iestatījumus.

1. Pierakstieties Microsoft 365 ierīču pārvaldībā un dodieties uz **ierīces**  >  **visas ierīces**.
2. Atlasiet ierīci, kuru vēlaties izdzēst.
3. Atlasiet, kāda veida attālo tīrīšanu vēlaties veikt. Pensionējoties dzēš tikai organizācijas informāciju, bet pilna tīrīšana atjauno ierīces rūpnīcas iestatījumus.
4. Atlasiet **Jā** , lai apstiprinātu. Līdz brīdim, kad tīrīšana ir pabeigta, ierīces darbības statuss tiek rādīts kā pensija gaida.</br>
    Kad darbība ir pabeigta, jūs vairs neredzat mobilo ierīci pārvaldītās ierīces sarakstā.

**Piezīmes** Uzņēmuma datus nevar noņemt no ierīcēm, kas SAVIENOTas ar Azure AD.

Lai iegūtu pilnu informāciju par atkāpju un tīrīšanas darbību sekām, tostarp par to, kas tiek paturēts un kas tiek izdzēsts, skatiet rakstu [Ierīču noņemšana, izmantojot notīrīšanu, pensionēju vai manuāli](https://docs.microsoft.com/intune/devices-wipe)atsaucot ierīci.

Informāciju par visu datu izdzēšanu no macOS ierīces skatiet rakstā [visu datu dzēšana no MacOS ierīces](https://docs.microsoft.com/intune/device-erase).