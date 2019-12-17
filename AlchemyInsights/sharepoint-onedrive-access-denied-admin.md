---
title: Ziņojumu par piekļuvi liegta problēmu novēršana
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 57919e6dbd81a5bf3b17fb067485e8eec23b7d4c
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051432"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Piekļuve liegta ziņojumu novēršana programmā SharePoint/OneDrive administrēšanas centrs

Ja saņemat ziņojumu par liegtu piekļuvi, mēģinot pārlūkot SharePoint/OneDrive administrēšanas centrs, lūdzu, pārliecinieties, vai [piešķirt licenci lietotājam](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Ja lietotājam ir licence, pārliecinieties, ka viņiem ir [piešķirta administratora loma](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) , kas var piekļūt administrēšanas centriem.

Šī problēma var rasties arī tad, ja lietotājs ir izdzēsts un atkārtoti izveidots ar pašu lietotāja pamatnosaukums (UPN). Jaunais konts ir izveidots, izmantojot citu PUID (Passport unikālo ID) vērtību. Kad lietotājs mēģina piekļūt vietņu kolekcijas vai to OneDrive, lietotājam ir nepareiza PUID. Otrs scenārijs ietver direktorija sinhronizēšana ar Active Directory organizatoriskajai vienībai (OU). Ja lietotāji jau ir pierakstījies SharePoint un pēc tam tiek pārvietoti uz citu OU un resynced ar SharePoint, tās var rasties šī problēma.

Lai novērstu šo problēmu, jums vajadzētu atjaunot sākotnējā UPN ar šajā rakstā aprakstītās darbības, [atjaunojiet lietotāja Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Piezīme: ja OneDrive vai SharePoint administrēšanas centrs nav pieejams vairākiem lietotājiem, kuriem iepriekš bija piekļuve, var būt pagaidu pakalpojumu problēma.  [Pārbaudiet pakalpojuma darbspējas informācijas paneli](https://portal.office.com/adminportal/home#/servicehealth).


