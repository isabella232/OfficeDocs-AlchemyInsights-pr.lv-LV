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
ms.openlocfilehash: 6a7c0497243ef7425917f54815e61f1244838c54
ms.sourcegitcommit: b14aa00b42ce4ca9d7dc3aa1fd57e66eae115447
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/28/2019
ms.locfileid: "30953351"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="b9a4c-102">Klasiskajā režīmā ierobežot SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="b9a4c-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="b9a4c-103">Daži uzņēmumi joprojām nepieciešama Classic režīmu pieredze.</span><span class="sxs-lookup"><span data-stu-id="b9a4c-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="b9a4c-104">Kamēr nav plānots noņemt klasiskajā režīmā granulveida līmenī, sākot aprīlis 1,2019, tas vairs nebūs iespējams ierobežot visam uzņēmumam (nomniekam) klasiskajā režīmā sarakstiem un bibliotēkām.</span><span class="sxs-lookup"><span data-stu-id="b9a4c-104">While there are no plans to remove classic mode at a granular level, starting April 1,2019, it will no longer be possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="b9a4c-105">Admin ir šādas opcijas, lai pārvaldītu atsevišķus sarakstus un bibliotēkas klasiskajā režīmā izmantojot granulveida atteikšanās slēdžiem, kurus mēs sniedzam šādos līmeņos:</span><span class="sxs-lookup"><span data-stu-id="b9a4c-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

<span data-ttu-id="b9a4c-106">bibliotēka - sarakstā vietnes kolekcijas - vietā-</span><span class="sxs-lookup"><span data-stu-id="b9a4c-106">-- site collection -- site -- list -- library</span></span>

<span data-ttu-id="b9a4c-107">Turklāt saraksti, kas noteiktu līdzekļu izmantošanai un pielāgojumi, kas nenodrošina mūsdienu tiks vēl automātiski pārslēgts uz klasiskajā režīmā.</span><span class="sxs-lookup"><span data-stu-id="b9a4c-107">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="b9a4c-108">Pēc 1. aprīļa, sarakstos un bibliotēkās, kas ir klasisks veids, kā rezultātā īrnieks atteikšanās automātiski vadīs vietnes līmenī un saraksta līmenī.</span><span class="sxs-lookup"><span data-stu-id="b9a4c-108">After April 1, lists and libraries that are in classic mode as a result of tenant opt-out will automatically be managed at the site level and list level.</span></span>

<span data-ttu-id="b9a4c-109">Ja jums ir nepieciešama klasiskajā režīmā Skatīt vairāk informācijas šeit un PnP Powershell instrukcija šeit, kas raksturo iespējas un instrumentus var izmantot šodien, lai sagatavotu izņemšanai īrnieks līmeņa atteikšanās 1. aprīlis.</span><span class="sxs-lookup"><span data-stu-id="b9a4c-109">If you require classic mode please see more information here and PnP Powershell instruction here that describes options and tools you can use today to prepare for the removal of the tenant level opt-out on April 1.</span></span>
