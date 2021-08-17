---
title: Problēmu novēršana saistībā ar piekļuvi liegtiem ziņojumiem
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9acde72f82a27c9f2faa2cf4d0417374aa5a294234da96080dc0498d07639248
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54085235"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Problēmu novēršana saistībā ar piekļuvi liegtiem ziņojumiem SharePoint/OneDrive centrā

Ja, mēģinot atvērt Sharepoint/OneDrive administrēšanas centru, tiek parādīts ziņojums par liegtu piekļuvi, pārliecinieties, vai piešķirat licenci [lietotājam.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) Ja lietotājam ir licence, pārliecinieties, vai lietotājam ir piešķirta administratora [loma,](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) kas var piekļūt administrēšanas centriem.

Šī problēma var rasties arī tad, ja lietotājs tiek izdzēsts un izveidots atkārtoti ar to pašu pamatnosaucību (user principal name — UPN). Jaunais konts tiek izveidots, izmantojot citu PUID (Passport Unique ID) vērtību. Kad lietotājs mēģina piekļūt vietņu kolekcijai vai viņa OneDrive, lietotājam ir nepareizs PUID. Otrajā scenārijā ir direktoriju sinhronizēšana ar Active Directory organizācijas vienību (OU). Ja lietotāji jau ir pierakstījušies SharePoint un pēc tam tiek pārvietoti uz citu OU un atkārtoti sinhronizēti ar SharePoint, iespējams, radusies šī problēma.

Lai novērstu šo problēmu, atjaunojiet sākotnējo UPN, izmantojot darbības, kas definētas rakstā Lietotāja [atjaunošana programmā Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)

Piezīme. Ja OneDrive vai SharePoint administrēšanas centrs nav pieejams vairākiem lietotājiem, kuriem iepriekš bija piekļuve, iespējams, ir īslaicīga pakalpojuma problēma.  [Pārbaudiet pakalpojuma darbspējas informācijas paneli](https://portal.office.com/adminportal/home#/servicehealth).


