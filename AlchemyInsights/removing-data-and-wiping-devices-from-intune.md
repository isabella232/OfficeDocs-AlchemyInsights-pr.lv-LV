---
title: Datu un tīrīšanas ierīču noņemšana no Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416320"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Datu un tīrīšanas ierīču noņemšana no Intune

Ierīces norakstīšanas un ierīces tīrīšanas attālās darbības var izmantot, lai noņemtu Intune pārvaldītos uzņēmuma datus vai veiktu rūpnīcas atiestatīšanu un atgrieztu ierīci noklusējuma iestatījumos.

1. Pierakstieties Microsoft 365 ierīču pārvaldībā un dodieties uz sadaļu **Ierīces** > **Visas ierīces**.
2. Atlasiet ierīci, kuru vēlaties tīrīt.
3. Atlasiet, kāda veida attālo tīrīšanu vēlaties veikt. Norakstīšanā tiek izdzēsta tikai organizācijas informācija, bet pilna tīrīšana atjauno ierīces rūpnīcas iestatījumus.
4. Atlasiet **Jā**, lai apstiprinātu. Līdz tīrīšana ir pabeigta, ierīces darbības statuss tiek rādīts kā *Gaida norakstīšanu*.
    Kad darbība būs pabeigta, mobilo ierīci vairs neredzēsit pārvaldītās ierīces sarakstā.

> [!NOTE]
> Uzņēmuma datus nevar noņemt no ierīcēm, kas PIEVIENOTAS Azure AD. 

Pilnu detalizētu informāciju par norakstīšanas un tīrīšanas darbībām, tostarp par to, kas tiek saglabāts un kas tiek izdzēsts, skatiet tālāk norādītajā dokumentācijā:

- [Noņemiet ierīces, izmantojot tīrīšanu, norakstīšanu vai manuāli atceliet ierīces reģistrāciju](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).
- [Kā tīrīt tikai uzņēmuma datus no Intune pārvaldītām lietojumprogrammām](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [Dzēsiet visus datus no MacOS ierīces](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).