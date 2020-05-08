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
ms.openlocfilehash: b54457427ffa563b6a6323d85e1c8800191eca11
ms.sourcegitcommit: d1aad215f8aa636ba89c93a13a0c9d90e997f752
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/06/2020
ms.locfileid: "44064400"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problēmas, izveidojot grupu savienota vietnes SharePoint

1. Dažas bieži sastopamās problēmas radās, izveidojot vai atkārtoti izveidot savienojumu grupas vietni.
Ja esat izdzēsis grupu un tās Savienoto vietni un vēlaties izveidot citu vietni ar tādu pašu URL, jums vajadzēs neatgriezeniski noņemt iepriekšējo vietni.

   - Lejupielādēt [spo Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Papildinformāciju par darba sākšanu programmā PowerShell skatiet rakstā [Darba sākšana ar SharePoint Online pārvaldības čaulu](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Noņemt vietni no izdzēstās vietnes, izmantojot PowerShell cmdlet [Noņemt SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) . PowerShell ir nepieciešams neatgriezeniski dzēst grupas vietnes.

1. Ja veidojat ar grupu saistītu vietni un saņemat brīdinājumu: **cita grupa ar tādu pašu aizstājvārdu jau pastāv**, pārbaudiet esošās grupas no [Microsoft 365 administrēšanas centra](https://admin.microsoft.com/AdminPortal/Home#/groups). Lai novērstu šo problēmu, izdzēsiet esošo grupu, ja tā vairs nav nepieciešama vai izveidot vietni ar citu piešķirto aizstājvārdu.

1. Ir dažādi veidi, kā izveidot un izmantot modernas grupas ar SharePoint.

   - Esošās vietnes var savienot ar Microsoft 365 grupu. Papildinformāciju skatiet rakstā [Microsoft 365 grupas savienošana, izmantojot SharePoint lietotāja interfeisu](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Izveidot savienojumu ar Microsoft 365 grupas vietni, jums vajadzēs izveidot [darba grupas vietni](https://admin.microsoft.com/sharepoint).
