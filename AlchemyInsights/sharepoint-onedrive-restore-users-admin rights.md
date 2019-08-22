---
title: Problēmu novēršanas pieeja liegta ziņojumus OneDrive darba vietām
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 39f9b9b1ca22f6e5959e2b431fb373b0002c0a92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507818"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Problēmu novēršanas pieeja liegta ziņojumus OneDrive darba vietām

Šī problēma visbiežāk rodas, ja lietotājs ir dzēsta un izveidota atkārtoti, izmantojot vienu un to pašu lietotāja pamatnosaukums (UPN). Jaunais konts ir izveidots, izmantojot citu PUID (pases unikālo ID) vērtību. Ja lietotājs mēģina piekļūt vietņu kolekcijā vai to OneDrive, lietotājam ir nepareiza PUID. Otrais scenārijs ietver directory sinhronizācija ar Active Directory organizācijas vienību (OU). Ja lietotāji jau pieslēdzās SharePoint, un tad ir pārvietots uz citu OU un resynced ar SharePoint, viņiem šī problēma var rasties.

1. Lai atrisinātu šo jautājumu vajadzētu atjaunot sākotnējo UPN ar rakstu,[atjaunot Office 365 lietotāja](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)darbības.
2. Ja sākotnējais lietotājs nevar atjaunot vecās lietotāja vajadzētu noņemt no OneDrive vietā, izmantojot šos norādījumus, [noņemtu kādu lietotāju, sarakstā lietotāja info](). 
3. Pēc tam, kad tas ir izdarīts, jūs varat pārbaudīt lietotājam nav administratora tiesības vietnē OneDrive, veiciet norādītās darbības, lai [pievienot admin lietotāja OneDrive kundzes](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Plašāku informāciju par atļauju līmeņiem, skatiet rakstā, [izpratne atļauju līmeņus koplietošanas vidē SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
