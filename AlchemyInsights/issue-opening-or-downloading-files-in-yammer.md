---
title: Failu atvēršanas vai lejupielādes problēmu yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148333"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a><span data-ttu-id="fe4c4-102">Failu atvēršanas vai lejupielādes problēmu yammer</span><span class="sxs-lookup"><span data-stu-id="fe4c4-102">Issue opening or downloading files in Yammer</span></span>

<span data-ttu-id="fe4c4-103">Klasiskais Yammer atbalsta vairākas opcijas failu augšupielādei ziņojumos un grupās.</span><span class="sxs-lookup"><span data-stu-id="fe4c4-103">Classic Yammer supports multiple option for file uploads to messages and groups.</span></span> <span data-ttu-id="fe4c4-104">Atkarībā no tīkla konfigurācijas faili pēc noklusējuma tiek lietoti krātuvē koplietošanas vidē SharePoint.</span><span class="sxs-lookup"><span data-stu-id="fe4c4-104">Depending on network configuration, files default to storage in SharePoint.</span></span>

<span data-ttu-id="fe4c4-105">Failu izvēle jaunā Yammer vēl neatbalsta visas opcijas, kas pieejamas klasiskajā Yammer.</span><span class="sxs-lookup"><span data-stu-id="fe4c4-105">The file picker in new Yammer does not yet support all the options available in classic Yammer.</span></span> <span data-ttu-id="fe4c4-106">Nākamajā atjauninājumā tiks pievienoti papildu līdzekļi.</span><span class="sxs-lookup"><span data-stu-id="fe4c4-106">A future update will add additional features.</span></span> <span data-ttu-id="fe4c4-107">Papildinformāciju skatiet rakstā [Faila vai attēla pievienošana Yammer sarunas ziņai](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span><span class="sxs-lookup"><span data-stu-id="fe4c4-107">For more info, see [Attach a file or image to a Yammer conversation post](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span></span>

<span data-ttu-id="fe4c4-108">**Nevar atvērt vai lejupielādēt failu**</span><span class="sxs-lookup"><span data-stu-id="fe4c4-108">**Unable to open or download a file**</span></span>  

<span data-ttu-id="fe4c4-109">Fails var augšupielādēt Yammer, bet arī saites uz failu SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="fe4c4-109">A file might upload to Yammer but also be linking to a file in SharePoint Online.</span></span> <span data-ttu-id="fe4c4-110">Lai novērstu problēmas, vispirms ir jānosaka faila atrašanās vieta.</span><span class="sxs-lookup"><span data-stu-id="fe4c4-110">To troubleshoot, first you must determine the location of the file.</span></span> <span data-ttu-id="fe4c4-111">Ja fails ir augšupielādēts Yammer, tam būs \*.yammer.com URL.</span><span class="sxs-lookup"><span data-stu-id="fe4c4-111">If the file has been uploaded to Yammer, it will have a \*.yammer.com URL.</span></span> <span data-ttu-id="fe4c4-112">Pārliecinieties, vai nepieciešamie vietrāži URL un IP adreses tiek atbloķēti.</span><span class="sxs-lookup"><span data-stu-id="fe4c4-112">Ensure that required URLs and IP addresses are unblocked.</span></span> <span data-ttu-id="fe4c4-113">Lai iegūtu papildinformāciju, skatiet emuāra [ziņu Izmantojot grūti kodēta IP adreses Yammer nav ieteicams](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span><span class="sxs-lookup"><span data-stu-id="fe4c4-113">For more info, see the blog post [Using hard coded IP addresses for Yammer is not recommended](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span></span>

<span data-ttu-id="fe4c4-114">Pārbaudiet, vai lietotājs, kurš ir arī globālais administrators, var lejupielādēt failu.</span><span class="sxs-lookup"><span data-stu-id="fe4c4-114">Check whether a user who is also a global admin can download the file.</span></span> <span data-ttu-id="fe4c4-115">Ja fails ir privāts, iespējams, ir jāizmanto privātā satura režīms.</span><span class="sxs-lookup"><span data-stu-id="fe4c4-115">If the file is private, you might have to use Private Content Mode.</span></span> <span data-ttu-id="fe4c4-116">Papildinformāciju skatiet rakstā Privātā [satura pārraudzība pakalpojumā Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span><span class="sxs-lookup"><span data-stu-id="fe4c4-116">For more info, see then [Monitor private content in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span></span>  

<span data-ttu-id="fe4c4-117">**Yammer tīkla līmeņa viesi un faili pakalpojumā SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="fe4c4-117">**Yammer network-level guests and files in SharePoint Online**</span></span>  

<span data-ttu-id="fe4c4-118">[Tīkla līmeņa viesi Yammer neizmanto](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) Azure AD B2B un ir iekšējā Yammer pakalpojumu, lai viņi nevar piekļūt Yammer failus, kas saglabāti SharePoint.</span><span class="sxs-lookup"><span data-stu-id="fe4c4-118">[Network-level guests in Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) do not use Azure AD B2B and are internal to the Yammer service, so they can't access Yammer files stored in SharePoint.</span></span> <span data-ttu-id="fe4c4-119">Izveidojiet ārēju AAD B2B lietotāju, kurš var piekļūt dokumentu bibliotēkām pakalpojumā SharePoint Online, izmantojot šo identitāti.</span><span class="sxs-lookup"><span data-stu-id="fe4c4-119">Create an external AAD B2B user who can access document libraries in SharePoint Online by using that identity.</span></span> <span data-ttu-id="fe4c4-120">Informāciju par turpmāko Azure AD B2B viesu atbalstu pakalpojumā Yammer skatiet rakstā [Biznesa-to-business (B2B) viesu atbalsts pakalpojumā Yammer Preview — klientu nosacījumi un bieži uzdotie jautājumi](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span><span class="sxs-lookup"><span data-stu-id="fe4c4-120">For information about future Azure AD B2B guest support in Yammer, see [Business-to-business (B2B) Guest support in Yammer Preview - Customer Terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span></span>