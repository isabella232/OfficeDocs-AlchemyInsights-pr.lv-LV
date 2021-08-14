---
title: Paraugprakses izmantošana, lai iegūtu uzlabotus meklēšanas vaicājumus
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: e2a22563a840cd6017afd343bad108be216738742938a48ba5ceb1010fd16098
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930140"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Paraugprakses izmantošana, lai iegūtu uzlabotus meklēšanas vaicājumus

Lai ātrāk iegūtu rezultātus un izvairītos no taimautiem, kamēr izpildāt sarežģītus vaicājumus, lietojiet šos vislabākās prakses piemērus:

- Mēģinot jaunus vaicājumus, vienmēr izmantojiet ierobežojumu, lai izvairītos no ļoti lielu rezultātu kopu iegūšanas. Izmantojiet `count` arī, lai veiktu rezultātu kopas lieluma sākotnējo novērtējumu.
- Vispirms izmantojiet laika filtrus. Ideālā gadījumā ierobežojiet vaicājumus līdz septiņām dienām.
- Vaicājuma sākumā tieši pēc laika filtra pievienojiet filtrus, kas tiek plānoti, lai noņemtu lielāko daļu datu.
- Meklējot pilnos marķierus, `has` izmantojiet operatoru, nevis `contains` .
- Veikt meklēšanu konkrētā kolonnā, nevis visās kolonnās.
- Savienojot tabulas, vispirms norādiet tabulu ar mazāk rindām.
- `project` tikai nepieciešamās kolonnas no tabulām, kuras esat pievienojis.

Papildinformāciju skatiet rakstā Papildu [meklēšanas vaicājumu vislabākā prakse.](https://go.microsoft.com/fwlink/?linkid=2144812)
