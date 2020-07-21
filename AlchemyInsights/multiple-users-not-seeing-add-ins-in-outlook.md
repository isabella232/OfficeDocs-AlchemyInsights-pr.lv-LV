---
title: Vairāki lietotāji neredz pievienojumprogrammas programmā Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197978"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="4d428-102">Vairāki lietotāji neredz pievienojumprogrammas programmā Outlook</span><span class="sxs-lookup"><span data-stu-id="4d428-102">Multiple users not seeing add-ins in Outlook</span></span>

<span data-ttu-id="4d428-103">Ja kā pirmo problēmu novēršanas darbību tiek pārbaudītas Outlook pievienojumprogrammas un neviena no tām nav parādīta, izmantojiet **cmdlet Get-OrganizationConfig** PowerShell, lai vaicātu _parametru AppsForOfficeEnabled._</span><span class="sxs-lookup"><span data-stu-id="4d428-103">If you test Outlook add-ins and none show up, as a first troubleshooting step, use the **Get-OrganizationConfig** PowerShell cmdlet to query the _AppsForOfficeEnabled_ parameter.</span></span> <span data-ttu-id="4d428-104">Ja vaicājums atgriež vērtību False , **iestatiet**šo parametru **uz True,** izmantojot cmdlet **Set-OrganizationConfig,** tāpēc pievienojumprogrammas tiek parādītas, kā paredzēts.</span><span class="sxs-lookup"><span data-stu-id="4d428-104">If the query returns a value of **False**, set this parameter to **True** by using the **Set-OrganizationConfig** cmdlet, so add-ins appear as expected.</span></span>

<span data-ttu-id="4d428-105">Nav ieteicams, ka _AppsForOfficeEnabled parametrs_ ir iestatīts uz **False**.</span><span class="sxs-lookup"><span data-stu-id="4d428-105">We do not recommend that the _AppsForOfficeEnabled_ parameter is set to **False**.</span></span> <span data-ttu-id="4d428-106">False vērtība **ignorē** visus iepriekš administratīvo un lietotāju lomu iestatījumus un neļauj jaunas programmas aktivizē jebkurš lietotājs organizācijā.</span><span class="sxs-lookup"><span data-stu-id="4d428-106">A value of **False** overrides all of the above Administrative and User role settings and prevents any new apps from being activated by any user in the organization.</span></span>

<span data-ttu-id="4d428-107">Papildinformāciju skatiet sadaļā To [administratoru un lietotāju nosaukāk, kuri var instalēt un pārvaldīt pievienojumprogrammas programmai Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span><span class="sxs-lookup"><span data-stu-id="4d428-107">For more information, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span></span>