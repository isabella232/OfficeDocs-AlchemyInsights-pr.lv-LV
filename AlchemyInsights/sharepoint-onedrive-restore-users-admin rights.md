---
title: Problēmu novēršanas pieeja liegta ziņojumus OneDrive darba vietām
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
ms.openlocfilehash: b394cc1441187133d8829cfc5fb0c1edbd71fd96
ms.sourcegitcommit: 204c8fadd59a597a18ebde24b3c63fbb656ec1b6
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223431"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Problēmu novēršanas pieeja liegta ziņojumus OneDrive darba vietām

Šī problēma visbiežāk rodas, ja lietotājs ir dzēsta un izveidota atkārtoti, izmantojot vienu un to pašu lietotāja pamatnosaukums (UPN). Jaunais konts ir izveidots, izmantojot citu PUID (pases unikālo ID) vērtību. Ja lietotājs mēģina piekļūt vietņu kolekcijā vai to OneDrive, lietotājam ir nepareiza PUID. Otrais scenārijs ietver directory sinhronizācija ar Active Directory organizācijas vienību (OU). Ja lietotāji jau pieslēdzās SharePoint, un tad ir pārvietots uz citu OU un resynced ar SharePoint, viņiem šī problēma var rasties.

Lai atrisinātu šo jautājumu vajadzētu atjaunot sākotnējo UPN ar rakstu,[atjaunot Office 365 lietotāja](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)darbības.

Pēc tam, kad tas ir izdarīts, jūs varat pārbaudīt lietotājam nav administratora tiesības vietnē OneDrive, veiciet norādītās darbības, lai [Pievienot admin lietotāja OneDrive kundzes](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Plašāku informāciju par atļauju līmeņiem, skatiet rakstā, [izpratne atļauju līmeņus koplietošanas vidē SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
