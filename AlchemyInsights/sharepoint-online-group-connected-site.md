---
title: Grupas pievienošana SharePoint vietnei
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771215"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problēmas, veidojot grupas savienotu vietni koplietošanas vidē SharePoint

1. Dažas bieži sastopamas problēmas, kas rodas, veidojot vai atkārtoti izveidojot grupu savienotu vietni.
Ja esat izdzēsis grupu un tās pievienoto vietni un vēlaties izveidot citu vietni ar vienu un to pašu vietrādi URL, ir jānoņem iepriekšējā vietne.

   - Lejupielādēt [spo pārvaldības čaulu](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Lai iegūtu papildinformāciju par darba sākšanu pakalpojumā PowerShell, skatiet rakstu [Darba sākšana ar SharePoint Online pārvaldības čaulu](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Noņemiet vietni no izdzēstajām vietnēm, izmantojot funkciju [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell cmdlet. PowerShell ir nepieciešama, lai neatgriezeniski dzēstu grupas vietnes.

1. Ja izveidojat grupai pievienotu vietni un saņemat brīdinājumu: **cita grupa ar tādu pašu aizstājvārdu jau pastāv**, atzīmējiet esošās grupas no [Microsoft 365 administrēšanas centra](https://admin.microsoft.com/AdminPortal/Home#/groups). Lai atrisinātu šo problēmu, izdzēsiet esošo grupu, ja tā vairs nav vajadzīga, vai izveidojiet vietni ar atšķirīgu aizstājvārdu.

1. Pastāv vairāki veidi, kā izveidot un izmantot mūsdienīgas grupas ar SharePoint.

   - Esošās vietnes varat savienot ar Microsoft 365 grupu. Papildinformāciju skatiet rakstā [Microsoft 365 grupas savienošana, izmantojot SharePoint lietotāja interfeisu](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Lai izveidotu savienotu Microsoft 365 grupu, ir jāizveido [grupas vietne](https://admin.microsoft.com/sharepoint).
