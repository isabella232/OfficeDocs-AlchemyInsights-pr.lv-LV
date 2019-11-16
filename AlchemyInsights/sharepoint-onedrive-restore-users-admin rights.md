---
title: Ziņojumu piekļuve liegta ziņojumus OneDrive darba vietas
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 3c40ad76a8961a3d0b4963483291c2a1364c51d3
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 11/15/2019
ms.locfileid: "37766718"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Ziņojumu piekļuve liegta ziņojumus OneDrive darba vietas

Visbiežāk šī problēma rodas, ja lietotājs tiek dzēsts un atkārtoti izveidots ar pašu lietotāja pamatnosaukums (UPN). Jaunais konts ir izveidots, izmantojot citu PUID (Passport unikālo ID) vērtību. Kad lietotājs mēģina piekļūt vietņu kolekcijas vai to OneDrive, lietotājam ir nepareiza PUID. Otrs scenārijs ietver direktorija sinhronizēšana ar Active Directory organizatoriskajai vienībai (OU). Ja lietotāji jau ir pierakstījies SharePoint un pēc tam tiek pārvietoti uz citu OU un resynced ar SharePoint, tās var rasties šī problēma.

1. Lai novērstu šo problēmu, ir jāatjauno sākotnējā UPN ar šajā rakstā aprakstītās darbības, [atjaunojiet lietotāja Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Ja nevarat atjaunot sākotnējo lietotāju, noņemiet veco lietotāju no vietnes OneDrive, veicot šīs darbības, [lietotāja informācijas sarakstā noņemiet lietotāju](). 
3. Pēc tam, kad tas ir izdarīts, varat pārbaudīt lietotājam ir administratora tiesības uz OneDrive vietni, izpildot darbības, lai [pievienotu admin lietotāja onedrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Papildinformāciju par atļauju līmeņiem skatiet rakstā [atļauju līmeņu izpratne SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
