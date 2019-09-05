---
title: 0x8004de40 kļūdas labošana pakalpojumā OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: aa0e0a63ac1e365a7cdce018626740446040a664
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755855"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>0x8004de40 kļūdas labošana pakalpojumā OneDrive

Ja pakalpojumā OneDrive tiek parādīta kļūda 0x8004de40:

- Atsāknējiet attiecīgajā datorā, kamēr izveidots savienojums ar Acitve direktorija domēns.
- Ja atsāknēšana neatrisina problēmu, atpievienojieties un atkārtoti Pievienojieties ierīcei no Azure AD. 

**Piezīme**: jums vajadzētu būt uzņēmuma tīklā, veicot šīs darbības. Neveiciet šīs darbības, ja nevarat izveidot savienojumu ar uzņēmuma infrastruktūru (piemēram, ceļojot). 

- Atveriet privileģēto komandu uzvedni. 
- Lai atvērtu privileģēto komandu uzvedni, noklikšķiniet uz **Sākt**, ar peles labo pogu noklikšķiniet uz **komandu uzvedne**un pēc tam noklikšķiniet uz **Palaist kā administratoram**.
- Ierakstiet *dsregcmd/Leave* un nospiediet taustiņu **Enter**.
- Kad pabeigta, ierakstiet *dsregcmd/Join* un nospiediet taustiņu **Enter**.
- Kad tas ir pabeigts, aizveriet komandu uzvedni.
- Atsāknējiet datoru un piesakieties pakalpojumā OneDrive.