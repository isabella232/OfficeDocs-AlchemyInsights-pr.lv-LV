---
title: Yammer tīmekļa daļas vidē SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5475"
- "9002494"
ms.openlocfilehash: d8b4043bb2889429a18c477505e7eca662943051
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664357"
---
# <a name="yammer-web-parts-in-sharepoint"></a><span data-ttu-id="dbbca-102">Yammer tīmekļa daļas vidē SharePoint</span><span class="sxs-lookup"><span data-stu-id="dbbca-102">Yammer web parts in SharePoint</span></span>

<span data-ttu-id="dbbca-103">Yammer sarunas un Yammer uzsver tīmekļa daļas Uzlabojiet sadarbību modernās un klasiskās SharePoint lapās.</span><span class="sxs-lookup"><span data-stu-id="dbbca-103">Yammer Conversations and Yammer Highlights web parts enhance collaboration on modern and classic SharePoint pages.</span></span> <span data-ttu-id="dbbca-104">Papildinformāciju skatiet rakstā [Yammer sarunas](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#conversations)  un  [Yammer Highlights](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#highlights).</span><span class="sxs-lookup"><span data-stu-id="dbbca-104">For more info, see [Yammer Conversations](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#conversations)  and  [Yammer Highlights](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#highlights).</span></span>    

<span data-ttu-id="dbbca-105">Modernās Yammer sarunas tīmekļa daļa tiek atjaunināta uz jauno Yammer pieredzi, un tā ir pieejama konkrētiem laidiena nomniekiem.</span><span class="sxs-lookup"><span data-stu-id="dbbca-105">The modern Yammer Conversations web part is being updated to the new Yammer experience and is available for Targeted Release tenants.</span></span> <span data-ttu-id="dbbca-106">Ir sākusies GA izvēršana.</span><span class="sxs-lookup"><span data-stu-id="dbbca-106">GA rollout has started.</span></span> <span data-ttu-id="dbbca-107">Jauni līdzekļi ietver iespēju sākt sarunu ar jebkuru ziņu (jautājumi, aptaujas, uzslava) un atzīmēt labākās atbildes tieši no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="dbbca-107">New features include the ability to start a conversation with any post (Questions, Polls, Praise) and to mark best answers directly from SharePoint.</span></span> <span data-ttu-id="dbbca-108">Papildinformāciju skatiet rakstā [jauni Yammer klientu termini un bieži uzdotie jautājumi](https://docs.microsoft.com/yammer/get-started-with-yammer/newyammer-faq).</span><span class="sxs-lookup"><span data-stu-id="dbbca-108">For more info, see [New Yammer customer terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/newyammer-faq).</span></span>

 <span data-ttu-id="dbbca-109">Lai izprastu, kura tīmekļa daļa un konfigurācija jums ir piemērota, skatiet rakstu [Yammer tīmekļa daļa izmantošana pakalpojumā SharePoint Online](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da).</span><span class="sxs-lookup"><span data-stu-id="dbbca-109">To understand which web part and configuration is right for you, see [Use a Yammer web part in SharePoint Online](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da).</span></span>  

<span data-ttu-id="dbbca-110">**Tīmekļa daļu izmantošana kopā ar SharePoint Server**</span><span class="sxs-lookup"><span data-stu-id="dbbca-110">**Using web parts with SharePoint Server**</span></span>  

<span data-ttu-id="dbbca-111">Tīmekļa daļas var izmantot modernās un klasiskās lapās lokālajā vidē.</span><span class="sxs-lookup"><span data-stu-id="dbbca-111">Web parts can be used in modern and classic pages within on-premises environments.</span></span>

- <span data-ttu-id="dbbca-112">Papildinformāciju par modernām lapām skatiet rakstā [Yammer plūsmas pievienošana mūsdienīgai SharePoint Server 2019 lapai](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-modern-page-in-sharepoint-server-2019).</span><span class="sxs-lookup"><span data-stu-id="dbbca-112">For more info about modern pages, see [Add a Yammer feed to a modern page in SharePoint Server 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-modern-page-in-sharepoint-server-2019).</span></span> 
- <span data-ttu-id="dbbca-113">Papildinformāciju par klasiskajām lapām skatiet rakstā [Yammer plūsmas pievienošana klasiskai lapai SharePoint serveros 2013, 2016 un 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-classic-page-in-sharepoint-servers-2013-2016-and-2019).</span><span class="sxs-lookup"><span data-stu-id="dbbca-113">For more info about classic pages, see [Add a Yammer feed to a classic page in SharePoint Servers 2013, 2016, and 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-classic-page-in-sharepoint-servers-2013-2016-and-2019).</span></span>

<span data-ttu-id="dbbca-114">**Yammer iegulšana**</span><span class="sxs-lookup"><span data-stu-id="dbbca-114">**Yammer Embed**</span></span>  

<span data-ttu-id="dbbca-115">Izmantojiet iegulšanas konfigurācijas rīku, lai testētu iegulšanas izmantošanu.</span><span class="sxs-lookup"><span data-stu-id="dbbca-115">Use the Embed Configuration tool to test Embed usage.</span></span> <span data-ttu-id="dbbca-116">Turpmākās iegulšanas atjauninājums ļaus izveidot jauno Yammer pieredzi.</span><span class="sxs-lookup"><span data-stu-id="dbbca-116">A future update to Embed will enable the new Yammer experience.</span></span> <span data-ttu-id="dbbca-117">Papildinformāciju skatiet rakstā [Yammer iegulšanas konfigurācijas rīks](https://aka.ms/YammerEmbedConfigureTool).</span><span class="sxs-lookup"><span data-stu-id="dbbca-117">For more info, see the [Yammer Embed Configuration tool](https://aka.ms/YammerEmbedConfigureTool).</span></span> <span data-ttu-id="dbbca-118">Lai labāk izprastu Yammer iegulšanas komponentu, skatiet rakstu [plūsmas iegulšana](https://aka.ms/YammerDevDocs).</span><span class="sxs-lookup"><span data-stu-id="dbbca-118">To better understand the Yammer Embed component, see [Embed Feed](https://aka.ms/YammerDevDocs).</span></span>

<span data-ttu-id="dbbca-119">**Zināmās problēmas un ierobežojumi**</span><span class="sxs-lookup"><span data-stu-id="dbbca-119">**Known issues and limitations**</span></span>

- <span data-ttu-id="dbbca-120">Grupas ID nav pieejami no jauniem Yammer vietrāžiem URL, kas ir mainījušies.</span><span class="sxs-lookup"><span data-stu-id="dbbca-120">Group IDs are not available from new Yammer URLs, which have changed.</span></span> <span data-ttu-id="dbbca-121">Pārslēdzieties atpakaļ uz klasisko režīmu, lai iegūtu grupas ID vai citus ID no vietrāžiem URL.</span><span class="sxs-lookup"><span data-stu-id="dbbca-121">Switch back to classic mode to obtain group IDs or other IDs from URLs.</span></span>
- <span data-ttu-id="dbbca-122">Pielāgoti (Vanity) domēni netiek atbalstīti.</span><span class="sxs-lookup"><span data-stu-id="dbbca-122">Custom (vanity) domains are not supported.</span></span>
- <span data-ttu-id="dbbca-123">Yammer iegulšana nav optimizēta mobilajai lietošanai.</span><span class="sxs-lookup"><span data-stu-id="dbbca-123">Yammer Embed is not optimized for mobile.</span></span> <span data-ttu-id="dbbca-124">Izmantojiet mūsdienīgas lapas ar Yammer sarunām tīmekļa daļā, lai iegūtu vislabāko pieredzi.</span><span class="sxs-lookup"><span data-stu-id="dbbca-124">Use modern pages with the Yammer Conversations web part for the best experience.</span></span>
- <span data-ttu-id="dbbca-125">Pielāgotie dizaini var ietekmēt Yammer sarunu tīmekļa daļu izskatu un lietojamību.</span><span class="sxs-lookup"><span data-stu-id="dbbca-125">Custom themes can affect the appearance and usability of the Yammer Conversations web part.</span></span> <span data-ttu-id="dbbca-126">Atveriet atbalsta gadījumu, lai ziņotu par problēmām.</span><span class="sxs-lookup"><span data-stu-id="dbbca-126">Open a support case to report issues.</span></span>