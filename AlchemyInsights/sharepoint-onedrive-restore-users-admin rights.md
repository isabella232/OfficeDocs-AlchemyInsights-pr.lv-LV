---
title: Problēmu novēršana saistībā ar piekļuvi liegtiem ziņojumiem OneDrive darbam vietnēs
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: fc4a2bd7dcc74f5f05e8b709e4bc3eac6ed445d6e2ea9ede698abbc8667723ce
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957800"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Problēmu novēršana saistībā ar piekļuvi liegtiem ziņojumiem OneDrive darbam vietnēs

Šī problēma visbiežāk rodas, ja lietotājs tiek izdzēsts un izveidots atkārtoti ar to pašu pamatnosaucību (user principal name — UPN). Jaunais konts tiek izveidots, izmantojot citu PUID (Passport Unique ID) vērtību. Kad lietotājs mēģina piekļūt vietņu kolekcijai vai viņa OneDrive, lietotājam ir nepareizs PUID. Otrajā scenārijā ir direktoriju sinhronizēšana ar Active Directory organizācijas vienību (OU). Ja lietotāji jau ir pierakstījušies SharePoint un pēc tam tiek pārvietoti uz citu OU un atkārtoti sinhronizēti ar SharePoint, iespējams, radusies šī problēma.

1. Lai novērstu šo problēmu, atjaunojiet sākotnējo UPN, izmantojot darbības, kas definētas rakstā [Lietotāja atjaunošana programmā Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)
2. Ja sākotnējo lietotāju nevarat atjaunot, vecais lietotājs ir jānoņem no vecās OneDrive, veicot šīs darbības: Lietotāja noņemšana [no lietotāja informācijas saraksta.]() 
3. Kad tas ir [paveikts,](https://docs.microsoft.com/sharepoint/manage-user-profiles) varat pārbaudīt, vai lietotājam ir administratora tiesības OneDrive vietnē, izpildot darbības, kas veicamas, lai pievienotu administratora tiesības lietotājam OneDrive

Papildinformāciju par atļauju līmeņiem skatiet rakstā Par [atļauju līmeņiem SharePoint.](https://docs.microsoft.com/sharepoint/understanding-permission-levels)
