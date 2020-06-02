---
title: Ziņojumu piekļuve liegta ziņojumus OneDrive darba vietas
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 95bd46e8b7a6006f3735612d9a5602fb2b2a283b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511191"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Ziņojumu piekļuve liegta ziņojumus OneDrive darba vietas

Visbiežāk šī problēma rodas, ja lietotājs tiek dzēsts un atkārtoti izveidots ar pašu lietotāja pamatnosaukums (UPN). Jaunais konts ir izveidots, izmantojot citu PUID (Passport unikālo ID) vērtību. Kad lietotājs mēģina piekļūt vietņu kolekcijas vai to OneDrive, lietotājam ir nepareiza PUID. Otrs scenārijs ietver direktorija sinhronizēšana ar Active Directory organizatoriskajai vienībai (OU). Ja lietotāji jau ir pierakstījies SharePoint un pēc tam tiek pārvietoti uz citu OU un resynced ar SharePoint, tās var rasties šī problēma.

1. Lai novērstu šo problēmu, jums vajadzētu atjaunot sākotnējā UPN ar šajā rakstā aprakstītās darbības, [atjaunot lietotāju Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Ja nevarat atjaunot sākotnējo lietotāju, noņemiet veco lietotāju no vietnes OneDrive, veicot šīs darbības, [lietotāja informācijas sarakstā noņemiet lietotāju](). 
3. Pēc tam, kad tas ir izdarīts, varat pārbaudīt lietotājam ir administratora tiesības uz OneDrive vietni, izpildot darbības, lai [pievienotu admin lietotāja onedrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Papildinformāciju par atļauju līmeņiem skatiet rakstā [atļauju līmeņu izpratne SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
