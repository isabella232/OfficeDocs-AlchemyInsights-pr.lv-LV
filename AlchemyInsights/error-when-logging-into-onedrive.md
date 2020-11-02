---
title: 0x8004de40 kļūda, palaižot OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823052"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 kļūda, palaižot OneDrive

Ja, pierakstoties pakalpojumā OneDrive, saņemat kļūdas ziņojumu **0x8004de40** , restartējiet datoru, kamēr ir izveidots savienojums ar darba vai mācību iestādes domēnu. Ja pēc atsāknēšanas saņemat šo kļūdu, izmēģiniet to, kamēr ir izveidots savienojums ar darba vai mācību iestādes domēnu:

1. Noklikšķiniet uz Sākt un meklēšanas lodziņā ierakstiet **cmd** vai **komandu uzvedne**  , ar peles labo pogu noklikšķiniet uz komandu uzvednes lietojumprogrammas un atlasiet  **Palaist kā administratoram** . Ja tiek parādīta uzvedne ar aicinājumu ievadīt administratora paroli vai apstiprinājumu, ierakstiet paroli vai noklikšķiniet uz **Atļaut** .  

2. Komandu uzvednes logā ierakstiet **dsregcmd/Leave**  un uzgaidiet, līdz tiek pabeigta komanda. Pēc tam ierakstiet **dsregcmd/Join** un uzgaidiet, līdz tiek pabeigta komanda.
3. Restartējiet datoru.
