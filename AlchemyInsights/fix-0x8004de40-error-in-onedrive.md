---
title: 0x8004de40 kļūdas labošana pakalpojumā OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716035"
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