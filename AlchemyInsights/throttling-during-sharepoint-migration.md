---
title: Ierobežošana SharePoint migrēšanas laikā
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom:
- "9000353"
- "1987"
- "9000136"
- "2968"
ms.assetid: ''
ms.openlocfilehash: dc77c462fcf32817c92709852e2d03ab2086b9a4
ms.sourcegitcommit: 926e4ab6aa64ddc7a244de633421eb2b817541f2
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/26/2020
ms.locfileid: "42958905"
---
# <a name="sharepoint-throttling"></a><span data-ttu-id="793a3-102">SharePoint ierobežošana</span><span class="sxs-lookup"><span data-stu-id="793a3-102">SharePoint throttling</span></span>

<span data-ttu-id="793a3-103">**Svarīgi**: šo bezprecedenta laiku mēs veicam darbības, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir plaši pieejami. Lai iegūtu papildinformāciju, apmeklējiet [SharePoint Online pagaidu līdzekļu pielāgojumi](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="793a3-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="793a3-104">**SharePoint Online ierobežošana**</span><span class="sxs-lookup"><span data-stu-id="793a3-104">**SharePoint Online throttling**</span></span>

<span data-ttu-id="793a3-105">SharePoint Online izmanto ierobežošanu, lai uzturētu optimālu SharePoint Online pakalpojuma veiktspēju un uzticamību.</span><span class="sxs-lookup"><span data-stu-id="793a3-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="793a3-106">Ierobežošana ierobežo lietotāju darbību vai vienlaicīgu zvanu skaitu (ar skriptu vai kodu), lai nepieļautu pārmērīgu resursu pielietojumu.</span><span class="sxs-lookup"><span data-stu-id="793a3-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span>

<span data-ttu-id="793a3-107">Lai iegūtu papildinformāciju, lūdzu, apmeklējiet šo tālāk norādītās saites:</span><span class="sxs-lookup"><span data-stu-id="793a3-107">For more information please visit the links below:</span></span>

- [<span data-ttu-id="793a3-108">Izvairīšanās no ierobežošanas vai bloķēšanas pakalpojumā SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="793a3-108">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)
- [<span data-ttu-id="793a3-109">Datu migrēšana un SPO ierobežošana</span><span class="sxs-lookup"><span data-stu-id="793a3-109">Data Migration and SPO Throttling</span></span>](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)
- [<span data-ttu-id="793a3-110">SharePoint Online un ODB migrēšanas ātrums</span><span class="sxs-lookup"><span data-stu-id="793a3-110">SharePoint Online and OneDrive Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)
- [<span data-ttu-id="793a3-111">SharePoint Online ierobežošana, izmantojot eksponenciālo atgriešanos</span><span class="sxs-lookup"><span data-stu-id="793a3-111">Handle SharePoint Online throttling by using exponential back off</span></span>](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)
- [<span data-ttu-id="793a3-112">Kapacitātes plānošana un slodzes pārbaude pakalpojumā SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="793a3-112">Capacity planning and load testing SharePoint Online</span></span>](https://support.office.com/article/Capacity-planning-and-load-testing-SharePoint-Online-c932bd9b-fb9a-47ab-a330-6979d03688c0)
- [<span data-ttu-id="793a3-113">Migrēšanas laikā radās vāja veiktspēja vai ierobežošana</span><span class="sxs-lookup"><span data-stu-id="793a3-113">I am experiencing poor performance or throttling during migration</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed#faq-and-troubleshooting)