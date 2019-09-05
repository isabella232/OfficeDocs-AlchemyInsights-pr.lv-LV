---
title: Ierobežot SharePoint Online klasiskajā režīmā
ms.author: pebaum
author: Techwriter40
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 18d263593d99f24c3020336ae601df14dbbf5411
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752075"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="503a2-102">Ierobežot SharePoint Online klasiskajā režīmā</span><span class="sxs-lookup"><span data-stu-id="503a2-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="503a2-103">Daži uzņēmumi joprojām ir nepieciešama klasiskā režīma pieredzi.</span><span class="sxs-lookup"><span data-stu-id="503a2-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="503a2-104">Lai gan nav plānots noņemt klasisko režīmu granulētā līmenī, vairs nav iespējams ierobežot visu organizāciju (nomnieku) klasiskajā režīmā sarakstiem un bibliotēkām.</span><span class="sxs-lookup"><span data-stu-id="503a2-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="503a2-105">Admin būs šādas iespējas, lai pārvaldītu atsevišķus sarakstus un bibliotēkas klasiskā režīmā, izmantojot granulu atteikšanās slēdžus, ko mēs nodrošinām šādos līmeņos:</span><span class="sxs-lookup"><span data-stu-id="503a2-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="503a2-106">vietņu kolekciju</span><span class="sxs-lookup"><span data-stu-id="503a2-106">site collection</span></span>
- <span data-ttu-id="503a2-107">Vietnes</span><span class="sxs-lookup"><span data-stu-id="503a2-107">site</span></span>
- <span data-ttu-id="503a2-108">Sarakstu</span><span class="sxs-lookup"><span data-stu-id="503a2-108">list</span></span>
- <span data-ttu-id="503a2-109">Bibliotēkas</span><span class="sxs-lookup"><span data-stu-id="503a2-109">library</span></span>

<span data-ttu-id="503a2-110">Turklāt saraksti, kas izmanto noteiktus līdzekļus un pielāgojumus, kurus neatbalsta mūsdienīga, joprojām automātiski pārslēgsies uz klasisko režīmu.</span><span class="sxs-lookup"><span data-stu-id="503a2-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="503a2-111">Sākuma aprīlis 1, 2019, procesu, lai atspējotu nomnieka līmenī atteikties no mūsdienu sarakstu un bibliotēkas sāksies un turpināsies līdz maijam 31, 2019.</span><span class="sxs-lookup"><span data-stu-id="503a2-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="503a2-112">Saraksti un bibliotēkas, kas ir klasiskajā režīmā, kā rezultātā nomnieka atteikšanās tiks automātiski pārvietoti uz mūsdienu.</span><span class="sxs-lookup"><span data-stu-id="503a2-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="503a2-113">Ja jums ir nepieciešama Classic mode Lūdzu, skatiet plašāku informāciju [šeit](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) un PNP PowerShell instrukcija [šeit](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) , kas apraksta opcijas un rīki, kurus var izmantot šodien, lai izmantotu klasisko režīmu pieredzi.</span><span class="sxs-lookup"><span data-stu-id="503a2-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
