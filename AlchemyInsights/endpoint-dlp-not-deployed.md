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
# <a name="endpoint-dlp-not-deployed-to-users-device"></a><span data-ttu-id="bc1e2-102">Galapunkta DLP nav izvietots lietotāja ierīcē</span><span class="sxs-lookup"><span data-stu-id="bc1e2-102">Endpoint DLP not deployed to user's device</span></span>

<span data-ttu-id="bc1e2-103">Ja galapunkta datu zuduma novēršanas (DLP) iestatījums nav lietots lietotāja ierīcei, pārliecinieties, vai atbilstat šīm prasībām:</span><span class="sxs-lookup"><span data-stu-id="bc1e2-103">If the Endpoint data loss prevention (DLP) setting has not applied to a user's device, confirm you meet these requirements:</span></span>

- <span data-ttu-id="bc1e2-104">Windows 10 ierīcē ir instalēts x64 būvējumu 1809 vai jaunāku versiju.</span><span class="sxs-lookup"><span data-stu-id="bc1e2-104">Windows 10 x64 build 1809 or later is installed on the device.</span></span>
- <span data-ttu-id="bc1e2-105">Tiek instalēta ļaunprogrammatūras novēršanas klienta versija 4.18.2009.7 vai jaunāka versija.</span><span class="sxs-lookup"><span data-stu-id="bc1e2-105">Anti-malware client version 4.18.2009.7 or later is installed.</span></span>
- <span data-ttu-id="bc1e2-106">Ierīce ir **viena no** šīm:</span><span class="sxs-lookup"><span data-stu-id="bc1e2-106">The device is **one** of these:</span></span>
    
    - <span data-ttu-id="bc1e2-107">Azure Active Directory (Azure AD) savienojums</span><span class="sxs-lookup"><span data-stu-id="bc1e2-107">Azure Active Directory (Azure AD) joined</span></span>
    - <span data-ttu-id="bc1e2-108">Hibrīds Azure AD pievienots</span><span class="sxs-lookup"><span data-stu-id="bc1e2-108">Hybrid Azure AD joined</span></span>
    - <span data-ttu-id="bc1e2-109">AAD reģistrēts</span><span class="sxs-lookup"><span data-stu-id="bc1e2-109">AAD registered</span></span>

- <span data-ttu-id="bc1e2-110">Lai ieviestu politikas darbības, pārliecinieties Chromium galapunkta ierīcē ir instalēta pārlūkprogramma Microsoft Chromium Edge.</span><span class="sxs-lookup"><span data-stu-id="bc1e2-110">To enforce policy actions, make sure Microsoft Chromium Edge browser is installed on the endpoint device.</span></span>

<span data-ttu-id="bc1e2-111">Papildu prasības galapunkta DLP izvietošanai skatiet rakstā Darba [sākšana ar galapunktu datu zuduma novēršanu.](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints)</span><span class="sxs-lookup"><span data-stu-id="bc1e2-111">For additional requirements for deploying Endpoint DLP, see [Get started with Endpoint data loss prevention](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).</span></span>