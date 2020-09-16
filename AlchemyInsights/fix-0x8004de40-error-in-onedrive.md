---
title: 0x8004de40 kļūdas novēršana pakalpojumā OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745137"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>0x8004de40 kļūdas novēršana pakalpojumā OneDrive

Ja saņemat 0x8004de40 kļūdu pakalpojumā OneDrive:

- Atsāknējiet ietekmēto datoru, kamēr ir izveidots savienojums ar savu aktivs direktorija domēnu.
- Ja atsāknēšana nenovērš problēmu, Atsaistiet un atkārtoti Pievienojieties ierīcei no Azure AD. 

**Piezīme**. veicot šīs darbības, jums jāatrodas korporatīvajā tīklā. Neveiciet šīs darbības, ja nevarat izveidot savienojumu ar savas korporatīvās infrastruktūras (piemēram, ceļojuma laikā). 

- Atveriet privileģētu komandu uzvedni. 
- Lai atvērtu privileģētu komandu uzvedni, noklikšķiniet uz **Sākt**, ar peles labo pogu noklikšķiniet uz **komandu uzvedne**un pēc tam noklikšķiniet uz **Palaist kā administratoram**.
- Ierakstiet *dsregcmd/Leave* un nospiediet taustiņu **Enter**.
- Kad tas ir paveikts, ierakstiet *dsregcmd/Join* un nospiediet taustiņu **Enter**.
- Kad tas ir paveikts, izvērsiet komandu uzvedni.
- Restartējiet datoru un piesakieties pakalpojumā OneDrive.