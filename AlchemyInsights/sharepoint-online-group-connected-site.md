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
ms.openlocfilehash: 14ad9dd094902c85eaf0398c76003cea20ad4c0a
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051108"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>Problēmas, veidojot vai grupu pievienotās vietnes SharePoint Online

Ir pāris bieži sastopamas problēmas, veidojot vai atkārtoti izveidot savienojumu grupas vietni.

 Ja esat izdzēsis grupu un tās Savienoto vietni un vēlaties izveidot citu vietni ar tādu pašu URL, jums vajadzēs neatgriezeniski noņemt iepriekšējo vietni.

Lejupielādēt [spo Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Papildinformāciju par darba sākšanu programmā PowerShell skatiet rakstā [Darba sākšana ar SharePoint Online pārvaldības čaulu](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Noņemt vietni no izdzēstās vietnes, izmantojot PowerShell cmdlet [Noņemt SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .

Ja veidojat ar grupu saistītu vietni un saņemat brīdinājumu, tad jau pastāv cita grupa ar šādu aizstājvārdu, pārbaudiet esošās grupas no [Office 365 no administrēšanas centra](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Lai novērstu šo problēmu, izdzēsiet esošo grupu, ja tā vairs nav nepieciešama vai izveidot vietni ar citu piešķirto aizstājvārdu.

Ir dažādi veidi, kā izveidot un izmantot modernas grupas ar SharePoint.

Esošās vietnes var savienot ar Office 365 grupu. Papildinformāciju skatiet rakstā [Office 365 grupas savienošana, izmantojot SharePoint lietotāja ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Lai izveidotu Office 365 grupu, kas ir savienota ar vietni, ir jāizveido darba grupas vietne. Papildinformāciju skatiet sadaļā [grupas vietnes izveide pakalpojumā SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

