---
title: Koplietošana ar ārējiem lietotājiem nedarbojas
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 9a40f52637bc8aa7894754118f0f862aa6c71fe2
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582782"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="4941c-102">SharePoint satura koplietošanas ar ārējiem lietotājiem problēmu novēršana</span><span class="sxs-lookup"><span data-stu-id="4941c-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="4941c-103">Pārliecinieties, vai jūsu organizācijai ir ieslēgta ārēja koplietošana.</span><span class="sxs-lookup"><span data-stu-id="4941c-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="4941c-104">Dodieties uz [pakalpojumu &amp; pievienojumprogrammas lapā Microsoft 365 administrēšanas centrs](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)un noklikšķiniet uz **vietnes**.</span><span class="sxs-lookup"><span data-stu-id="4941c-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="4941c-105">Pārliecinieties, vai iestatījums ir ieslēgts.</span><span class="sxs-lookup"><span data-stu-id="4941c-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="4941c-106">Ja ir atlasīts "tikai esošie ārējie lietotāji", pārliecinieties, vai ārējais lietotājs ir norādīts Microsoft 365 administrēšanas centrā.</span><span class="sxs-lookup"><span data-stu-id="4941c-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="4941c-107">Pārliecinieties, vai ārējā koplietošana tā ir ieslēgta vietnei.</span><span class="sxs-lookup"><span data-stu-id="4941c-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="4941c-108">Klasiskajai vietņu kolekcijai:</span><span class="sxs-lookup"><span data-stu-id="4941c-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="4941c-109">Jaunajā SharePoint administrēšanas centrā kreisajā rūtī noklikšķiniet uz **vietnes**.</span><span class="sxs-lookup"><span data-stu-id="4941c-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="4941c-110">Atlasiet vietni vai vietnes un lentē noklikšķiniet uz **koplietošana**.</span><span class="sxs-lookup"><span data-stu-id="4941c-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="4941c-111">Grupas vietne, kas pieder Microsoft 365 grupas vai saziņas vietnes:</span><span class="sxs-lookup"><span data-stu-id="4941c-111">For a team site that belongs to a Microsoft 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="4941c-112">Šiem jaunajiem vietnes tipiem ir tāds pats kopīgošanas iestatījums kā organizācijas iestatījumam, ja vien organizācijas mēroga iestatījums neļauj koplietot failus, izmantojot saites, kurām nav nepieciešama pierakstīšanās.</span><span class="sxs-lookup"><span data-stu-id="4941c-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="4941c-113">Šajā gadījumā vietnes ļauj koplietot ar jauniem un esošiem ārējiem lietotājiem, kuri ir pierakstīgi.</span><span class="sxs-lookup"><span data-stu-id="4941c-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="4941c-114">Lai mainītu iestatījumu konkrētām vietnēm, izmantojiet jauno SharePoint administrēšanas centru vai PowerShell.</span><span class="sxs-lookup"><span data-stu-id="4941c-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="4941c-115">[Papildinformācija](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="4941c-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="4941c-116">Jebkuras vietnes ārējās koplietošanas iestatījums var būt ierobežojošāks nekā jūsu organizācijas iestatījums, bet ne vairāk, nekā tas ir iespējams visā organizācijā.</span><span class="sxs-lookup"><span data-stu-id="4941c-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

