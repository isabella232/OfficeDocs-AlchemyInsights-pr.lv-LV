---
title: Ļauj lietotājiem piekļūt SharePoint un OneDrive
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: ae4d2c00be6387744bdc84e1d8a021530f80f8fa
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/04/2019
ms.locfileid: "34715218"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a>Ļauj lietotājiem piekļūt SharePoint un OneDrive

<p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Šī problēma visbiežāk rodas, ja lietotājs ir dzēsta un izveidota atkārtoti, izmantojot vienu un to pašu lietotāja pamatnosaukums (UPN). Jaunais konts ir izveidots, izmantojot citu PUID (pases unikālo ID) vērtību. Ja lietotājs mēģina piekļūt vietņu kolekcijā vai to OneDrive, lietotājam ir nepareiza PUID. Otrais scenārijs ietver directory sinhronizācija ar Active Directory organizācijas vienību (OU). Ja lietotāji jau pieslēdzās SharePoint, un tad ir pārvietots uz citu OU un resynced ar SharePoint, viņiem šī problēma var rasties.</span></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Lai atrisinātu šo jautājumu, vajadzētu atjaunot sākotnējo UPN ar rakstā aprakstītie soļi <a href="https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide">atjaunot lietotāja Office 365.</a></span></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Pēc tam, kad tas ir izdarīts, jūs varat pārbaudīt, lietotājam ir admin tiesības OneDrive vietā, veicot šādas darbības, lai <a href="https://docs.microsoft.com/en-us/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive">Pievienot admin lietotāja OneDrive.</a></span></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Plašāku informāciju par atļauju līmeņiem, skatiet rakstā, <a href="https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels">izpratni, atļauju līmeņi SharePoint.</a>&nbsp;</span></p>
