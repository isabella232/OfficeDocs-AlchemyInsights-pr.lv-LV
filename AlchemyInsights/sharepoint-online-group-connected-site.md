---
title: Grupas pievienošana SharePoint vietnei
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: e7bfabe1555bb94e915f8544d460deecce6171be
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770358"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problēmas, izveidojot grupu savienota vietnes SharePoint

1. Dažas bieži sastopamās problēmas radās, izveidojot vai atkārtoti izveidot savienojumu grupas vietni.
Ja esat izdzēsis grupu un tās Savienoto vietni un vēlaties izveidot citu vietni ar tādu pašu URL, jums vajadzēs neatgriezeniski noņemt iepriekšējo vietni.

   - Lejupielādēt [spo Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Papildinformāciju par darba sākšanu programmā PowerShell skatiet rakstā [Darba sākšana ar SharePoint Online pārvaldības čaulu](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Noņemt vietni no izdzēstās vietnes, izmantojot PowerShell cmdlet [Noņemt SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) . PowerShell ir nepieciešams neatgriezeniski dzēst grupas vietnes.

1. Ja veidojat grupai pievienotu vietni un saņemat brīdinājumu: **cita grupa ar šādu aizstājvārdu jau pastāv**, pārbaudiet esošās grupas no [Office 365 administrēšanas centrs](https://admin.microsoft.com/AdminPortal/Home#/groups). Lai novērstu šo problēmu, izdzēsiet esošo grupu, ja tā vairs nav nepieciešama vai izveidot vietni ar citu piešķirto aizstājvārdu.

1. Ir dažādi veidi, kā izveidot un izmantot modernas grupas ar SharePoint.

   - Esošās vietnes var savienot ar Office 365 grupu. Papildinformāciju skatiet rakstā [Office 365 grupas savienošana, izmantojot SharePoint lietotāja interfeisu](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Lai izveidotu Office 365 grupu, kas ir savienota ar vietni, ir jāizveido [darba grupas vietne](https://admin.microsoft.com/sharepoint).
