---
title: Lietotājs saņem kļūdu AADSTS7000112 Yammer ir atspējota
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198055"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a><span data-ttu-id="b8f58-102">Lietotājs saņem kļūdu AADSTS7000112 Yammer ir atspējota</span><span class="sxs-lookup"><span data-stu-id="b8f58-102">User receives error AADSTS7000112 Yammer is disabled</span></span>

<span data-ttu-id="b8f58-103">Ja saņemat kļūdas ziņojumu "AADSTS7000112: lietojumprogramma '00000005-0000-0ff1-ce00-0000000000"(Yammer) ir atspējota", rodas problēma ar pakalpojuma vadītāju Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b8f58-103">If you receive the error "AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled", a problem exists with the service principal within Azure AD.</span></span> <span data-ttu-id="b8f58-104">Administrators, iespējams, ir atspējojis pakalpojuma vadītāju, lai bloķētu piekļuvi Yammer.</span><span class="sxs-lookup"><span data-stu-id="b8f58-104">An administrator might have disabled the service principal to block access to Yammer.</span></span>

<span data-ttu-id="b8f58-105">Pakalpojuma vadītāja atspējošana nav ieteicama un var radīt papildu problēmas.</span><span class="sxs-lookup"><span data-stu-id="b8f58-105">Disabling the service principal is not recommended and can cause additional issues.</span></span> <span data-ttu-id="b8f58-106">Lai iegūtu papildinformāciju par atbalstīto pieeju, lai bloķētu lietotāju piekļuvi Yammer, [skatiet Yammer piekļuves izslēgšana Microsoft 365 lietotājiem](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span><span class="sxs-lookup"><span data-stu-id="b8f58-106">For more info about the supported approach to block user access to Yammer, see [Turn off Yammer access for Microsoft 365 users](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span></span>  

<span data-ttu-id="b8f58-107">Lai novērstu šo problēmu Azure portālā un atjaunot lietotāja piekļuvi Yammer:</span><span class="sxs-lookup"><span data-stu-id="b8f58-107">To correct this issue in the Azure Portal and restore user access to Yammer:</span></span>

1.  <span data-ttu-id="b8f58-108">Atveriet Azure Active Directory lapu un atlasiet **uzņēmuma lietojumprogrammas** **zem Pārvaldīt** kreisajā navigācijas rūtī.</span><span class="sxs-lookup"><span data-stu-id="b8f58-108">Open the Azure Active Directory page, and select **Enterprise applications** under **Manage** in the left navigation pane.</span></span>
3.  <span data-ttu-id="b8f58-109">Meklēšanas **lodziņā ierakstiet Office 365 Yammer** un atlasiet lietojumprogrammas nosaukumu, lai atvērtu iestatījumus.</span><span class="sxs-lookup"><span data-stu-id="b8f58-109">Type **Office 365 Yammer** in the search box, and select the application name to open settings.</span></span>
4.  <span data-ttu-id="b8f58-110">Kreisajā **navigācijas** **rūtī atlasiet** Rekvizīti zem Pārvaldīt.</span><span class="sxs-lookup"><span data-stu-id="b8f58-110">Select **Properties** under **Manage** in the left navigation pane.</span></span>
5.  <span data-ttu-id="b8f58-111">Vai iestatīt vērtību **Yes** **Iespējots, lai lietotāji varētu pierakstīties?** **Save**</span><span class="sxs-lookup"><span data-stu-id="b8f58-111">Set the value of **Enabled for users to sign-in?** to **Yes**, and then select **Save**.</span></span>
6.  <span data-ttu-id="b8f58-112">Vēlreiz pierakstieties pakalpojumā Yammer.</span><span class="sxs-lookup"><span data-stu-id="b8f58-112">Sign in to Yammer again.</span></span> <span data-ttu-id="b8f58-113">Iespējams, būs jānotīra sīkfaili.</span><span class="sxs-lookup"><span data-stu-id="b8f58-113">You might need to clear cookies.</span></span>

<span data-ttu-id="b8f58-114">Vai arī palaidiet PowerShell komandas, lai iestatītu vērtību.</span><span class="sxs-lookup"><span data-stu-id="b8f58-114">Alternatively, run PowerShell commands to set the value.</span></span> <span data-ttu-id="b8f58-115">Lai iegūtu papildinformāciju, [skatiet "Atvainojiet, bet mums ir problēmas ar pierakstīšanos"kļūda, noklikšķinot uz Yammer mozaīkas Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="b8f58-115">For more info, see ["Sorry, but we're having trouble signing you in" error when you click the Yammer tile in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span></span> 