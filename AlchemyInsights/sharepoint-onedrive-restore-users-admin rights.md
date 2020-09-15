---
title: Piekļuve liegta ziņojumiem pakalpojumā OneDrive darbam vietnes
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
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670623"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Piekļuve liegta ziņojumiem pakalpojumā OneDrive darbam vietnes

Šī problēma visbiežāk rodas, ja lietotājs tiek izdzēsts un atkārtoti izveidots ar vienu un to pašu lietotāja pamatnosaukumu (UPN). Jaunais konts ir izveidots, izmantojot citu PUID (pases unikālā ID) vērtību. Kad lietotājs mēģina piekļūt vietņu kolekcijai vai to OneDrive, lietotājam ir nepareizs PUID. Otrais scenārijs ietver direktorija sinhronizēšanu ar Active Directory organizācijas vienību (OU). Ja lietotāji jau ir pierakstījušies pakalpojumā SharePoint, un pēc tam tiek pārvietoti uz citu un sinhronizētu ar SharePoint, šī problēma var rasties.

1. Lai atrisinātu šo problēmu, atjaunojiet sākotnējo UPN, veicot šajā rakstā norādītās darbības, [atjaunojiet lietotāju pakalpojumā Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Ja nevarat atjaunot oriģinālo lietotāju, no OneDrive vietnes Noņemiet veco lietotāju, veicot šīs darbības, lietotāja [informācijas sarakstā noņemiet lietotāju](). 
3. Kad tas ir paveikts, varat pārbaudīt, vai lietotājam ir administratora tiesības uz OneDrive vietni, izpildot darbības, kas jāveic, lai [pievienotu administratora atļaujas lietotāja OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Papildinformāciju par atļauju līmeņiem skatiet rakstā informācija par [SharePoint atļauju līmeņiem](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
