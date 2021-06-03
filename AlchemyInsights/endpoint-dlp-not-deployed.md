---
title: Galapunkta DLP nav izvietots lietotāja ierīcē
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/27/2021
ms.locfileid: "52731588"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a>Galapunkta DLP nav izvietots lietotāja ierīcē

Ja galapunkta datu zuduma novēršanas (DLP) iestatījums nav lietots lietotāja ierīcei, pārliecinieties, vai atbilstat šīm prasībām:

- Windows 10 ierīcē ir instalēts x64 būvējumu 1809 vai jaunāku versiju.
- Tiek instalēta ļaunprogrammatūras novēršanas klienta versija 4.18.2009.7 vai jaunāka versija.
- Ierīce ir **viena no** šīm:
    
    - Azure Active Directory (Azure AD) savienojums
    - Hibrīds Azure AD pievienots
    - AAD reģistrēts

- Lai ieviestu politikas darbības, pārliecinieties Chromium galapunkta ierīcē ir instalēta pārlūkprogramma Microsoft Chromium Edge.

Papildu prasības galapunkta DLP izvietošanai skatiet rakstā Darba [sākšana ar galapunktu datu zuduma novēršanu.](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints)