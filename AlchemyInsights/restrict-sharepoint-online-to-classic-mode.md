---
title: SharePoint Online ierobežošana klasiskajā režīmā
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751429"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="17a33-102">SharePoint Online ierobežošana klasiskajā režīmā</span><span class="sxs-lookup"><span data-stu-id="17a33-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="17a33-103">Dažām organizācijām ir nepieciešama klasiska režīma pieredze.</span><span class="sxs-lookup"><span data-stu-id="17a33-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="17a33-104">Kamēr nav plānu noņemt klasisko režīmu granulētā līmenī, vairs nav iespējams ierobežot visu organizāciju (nomnieku) uz klasisko režīmu sarakstiem un bibliotēkām.</span><span class="sxs-lookup"><span data-stu-id="17a33-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="17a33-105">Lai klasiskajā režīmā pārvaldītu atsevišķus sarakstus un bibliotēkas, administratoram ir pieejamas šādas opcijas: tālāk norādītajos līmeņos izmantojiet granulu atteikuma slēdžus.</span><span class="sxs-lookup"><span data-stu-id="17a33-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="17a33-106">vietņu kolekcija</span><span class="sxs-lookup"><span data-stu-id="17a33-106">site collection</span></span>
- <span data-ttu-id="17a33-107">vietnes</span><span class="sxs-lookup"><span data-stu-id="17a33-107">site</span></span>
- <span data-ttu-id="17a33-108">sarakstā</span><span class="sxs-lookup"><span data-stu-id="17a33-108">list</span></span>
- <span data-ttu-id="17a33-109">bibliotēkā</span><span class="sxs-lookup"><span data-stu-id="17a33-109">library</span></span>

<span data-ttu-id="17a33-110">Turklāt saraksti, kuros izmantoti noteikti līdzekļi un pielāgojumi, ko neatbalsta mūsdienīgs, joprojām tiks automātiski pārslēgti uz klasisko režīmu.</span><span class="sxs-lookup"><span data-stu-id="17a33-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="17a33-111">Sākot ar 2019. aprīli, tiek sākta darbība, lai atspējotu nomnieka līmeņa atteikšanos no modernā saraksta un bibliotēkām un turpinātu līdz 31. maijam 2019.</span><span class="sxs-lookup"><span data-stu-id="17a33-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="17a33-112">Saraksta un bibliotēkas, kas ir klasiskajā režīmā kā nomnieka atteikuma rezultāts, tiks automātiski pārbīdītas uz mūsdienīgu.</span><span class="sxs-lookup"><span data-stu-id="17a33-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="17a33-113">Ja jums ir nepieciešams klasiskais režīms, papildinformāciju skatiet [šeit](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) un PNP PowerShell [instrukcijā](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) , kurā aprakstītas opcijas un rīki, ko var izmantot šodien, lai izmantotu klasisko režīmu.</span><span class="sxs-lookup"><span data-stu-id="17a33-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
