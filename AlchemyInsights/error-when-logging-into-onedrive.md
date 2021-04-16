---
title: 0x8004de40 kļūda, palaižot OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813659"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 kļūda, palaižot OneDrive

Ja, piesakoties **pakalpojumā** OneDrive, 0x8004de40 kļūda, restartējiet datoru, kamēr ir izveidots savienojums ar darba vai mācību domēnu. Ja pēc atkārtotas palaišanas tiek parādīta šāda kļūda, mēģiniet to veikt, kamēr ir izveidots savienojums ar darba vai mācību domēnu.

1. Noklikšķiniet uz Sākt un  meklēšanas **lodziņā ierakstiet cmd** vai komandu uzvedne, ar peles labo pogu noklikšķiniet uz komandu uzvednes lietojumprogrammas un atlasiet Palaist **kā administratoram.** Ja saņemat aicinājumu ierakstīt administratora paroli vai apstiprinājumu, ierakstiet paroli vai noklikšķiniet uz **Atļaut**.  

2. Komandu uzvednes logā ierakstiet **dsregcmd /leave un**  gaidiet, līdz komanda tiek pabeigta. Pēc tam **ierakstiet dsregcmd /join un** gaidiet, līdz komanda tiek pabeigta.
3. Restartējiet datoru.
