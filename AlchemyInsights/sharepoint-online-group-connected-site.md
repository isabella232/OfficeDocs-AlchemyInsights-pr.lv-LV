---
title: Grupas pievienošana SharePoint vietnei
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: f0126f7f753275e9bbf8c3a09a6af5faf9a27862
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758737"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>Izveidot grupu pievienotās vietnes SharePoint Online

Tur ir pāris raksturīgām problēmām, kas radās, kad veidot vai atkārtoti veidot grupu saistītas vietnes.

 Ja jūs esat izdzēsis grupas un tās pievienoto vietni un vēlaties izveidot citā vietā ar tādu pašu URL, jums vajadzēs neatgriezeniski noņemt iepriekšējā vietā.

Lejupielādējiet [SPO pārvaldības čaulu](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Lai iegūtu vairāk informācijas par iesākumam ar powershell, skatiet [Darba sākšana ar SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Noņemiet vietni no Izdzēstie vietnēs, izmantojot [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.

Ja veidojat grupu pievienotās vietnes un saņemt brīdinājumu citu grupu ar tāds pats aizstājvārds jau pastāv, pārbaudiet esošās grupas no [Office 365 no administrēšanas centrs](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Atrisinātu problēmu, izdzēst esošu grupu, ja tā vairs nav vajadzīga vai izveidot vietni ar citu aizstājvārdu piešķir.

Ir dažādi veidi, kā izveidot un lietot mūsdienu grupām ar SharePoint.

Esošajās vietnēs var pieslēgties Office 365 grupa. Lai iegūtu vairāk informācijas, skatiet [savienojuma izveidošana Office 365 grupu, izmantojot SharePoint lietotāja ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Lai izveidotu Office 365 grupa pievienotās vietnes, jums vajadzēs radāt darba grupas vietni. Lai iegūtu vairāk informācijas, skatiet [Create darba grupas vietni koplietošanas vidē SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

