---
title: Nedarbojas koplietošanas ar ārējiem lietotājiem
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 69e290e5a13f40ad045086791189a7d0af88240b
ms.sourcegitcommit: 228c986911ecf73217116a5d1fdcd2e89362774e
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/09/2019
ms.locfileid: "31747605"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="c340c-102">Novērst problēmas SharePoint satura koplietošana ar ārējiem lietotājiem</span><span class="sxs-lookup"><span data-stu-id="c340c-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="c340c-103">Pārliecinieties, vai jūsu uzņēmuma ārējā koplietošana ir ieslēgta:</span><span class="sxs-lookup"><span data-stu-id="c340c-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="c340c-104">Dodieties uz [pakalpojumus &amp; pievienojumprogrammas Microsoft 365 admin centra lapā](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), un noklikšķiniet uz **vietas**.</span><span class="sxs-lookup"><span data-stu-id="c340c-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="c340c-105">Pārliecinieties, vai iestatījums ir ieslēgts, lai "Par".</span><span class="sxs-lookup"><span data-stu-id="c340c-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="c340c-106">Ja atlasīts "Tikai esošajiem ārējiem lietotājiem", pārliecinieties, vai ārējais lietotājs ir iekļauts Microsoft 365 administrēšanas centrs.</span><span class="sxs-lookup"><span data-stu-id="c340c-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="c340c-107">Pārliecinieties, vai ārējā sadales to ieslēdzis vietā.</span><span class="sxs-lookup"><span data-stu-id="c340c-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="c340c-108">Klasisks vietņu kolekcijas:</span><span class="sxs-lookup"><span data-stu-id="c340c-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="c340c-109">Jaunu SharePoint administrēšanas centru, kreisajā rūtī noklikšķiniet uz **vietnes**.</span><span class="sxs-lookup"><span data-stu-id="c340c-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="c340c-110">Atlasiet vietu vai vietām, un uz lentes noklikšķiniet uz **koplietošana**.</span><span class="sxs-lookup"><span data-stu-id="c340c-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="c340c-111">Grupas vietnē Office 365 grupai piederošu vai saziņas vietne:</span><span class="sxs-lookup"><span data-stu-id="c340c-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="c340c-112">Šīs jaunās vietnes tipi ir pašā koplietošanas iestatīšana kā uzņēmuma mēroga iestatījumu, ja vien uzņēmuma līmeņa iestatījums ļauj koplietot failus, izmantojot saites, kas nav nepieciešama pierakstīšanās.</span><span class="sxs-lookup"><span data-stu-id="c340c-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="c340c-113">Šajā gadījumā vietņu ir atļauts koplietot ar jauniem un esošajiem ārējiem lietotājiem, kas pierakstīties.</span><span class="sxs-lookup"><span data-stu-id="c340c-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="c340c-114">Lai mainītu iestatījumus konkrētām vietnēm, izmantojiet jauno SharePoint administrēšanas centru vai PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c340c-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="c340c-115">[Uzzināt vairāk](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="c340c-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="c340c-116">Ārējās koplietošanas iestatījumu jebkurā vietā var būt stingrāki nekā uzņēmuma mēroga iestatījumu, taču ne vairāk pieļaujamām nekā uzņēmuma līmeņa iestatījums.</span><span class="sxs-lookup"><span data-stu-id="c340c-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

