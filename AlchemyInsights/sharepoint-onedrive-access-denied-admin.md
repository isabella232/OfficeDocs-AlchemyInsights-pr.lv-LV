---
title: Piekļuve liegta ziņojumu novēršana
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767669"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Problēmu novēršana saistībā ar piekļuvi liegti SharePoint/OneDrive administrēšanas centrā

Ja tiek saņemts ziņojums par liegtu piekļuvi, mēģinot pārlūkot SharePoint/OneDrive administrēšanas centru, pārliecinieties, vai jums ir [piešķirta licence lietotājam](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Ja lietotājam ir licence, pārliecinieties arī, vai tiem ir [piešķirta administratora loma](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) , kas var piekļūt administrēšanas centriem.

Šī problēma var rasties arī tad, ja lietotājs tiek izdzēsts un atkārtoti izveidots ar vienu un to pašu lietotāja pamatnosaukumu (UPN). Jaunais konts ir izveidots, izmantojot citu PUID (pases unikālā ID) vērtību. Kad lietotājs mēģina piekļūt vietņu kolekcijai vai to OneDrive, lietotājam ir nepareizs PUID. Otrais scenārijs ietver direktorija sinhronizēšanu ar Active Directory organizācijas vienību (OU). Ja lietotāji jau ir pierakstījušies pakalpojumā SharePoint, un pēc tam tiek pārvietoti uz citu un sinhronizētu ar SharePoint, šī problēma var rasties.

Lai atrisinātu šo problēmu, atjaunojiet oriģinālo UPN, veicot rakstā norādītās darbības, [atjaunojiet lietotāju pakalpojumā Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Piezīme. Ja jūsu OneDrive vai SharePoint administrēšanas centrs nav pieejams vairākiem lietotājiem, kuriem agrāk bija piekļuve, iespējama īslaicīga pakalpojumu problēma.  [Skatiet pakalpojuma darbspējas informācijas paneli](https://portal.office.com/adminportal/home#/servicehealth).


