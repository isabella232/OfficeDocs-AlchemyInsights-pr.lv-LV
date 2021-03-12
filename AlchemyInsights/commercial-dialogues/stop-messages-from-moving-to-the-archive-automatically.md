---
title: Ziņojumu automātiska pārvietošana uz arhīvu
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 2cb3e29dfd4f422e946b7887d4d44f373ff03794
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746328"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a><span data-ttu-id="e9bc2-102">Ziņojumu automātiska pārvietošana uz arhīvu</span><span class="sxs-lookup"><span data-stu-id="e9bc2-102">Stop messages from moving to the archive automatically</span></span>

<span data-ttu-id="e9bc2-103">Ja izmantojat saglabāšanas politiku, varat mainīt saglabāšanas vecumu attiecīgajā politikā, lai pārtrauktu automātisku ziņojumu arhivēšanu.</span><span class="sxs-lookup"><span data-stu-id="e9bc2-103">If you are using a retention policy, you can change the retention age in that policy to stop messages from archiving automatically.</span></span> <span data-ttu-id="e9bc2-104">Tālāk aprakstīts, kā to paveikt.</span><span class="sxs-lookup"><span data-stu-id="e9bc2-104">Here's how:</span></span>

1. <span data-ttu-id="e9bc2-105">[Exchange administrēšanas centrā](https://go.microsoft.com/fwlink/?linkid=2059104)izvēlieties **atbilstības pārvaldības**  >  **saglabāšanas atzīmes**.</span><span class="sxs-lookup"><span data-stu-id="e9bc2-105">In the [Exchange admin center](https://go.microsoft.com/fwlink/?linkid=2059104), choose **compliance management** > **retention tags**.</span></span> <span data-ttu-id="e9bc2-106">Atrodiet savu pārvietot uz arhīva saglabāšanas atzīmi.</span><span class="sxs-lookup"><span data-stu-id="e9bc2-106">Locate your Move to Archive retention tag.</span></span>
2. <span data-ttu-id="e9bc2-107">Saglabāšanas tagā mainiet saglabāšanas periodu (arhīva periodu) **, lai neļautu** automātiski arhivēt vienumus, izmantojot saglabāšanas politiku.</span><span class="sxs-lookup"><span data-stu-id="e9bc2-107">In the retention tag, change the retention period (archive period) to **Never** to stop items from being automatically archived by a retention policy.</span></span>

> [!NOTE]
> <span data-ttu-id="e9bc2-108">Tas mainīs arhivēšanas iestatījumu visām pastkastēm, kurām ir lietots šis saglabāšanas Tags.</span><span class="sxs-lookup"><span data-stu-id="e9bc2-108">This will change the archive setting for all mailboxes with this retention tag applied to them.</span></span>
