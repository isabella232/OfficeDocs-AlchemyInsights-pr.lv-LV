---
title: OneDrive darbam tīmekļa OneDrive novirzīšana uz Delve
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: 96f23585f7cbce672842f6330ba79816f24dbc41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51799996"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="ef495-102">Novirzīts uz Delve pēc noklikšķināšanas uz OneDrive</span><span class="sxs-lookup"><span data-stu-id="ef495-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="ef495-103">Skatiet mūsu detalizēto [problēmu novēršanas rokasgrāmatu.](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)</span><span class="sxs-lookup"><span data-stu-id="ef495-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="ef495-104">Lai novērstu šo problēmu, administratoram jāpiešķir lietotājiem tiesības izveidot savu vietņu Mana vietne.</span><span class="sxs-lookup"><span data-stu-id="ef495-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="ef495-105">Tas ir tāpēc, ka pakalpojuma OneDrive darbam lapa ir izveidota lapā Manas vietnes.</span><span class="sxs-lookup"><span data-stu-id="ef495-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="ef495-106">Lai piešķirtu šīs tiesības, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="ef495-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="ef495-107">SharePoint administrēšanas centrā noklikšķiniet uz lietotāju **profili.**</span><span class="sxs-lookup"><span data-stu-id="ef495-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="ef495-108">Sadaļā **Personas noklikšķiniet** uz Lietotāju **atļauju pārvaldība.**</span><span class="sxs-lookup"><span data-stu-id="ef495-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="ef495-109">Pievienojiet lietotājus, kuriem nepieciešamas atļaujas, lai izveidotu savu vietni Mana vietne.</span><span class="sxs-lookup"><span data-stu-id="ef495-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="ef495-110">Pēc noklusējuma šis iestatījums ir iestatīts uz **Ikviens, izņemot ārējos lietotājus.**</span><span class="sxs-lookup"><span data-stu-id="ef495-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="ef495-111">Pēc tam, kad esat pievienojis lietotāju, lietotājus vai grupu, pārliecinieties, vai ir  atlasīts pievienotais lietotājs, lietotāji vai grupa, ritiniet līdz atļauju sadaļai un pēc tam atzīmējiet izvēles rūtiņu pie Izveidot personisko vietni (nepieciešama personiskajai krātuvēm, jaunumu plūsmai un saturam, kam **sekojat).**</span><span class="sxs-lookup"><span data-stu-id="ef495-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="ef495-112">Noklikšķiniet **uz** Labi un pēc tam lū spiediet lietotāju, lai tas pārlūkojot atrastu OneDrive lapu un izveidotu vietni.</span><span class="sxs-lookup"><span data-stu-id="ef495-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
