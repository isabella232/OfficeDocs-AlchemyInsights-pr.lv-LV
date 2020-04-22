---
title: Ziņojumu par piekļuvi liegta problēmu novēršana
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 82e11458529b8a49e583b1a6963a51e2a466bfd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758471"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Piekļuve liegta ziņojumu novēršana programmā SharePoint/OneDrive administrēšanas centrs

Ja saņemat ziņojumu par liegtu piekļuvi, mēģinot pārlūkot SharePoint/OneDrive administrēšanas centrs, lūdzu, pārliecinieties, vai [piešķirt licenci lietotājam](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Ja lietotājam ir licence, pārliecinieties, ka viņiem ir [piešķirta administratora loma](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) , kas var piekļūt administrēšanas centriem.

Šī problēma var rasties arī tad, ja lietotājs ir izdzēsts un atkārtoti izveidots ar pašu lietotāja pamatnosaukums (UPN). Jaunais konts ir izveidots, izmantojot citu PUID (Passport unikālo ID) vērtību. Kad lietotājs mēģina piekļūt vietņu kolekcijas vai to OneDrive, lietotājam ir nepareiza PUID. Otrs scenārijs ietver direktorija sinhronizēšana ar Active Directory organizatoriskajai vienībai (OU). Ja lietotāji jau ir pierakstījies SharePoint un pēc tam tiek pārvietoti uz citu OU un resynced ar SharePoint, tās var rasties šī problēma.

Lai novērstu šo problēmu, jums vajadzētu atjaunot sākotnējā UPN ar šajā rakstā aprakstītās darbības, [atjaunot lietotāju Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Piezīme: ja OneDrive vai SharePoint administrēšanas centrs nav pieejams vairākiem lietotājiem, kuriem iepriekš bija piekļuve, var būt pagaidu pakalpojumu problēma.  [Pārbaudiet pakalpojuma darbspējas informācijas paneli](https://portal.office.com/adminportal/home#/servicehealth).


