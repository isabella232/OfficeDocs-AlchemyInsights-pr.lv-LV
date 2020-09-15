---
title: Koplietošana ar ārējiem lietotājiem nedarbojas
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691582"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="55cc3-102">Problēmu novēršana saistībā ar SharePoint satura koplietošanu ar ārējiem lietotājiem</span><span class="sxs-lookup"><span data-stu-id="55cc3-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="55cc3-103">Pārliecinieties, vai jūsu organizācijā ir ieslēgta ārējā koplietošana:</span><span class="sxs-lookup"><span data-stu-id="55cc3-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="55cc3-104">Atveriet [ &amp; Microsoft 365 administrēšanas centra lapu pakalpojumu pievienojumprogrammas](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)un noklikšķiniet uz **vietnes**.</span><span class="sxs-lookup"><span data-stu-id="55cc3-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="55cc3-105">Pārliecinieties, vai iestatījums ir ieslēgts.</span><span class="sxs-lookup"><span data-stu-id="55cc3-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="55cc3-106">Ja ir atlasīts tikai esošie ārējie lietotāji, pārliecinieties, vai ārējais lietotājs ir norādīts Microsoft 365 administrēšanas centrā.</span><span class="sxs-lookup"><span data-stu-id="55cc3-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="55cc3-107">Pārliecinieties, vai šī vietne ir ieslēgta ar ārējo koplietošanu.</span><span class="sxs-lookup"><span data-stu-id="55cc3-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="55cc3-108">Klasiskai vietņu kolekcijai:</span><span class="sxs-lookup"><span data-stu-id="55cc3-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="55cc3-109">Jaunajā SharePoint administrēšanas centrā kreisajā rūtī noklikšķiniet uz **vietnes**.</span><span class="sxs-lookup"><span data-stu-id="55cc3-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="55cc3-110">Atlasiet vietni vai vietnes un lentē noklikšķiniet uz **koplietošana**.</span><span class="sxs-lookup"><span data-stu-id="55cc3-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="55cc3-111">Grupas vietnē, kas pieder Microsoft 365 grupai, vai saziņas vietne:</span><span class="sxs-lookup"><span data-stu-id="55cc3-111">For a team site that belongs to a Microsoft 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="55cc3-112">Šiem jaunajiem vietņu tipiem ir vienāds kopīgošanas iestatījums atbilstoši organizācijas iestatījumiem, ja vien organizācijas mēroga iestatījums nenodrošina failu koplietošanu, izmantojot saites, kurām nav nepieciešama pierakstīšanās.</span><span class="sxs-lookup"><span data-stu-id="55cc3-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="55cc3-113">Šajā gadījumā vietnes atļauj koplietošanu ar jauniem un esošiem ārējiem lietotājiem, kuri pierakstās.</span><span class="sxs-lookup"><span data-stu-id="55cc3-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="55cc3-114">Lai mainītu noteiktu vietņu iestatījumu, izmantojiet jauno SharePoint administrēšanas centru vai PowerShell.</span><span class="sxs-lookup"><span data-stu-id="55cc3-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="55cc3-115">[Papildinformācija](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="55cc3-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="55cc3-116">Jebkuras vietnes ārējās koplietošanas iestatījums var būt vairāk ierobežojošs nekā organizācijas mēroga iestatījums, bet ne vairāk pieļaujams nekā organizācijas mēroga iestatījums.</span><span class="sxs-lookup"><span data-stu-id="55cc3-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

