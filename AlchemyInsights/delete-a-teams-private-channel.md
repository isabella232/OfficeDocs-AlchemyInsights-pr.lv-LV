---
title: Teams privāta kanāla dzēšana
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439324"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="2f226-102">Teams privāta kanāla dzēšana</span><span class="sxs-lookup"><span data-stu-id="2f226-102">Delete a Teams private channel</span></span>

<span data-ttu-id="2f226-103">Microsoft ir informēta par problēmu, kas izdzēš Teams privāto kanālu, ja jums ir iespējots SharePoint saglabāšanas politikas pamatā esošajai SharePoint vietnei.</span><span class="sxs-lookup"><span data-stu-id="2f226-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="2f226-104">Microsoft strādā pie labojuma.</span><span class="sxs-lookup"><span data-stu-id="2f226-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="2f226-105">Tikmēr varat izmantot tālāk norādītos risinājumus, lai izdzēstu privāto kanālu.</span><span class="sxs-lookup"><span data-stu-id="2f226-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="2f226-106">**Izslēgt grupas/vietņu kolekciju no SharePoint saglabāšanas politikas.**</span><span class="sxs-lookup"><span data-stu-id="2f226-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="2f226-107">Dodieties uz Office 365 administrēšanas portālu un kreisajā navigācijas rūtī atlasiet **Rādīt visu** .</span><span class="sxs-lookup"><span data-stu-id="2f226-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="2f226-108">Sadaļā **administrēšanas centri**dodieties uz sadaļu **drošības & atbilstības**  >  **datu zuduma novēršanas**  >  **politika**.</span><span class="sxs-lookup"><span data-stu-id="2f226-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="2f226-109">Identificējiet politiku, kas attiecas uz SharePoint vietnēm, un modificējiet politiku, lai tā SharePoint vietne grupai, kurā ir privāts kanāls, nebūtu iekļauta saglabāšanas politikā.</span><span class="sxs-lookup"><span data-stu-id="2f226-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="2f226-110">Saglabājiet politiku.</span><span class="sxs-lookup"><span data-stu-id="2f226-110">Save the policy.</span></span>
    <span data-ttu-id="2f226-111">Lai politikas iestatījumi stātos spēkā, var paiet līdz pat 24 stundām.</span><span class="sxs-lookup"><span data-stu-id="2f226-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="2f226-112">Pēc tam, kad vietne ir izslēgta, varat izdzēst privāto kanālu.</span><span class="sxs-lookup"><span data-stu-id="2f226-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="2f226-113">Jūs, ***iespējams*** , varat izdzēst privāto kanālu, izmantojot Microsoft Teams savā Android ierīcē.</span><span class="sxs-lookup"><span data-stu-id="2f226-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="2f226-114">Saistīto SharePoint informāciju skatiet rakstā [nevar izdzēst vienumus pakalpojumā SharePoint Online vai OneDrive darbam](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span><span class="sxs-lookup"><span data-stu-id="2f226-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>