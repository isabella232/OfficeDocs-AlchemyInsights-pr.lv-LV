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
ms.openlocfilehash: 352bad1b8fe219f95a37c9ac268c6c4dd8801dfc
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719488"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>Izveidot grupu pievienotās vietnes SharePoint Online

<p><strong>Tur ir pāris raksturīgām problēmām, kas radās, kad veidot vai atkārtoti veidot grupu saistītas vietnes.&nbsp;</strong></p>  <p>1.Ja jūs esat izdzēsis grupas un tās pievienoto vietni un vēlaties izveidot citā vietā ar tādu pašu URL, jums vajadzēs neatgriezeniski noņemt iepriekšējā vietā.</p>  <ul>  <li>Lejupielādēt <a title="SPO pārvaldības čaulu" href="https://support.office.com/en-ie/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429">SPO Management Shell</a> - vairāk info par iesākumam ar powershell, sk <a title="iesākumam ar SharePoint Online Management Shell" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Darba sākšana ar SharePoint Online Management Shell</a>. <br /><br /></li>  <li>Noņemiet vietni no vietas dzēsti, izmantojot <a title="noņemt SPODeletedSite" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Noņemt SPODeletedSite</a> powershell cmdlet.</li>  </ul>  <p>Ja jūs veidojat grupu pievienotās vietnes un saņemt brīdinājumu <strong>"cita grupa ar tāds pats aizstājvārds jau pastāv"</strong>, pārbaudīt esošās grupas no <a title="Office 365 no Admin Center" href="https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups">Biroja 365 no administrēšanas centrs</a>. Atrisinātu problēmu, izdzēst esošu grupu, ja tā vairs nav vajadzīga vai izveidot vietni ar citu aizstājvārdu piešķir.&nbsp;</p>  <p><strong>Ir dažādi veidi, kā izveidot un lietot mūsdienu grupām ar SharePoint.&nbsp;</strong></p>  <ol>  <li>Esošajās vietnēs var pieslēgties Office 365 grupa. Lai iegūtu vairāk informācijas, skatīt <a title="Savienojiet Office 365 grupu, izmantojot SharePoint lietotāja ineterface" href="https://docs.microsoft.com/en-us/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface">Savienojiet Office 365 grupu, izmantojot SharePoint lietotāja ineterface</a>.</li>  <li>Lai izveidotu Office 365 grupa pievienotās vietnes, jums vajadzēs radāt darba grupas vietni. Lai iegūtu vairāk informācijas, skatīt <a title="radiet darba grupas vietni koplietošanas vides SharePoint" href="https://support.office.com/en-us/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d">Radiet darba grupas vietni koplietošanas vidē SharePoint.</a></li>  </ol>

