---
title: Izdzēstas vietnes atjaunošana
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 5/1/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 9e4e9ade058c60ecd7a6ce1b2a40c4996ac5676f
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 10/18/2019
ms.locfileid: "36552479"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="786db-102">Izdzēstas vietnes atjaunošana</span><span class="sxs-lookup"><span data-stu-id="786db-102">Restore a deleted site</span></span>

<span data-ttu-id="786db-103">Kad administrators izdzēš vietni, tā tiek ievietota vietņu kolekcijas atkritnē, kur tā tiek glabāta 93 dienas pirms tā tiek neatgriezeniski dzēsta.</span><span class="sxs-lookup"><span data-stu-id="786db-103">When an admin deletes a site , it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="786db-104">Lai atjaunotu vietni:</span><span class="sxs-lookup"><span data-stu-id="786db-104">To restore the site:</span></span>
  
1. <span data-ttu-id="786db-105">Jaunajā SharePoint administrēšanas centrā lentē noklikšķiniet uz **Atkritne** .</span><span class="sxs-lookup"><span data-stu-id="786db-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="786db-106">Atzīmējiet izvēles rūtiņu blakus vietņu kolekcijai, kuru vēlaties atjaunot.</span><span class="sxs-lookup"><span data-stu-id="786db-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="786db-107">Noklikšķiniet uz **atjaunot izdzēstos vienumus**.</span><span class="sxs-lookup"><span data-stu-id="786db-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="786db-108">Lai atjaunotu dzēstu saziņas vietni, varat izmantot jauno SharePoint administrēšanas centru.</span><span class="sxs-lookup"><span data-stu-id="786db-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="786db-109">Pretējā gadījumā jums ir nepieciešams, lai izmantotu Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="786db-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="786db-110">Lai atjaunotu vietni, kas pieder grupai Office 365, ir jāatjauno grupas Exchange administrēšanas centrs.</span><span class="sxs-lookup"><span data-stu-id="786db-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="786db-111">Grupas var atjaunot 30 dienas pēc to dzēšanas.</span><span class="sxs-lookup"><span data-stu-id="786db-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

