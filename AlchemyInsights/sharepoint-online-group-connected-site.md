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
ms.custom:
- "5200004"
- "5766"
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 8166c2a19e5849de6caace4eea0fee5866f5adc3bfc2c483f18fc788c1bf2fa9
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/11/2021
ms.locfileid: "57897723"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>Bieži sastopamas problēmas, veidojot ar grupu pievienotu vietni SharePoint

1. Ja esat izdzēsis grupu un tās savienoto vietni un vēlaties izveidot citu vietni ar tādu pašu vietrādi URL, iepriekšējā vietne ir jānoņem neatgriezeniski.

   - [SPO pārvaldības čaulas lejupielāde](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Papildinformāciju par darba sākšanu ar Powershell skatiet rakstā [Darba sākšana ar SharePoint Online pārvaldības čaulu.](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)
   - Noņemiet vietni no izdzēstām vietnēm, izmantojot Powershell cmdlet [Remove-SPODeletedSite.](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell ir nepieciešams, lai neatgriezeniski izdzēstu grupas vietnes.

1. Ja veidojat ar grupu savienotu vietni un saņemat **brīdinājumu:** Cita grupa ar tādu pašu aizstājvārdu jau pastāv, pārbaudiet esošās grupas no šīs [Microsoft 365 administrēšanas centrs.](https://admin.microsoft.com/AdminPortal/Home#/groups) Lai atrisinātu šo problēmu, izdzēsiet esošo grupu, ja tā vairs nav nepieciešama, vai izveidojiet vietni ar citu piešķirtu aizstājvārdu.

1. Ir dažādi veidi, kā izveidot un izmantot modernas grupas ar SharePoint.

   - Esošās vietnes var savienot ar Microsoft 365 grupu. Papildinformāciju skatiet rakstā [Savienošana grupas Microsoft 365, izmantojot SharePoint lietotāja interfeisu.](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)
   - Lai izveidotu Microsoft 365 ar grupu pievienotu vietni, ir jāizveido grupas [vietne.](https://admin.microsoft.com/sharepoint)
