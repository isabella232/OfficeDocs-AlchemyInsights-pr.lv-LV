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
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 20b538846997c021b6e88596a1e8aff401ea935b
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/12/2019
ms.locfileid: "29900885"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="45ed5-102">Novērst problēmas SharePoint satura koplietošana ar ārējiem lietotājiem</span><span class="sxs-lookup"><span data-stu-id="45ed5-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="45ed5-103">Pārliecinieties, vai jūsu uzņēmuma ārējā koplietošana ir ieslēgta:</span><span class="sxs-lookup"><span data-stu-id="45ed5-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="45ed5-104">Dodieties uz [pakalpojumus &amp; pievienojumprogrammas Office 365 admin centra lapā](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), un noklikšķiniet uz **vietas**.</span><span class="sxs-lookup"><span data-stu-id="45ed5-104">Go to the [Services &amp; add-ins page in the Office 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="45ed5-p101">Pārliecinieties, vai iestatījums ir ieslēgts, lai "Par". Ja atlasīts "Tikai esošajiem ārējiem lietotājiem", pārliecinieties, vai ārējais lietotājs ir iekļauts Office 365 administrēšanas centrs.</span><span class="sxs-lookup"><span data-stu-id="45ed5-p101">Make sure the setting is turned to "On." If "Only existing external users" is selected, make sure the external user is listed in the Office 365 admin center.</span></span>
    
<span data-ttu-id="45ed5-p102">Pārliecinieties, vai ārējā sadales to ieslēdzis vietā. Klasisks vietņu kolekcijas:</span><span class="sxs-lookup"><span data-stu-id="45ed5-p102">Make sure external sharing it turned on for the site. For a classic site collection:</span></span>
  
1. <span data-ttu-id="45ed5-109">Klasisks SharePoint administrēšanas centru, kreisajā rūtī noklikšķiniet uz **vietņu kolekcijas**.</span><span class="sxs-lookup"><span data-stu-id="45ed5-109">In the classic SharePoint admin center, in the left pane, click **site collections**.</span></span>
    
2. <span data-ttu-id="45ed5-110">Atlasiet vietu vai vietām, un uz lentes noklikšķiniet uz **koplietošana**.</span><span class="sxs-lookup"><span data-stu-id="45ed5-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="45ed5-111">Grupas vietnē Office 365 grupai piederošu vai saziņas vietne:</span><span class="sxs-lookup"><span data-stu-id="45ed5-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="45ed5-p103">Šīs jaunās vietnes tipi ir pašā koplietošanas iestatīšana kā uzņēmuma mēroga iestatījumu, ja vien uzņēmuma līmeņa iestatījums ļauj koplietot failus, izmantojot saites, kas nav nepieciešama pierakstīšanās. Šajā gadījumā vietņu ir atļauts koplietot ar jauniem un esošajiem ārējiem lietotājiem, kas pierakstīties. Lai mainītu iestatījumus konkrētām vietnēm, izmantojiet jauno SharePoint administrēšanas centru (priekšskatījuma) vai PowerShell. [Uzzināt vairāk](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="45ed5-p103">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in. In this case, the sites allow sharing with new and existing external users who sign in. To change the setting for specific sites, use the new SharePoint admin center (preview) or PowerShell. [Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="45ed5-116">Ārējās koplietošanas iestatījumu jebkurā vietā var būt stingrāki nekā uzņēmuma mēroga iestatījumu, taču ne vairāk pieļaujamām nekā uzņēmuma līmeņa iestatījums.</span><span class="sxs-lookup"><span data-stu-id="45ed5-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

