---
title: Klasiskajā režīmā ierobežot SharePoint Online
ms.author: kirks
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
ms.openlocfilehash: 52c63d8909796f8d0d114a46c5255e4073e8c47d
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/28/2019
ms.locfileid: "35369780"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="a5143-102">Klasiskajā režīmā ierobežot SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="a5143-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="a5143-103">Daži uzņēmumi joprojām nepieciešama Classic režīmu pieredze.</span><span class="sxs-lookup"><span data-stu-id="a5143-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="a5143-104">Kamēr nav plānots noņemt klasiskajā režīmā granulveida līmenī, tas vairs nav iespējams ierobežot visam uzņēmumam (nomniekam) klasiskajā režīmā sarakstiem un bibliotēkām.</span><span class="sxs-lookup"><span data-stu-id="a5143-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="a5143-105">Admin ir šādas opcijas, lai pārvaldītu atsevišķus sarakstus un bibliotēkas klasiskajā režīmā izmantojot granulveida atteikšanās slēdžiem, kurus mēs sniedzam šādos līmeņos:</span><span class="sxs-lookup"><span data-stu-id="a5143-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="a5143-106">vietņu kolekcijas</span><span class="sxs-lookup"><span data-stu-id="a5143-106">site collection</span></span>
- <span data-ttu-id="a5143-107">vieta</span><span class="sxs-lookup"><span data-stu-id="a5143-107">site</span></span>
- <span data-ttu-id="a5143-108">saraksts</span><span class="sxs-lookup"><span data-stu-id="a5143-108">list</span></span>
- <span data-ttu-id="a5143-109">bibliotēka</span><span class="sxs-lookup"><span data-stu-id="a5143-109">library</span></span>

<span data-ttu-id="a5143-110">Turklāt saraksti, kas noteiktu līdzekļu izmantošanai un pielāgojumi, kas nenodrošina mūsdienu tiks vēl automātiski pārslēgts uz klasiskajā režīmā.</span><span class="sxs-lookup"><span data-stu-id="a5143-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="a5143-111">April 1, 2019, procesu, lai atspējotu īrnieks līmenis sāk atteikties no mūsdienu saraksta un bibliotēkas sāksies un turpināsies līdz 2019. gada 31 maijs.</span><span class="sxs-lookup"><span data-stu-id="a5143-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="a5143-112">Sarakstiem un bibliotēkām, kas ir klasisks veids, kā rezultātā īrnieks atteikšanās tiks automātiski pārvietoti uz mūsdienu.</span><span class="sxs-lookup"><span data-stu-id="a5143-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="a5143-113">Ja jums ir nepieciešama klasiskajā režīmā skatiet plašāku informāciju [šeit](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) un PnP Powershell instrukcija [šeit](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) , kas raksturo iespējas un rīkus, ko var izmantot šodien izmantot klasiskās sapratnes pieredzi.</span><span class="sxs-lookup"><span data-stu-id="a5143-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
