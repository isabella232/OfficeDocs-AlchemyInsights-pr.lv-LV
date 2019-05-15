---
title: Mūsdienu vietni kā saknes vietni
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057739"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="394f0-102">Mūsdienu vietni kā saknes</span><span class="sxs-lookup"><span data-stu-id="394f0-102">Modern site as root site</span></span>

<span data-ttu-id="394f0-103">[Release mērķa](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) klienti tagad var aktivizēt mūsdienu saziņas vietnes pieredzi savas SharePoint īrnieka vietā klasiskās saknes.</span><span class="sxs-lookup"><span data-stu-id="394f0-103">[Target Release](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) customers can now enable the modern communication site experience at the classic root site of their SharePoint tenant.</span></span>

<span data-ttu-id="394f0-104">Šo funkciju var aktivizēt, izpildot vienkāršas PowerShell cmdlet.</span><span class="sxs-lookup"><span data-stu-id="394f0-104">This feature can be activated by running a simple PowerShell cmdlet.</span></span> <span data-ttu-id="394f0-105">Saknes vietne PowerShell command(s) sekmīgu izpildi, būs jaunas saziņas vietnes mājas lapā.</span><span class="sxs-lookup"><span data-stu-id="394f0-105">On the successful execution of the PowerShell command(s), the root site will have a new communication site home page.</span></span> <span data-ttu-id="394f0-106">Detalizēta informācija par prasībām PowerShell cmdlet un iezīme ir pieejamo [Iespējot SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps)rakstu.</span><span class="sxs-lookup"><span data-stu-id="394f0-106">Details about the PowerShell cmdlet and feature requirements are available in the article [Enable-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span></span> 

<span data-ttu-id="394f0-107">Mums būs pakāpeniski ritošo šo out, izslēgts pēc noklusējuma, mērķtiecīgi presei klientiem jau maijā 2019 un izskrējienu būs pieejams visā pasaulē 2019 jūnija beigās.</span><span class="sxs-lookup"><span data-stu-id="394f0-107">We'll be gradually rolling this out, off by default, to Targeted Release customers in early May 2019, and the roll out will be available worldwide by the end of June 2019.</span></span> <span data-ttu-id="394f0-108">Arī turpmāk atsaukties uz [Īsziņu centru](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) citas jaunas funkcijas ar modernu.</span><span class="sxs-lookup"><span data-stu-id="394f0-108">Continue to refer to the [Message Center](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) for other new features with Modern.</span></span> 

<span data-ttu-id="394f0-109">**Svarīgi**: klasiskās saknes vietne, lai izveidotu mūsdienīgu saziņas vietne netiek dzēstas.</span><span class="sxs-lookup"><span data-stu-id="394f0-109">**Important**: Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="394f0-110">Šī korporācija Microsoft to neatbalsta.</span><span class="sxs-lookup"><span data-stu-id="394f0-110">This is not supported by Microsoft.</span></span> <span data-ttu-id="394f0-111">Saknes vietnes dzēšana padarīs visas SharePoint vietnes organizācijā nepieejama visiem lietotājiem, kamēr vietā atjaunot vai izveidot jaunu vietni ar tādu pašu URL.</span><span class="sxs-lookup"><span data-stu-id="394f0-111">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> 
 
 