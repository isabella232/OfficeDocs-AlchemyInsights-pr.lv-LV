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
ms.openlocfilehash: 23c57356c8bd94c1cbafb538c9318208429754115a7c4e88abc93d293b5ea6e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946586"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 kļūda, palaižot OneDrive

Ja, piesakoties **pakalpojumā 0x8004de40** pakalpojumā OneDrive, tiek atkārtoti palaists dators, kamēr ir izveidots savienojums ar darba vai mācību domēnu. Ja pēc atkārtotas palaišanas tiek parādīta šāda kļūda, mēģiniet to veikt, kamēr ir izveidots savienojums ar darba vai mācību domēnu.

1. Noklikšķiniet uz Sākt un  meklēšanas **lodziņā ierakstiet cmd** vai komandu uzvedne, ar peles labo pogu noklikšķiniet uz komandu uzvednes lietojumprogrammas un atlasiet Palaist **kā administratoram.** Ja saņemat aicinājumu ierakstīt administratora paroli vai apstiprinājumu, ierakstiet paroli vai noklikšķiniet uz **Atļaut**.  

2. Komandu uzvednes logā ierakstiet **dsregcmd /leave un**  gaidiet, līdz komanda tiek pabeigta. Pēc tam **ierakstiet dsregcmd /join un** gaidiet, līdz komanda tiek pabeigta.
3. Restartējiet datoru.
