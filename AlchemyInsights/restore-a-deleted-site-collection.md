---
title: Izdzēstas vietnes atjaunošana
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 570284765f32212b4ef2062db5b70f427b28c121
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47692050"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="97dd4-102">Izdzēstas vietnes atjaunošana</span><span class="sxs-lookup"><span data-stu-id="97dd4-102">Restore a deleted site</span></span>

<span data-ttu-id="97dd4-103">Kad administrators izdzēš SharePoint vietni, tā tiek ievietota vietņu kolekcijas atkritnē, kur tā tiek glabāta 93 dienas, pirms tā tiek neatgriezeniski izdzēsta.</span><span class="sxs-lookup"><span data-stu-id="97dd4-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="97dd4-104">Lai atjaunotu vietni:</span><span class="sxs-lookup"><span data-stu-id="97dd4-104">To restore the site:</span></span>
  
1. <span data-ttu-id="97dd4-105">Jaunajā SharePoint administrēšanas centrā lentē noklikšķiniet uz **Atkritne** .</span><span class="sxs-lookup"><span data-stu-id="97dd4-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="97dd4-106">Atzīmējiet izvēles rūtiņu blakus vietņu kolekcijai, kuru vēlaties atjaunot.</span><span class="sxs-lookup"><span data-stu-id="97dd4-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="97dd4-107">Noklikšķiniet uz **atjaunot izdzēstos vienumus**.</span><span class="sxs-lookup"><span data-stu-id="97dd4-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="97dd4-108">Lai atjaunotu izdzēstu saziņas vietni, varat izmantot jauno SharePoint administrēšanas centru.</span><span class="sxs-lookup"><span data-stu-id="97dd4-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="97dd4-109">Pretējā gadījumā jums ir jāizmanto Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="97dd4-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="97dd4-110">Lai atjaunotu vietni, kas pieder Microsoft 365 grupai, šī grupa ir jāatjauno Exchange administrēšanas centrā.</span><span class="sxs-lookup"><span data-stu-id="97dd4-110">To restore a site that belongs to a Microsoft 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="97dd4-111">Grupas var atjaunot 30 dienas pēc tam, kad tās ir izdzēstas.</span><span class="sxs-lookup"><span data-stu-id="97dd4-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

