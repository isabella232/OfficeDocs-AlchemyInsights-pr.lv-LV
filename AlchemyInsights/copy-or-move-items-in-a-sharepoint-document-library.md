---
title: Vienumu kopēšana vai pārvietošana SharePoint dokumentu bibliotēkā
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "454"
- "5300013"
ms.assetid: 592f502a-493f-4bf4-adc3-5bc8aea87bb5
ms.openlocfilehash: d7aa865a6b3db0871a57313dd7d6f5b0213ca0e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807126"
---
# <a name="copy-or-move-items-in-a-sharepoint-document-library"></a><span data-ttu-id="44996-102">Vienumu kopēšana vai pārvietošana SharePoint dokumentu bibliotēkā</span><span class="sxs-lookup"><span data-stu-id="44996-102">Copy or move items in a SharePoint document library</span></span>

<span data-ttu-id="44996-103">Varat kopēt un pārvietot failus, mapes un saites uz citu atrašanās vietu dokumentu bibliotēkā.</span><span class="sxs-lookup"><span data-stu-id="44996-103">You can copy and move files, folders, and links to different locations within a document library.</span></span> <span data-ttu-id="44996-104">Varat arī kopēt vienumus citās vietnēs.</span><span class="sxs-lookup"><span data-stu-id="44996-104">You can also copy items across sites.</span></span> 
  
1. <span data-ttu-id="44996-105">Pārlūkprogrammā pārlūkojiet līdz failiem, mapēm vai saitēm, ko vēlaties pārvietot, un pēc tam noklikšķiniet uz **Kopēt** vai **Pārvietot uz**.</span><span class="sxs-lookup"><span data-stu-id="44996-105">In a browser, browse to the files, folders, or links you want to move, and then click **Copy to** or **Move to**.</span></span>

    > [!NOTE]
    > <span data-ttu-id="44996-106">**Kopējiet uz** un **pārvietojiet uz** nav pieejami, ja izmantojat SharePoint Online klasisko pieredzi.</span><span class="sxs-lookup"><span data-stu-id="44996-106">**Copy to** and **Move to** aren't available if you're using the classic experience of SharePoint Online.</span></span>
  
2. <span data-ttu-id="44996-107">Sadaļā **izvēlēties mērķi**atlasiet atrašanās vietu, kurā vēlaties kopēt vai pārvietot vienumus, vai noklikšķiniet uz **Pārlūkot vietnes** , lai redzētu pilnu vietņu sarakstu.</span><span class="sxs-lookup"><span data-stu-id="44996-107">Under **Choose a destination**, select the location to which you want to copy or move the items or click **Browse sites** to see the full list of sites.</span></span>

    > [!NOTE]
    > <span data-ttu-id="44996-108">Ja, kopējot vienumus, netiek rādītas citas vietnes, kopēšana vairākās vietnēs nav konfigurēta.</span><span class="sxs-lookup"><span data-stu-id="44996-108">If you don't see other sites listed when you copy items, copying across sites hasn't been configured.</span></span> <span data-ttu-id="44996-109">Lai to iespējotu, dodieties uz SharePoint administrēšanas centra iestatījumu lapu un noklikšķiniet uz **Labi**.</span><span class="sxs-lookup"><span data-stu-id="44996-109">To enable it, go to the settings page of the SharePoint admin center and click **OK**.</span></span>
  
    <span data-ttu-id="44996-110">Lai izveidotu jaunu mapi, atlasiet atrašanās vietu mapju hierarhijā, noklikšķiniet uz **Jauna mape**, ievadiet mapes nosaukumu un noklikšķiniet uz atzīmes, lai saglabātu nosaukumu.</span><span class="sxs-lookup"><span data-stu-id="44996-110">To create a new folder, select a location in the folder hierarchy, click **New folder**, enter a name for the folder, and click the check mark to save the name.</span></span>

3. <span data-ttu-id="44996-111">Noklikšķiniet uz **Kopēt šeit** vai **Pārvietot šeit**.</span><span class="sxs-lookup"><span data-stu-id="44996-111">Click **Copy here** or **Move here**.</span></span>

    > [!NOTE]
    > <span data-ttu-id="44996-112">Varat vienlaikus kopēt līdz 500 MB failu un mapju.</span><span class="sxs-lookup"><span data-stu-id="44996-112">You can copy up to 500 MB of files and folders at one time.</span></span> <span data-ttu-id="44996-113">> kopējot dokumentus, kuriem ir versiju vēsture, tiek kopēta tikai jaunākā versija.</span><span class="sxs-lookup"><span data-stu-id="44996-113">>  When you copy documents that have version history, only the latest version is copied.</span></span> <span data-ttu-id="44996-114">Pārvietojot dokumentus, tiek pārvietoti arī to vēsture.</span><span class="sxs-lookup"><span data-stu-id="44996-114">When you move documents, their history is also moved.</span></span>
  
 <span data-ttu-id="44996-115">Kad fails tiek pārvietots, tas joprojām būs redzams avota direktorijā, līdz tas pilnībā tiks pārvietots uz mērķi, un pēc tam tas tiks dzēsts.</span><span class="sxs-lookup"><span data-stu-id="44996-115">When a file is moving, it will still appear in the source directory until its fully moved to the destination, and then it will be deleted.</span></span> <span data-ttu-id="44996-116">Fails paliks avota vietņu atkritnē pēc tam, kad pārvietošana būs pabeigta, un tiks pakļauts parastajam pārstrādes grafikam, ja vien lietotājs to neatkopj no atkritnes.</span><span class="sxs-lookup"><span data-stu-id="44996-116">The file will remain in the source sites recycle bin after the move is complete and be subject to the normal recycle schedule unless a user recovers it from the recycle bin.</span></span>

<span data-ttu-id="44996-117">Papildinformāciju skatiet rakstā:</span><span class="sxs-lookup"><span data-stu-id="44996-117">For more information, see:</span></span>

 - <span data-ttu-id="44996-118">[Failu pārvietošana vai kopēšana koplietošanas vidē SharePoint](https://support.office.com/article/move-or-copy-files-in-sharepoint-00e2f483-4df3-46be-a861-1f5f0c1a87bc) (Office atbalsta raksts)</span><span class="sxs-lookup"><span data-stu-id="44996-118">[Move or copy files in SharePoint](https://support.office.com/article/move-or-copy-files-in-sharepoint-00e2f483-4df3-46be-a861-1f5f0c1a87bc) (Office support article)</span></span>
 - <span data-ttu-id="44996-119">[Failu pārvietošana no jebkuras mapes](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Now-move-files-anywhere-in-Office-365-SharePoint-and-OneDrive/ba-p/146973) (Microsoft Tech Community blog raksts)</span><span class="sxs-lookup"><span data-stu-id="44996-119">[Move files from any folder](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Now-move-files-anywhere-in-Office-365-SharePoint-and-OneDrive/ba-p/146973) (Microsoft Tech Community blog article)</span></span>  