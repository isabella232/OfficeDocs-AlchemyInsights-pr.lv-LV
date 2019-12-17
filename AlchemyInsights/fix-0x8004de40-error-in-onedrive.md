---
title: 0x8004de40 kļūdas labošana pakalpojumā OneDrive
ms.author: pebaum
author: pebaum
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 48b29f57763ca22a71a23b2afddcac0e8e8a95db
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052044"
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