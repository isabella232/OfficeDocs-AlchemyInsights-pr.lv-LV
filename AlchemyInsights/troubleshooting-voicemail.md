---
title: 'Balss pasta problēmu novēršana '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7564"
ms.openlocfilehash: a2d26da512838ae112c352fe21366074b69fa224
ms.sourcegitcommit: 3802f2f4db4f53a408a360187db67f2296448c21
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/09/2020
ms.locfileid: "49677966"
---
# <a name="troubleshooting-voicemail"></a><span data-ttu-id="e137d-102">Balss pasta problēmu novēršana</span><span class="sxs-lookup"><span data-stu-id="e137d-102">Troubleshooting Voicemail</span></span>

<span data-ttu-id="e137d-103">Nodrošiniet, lai aizņemtības līdzeklis būtu ar nodomu.</span><span class="sxs-lookup"><span data-stu-id="e137d-103">Ensure that the Busy on Busy feature is intentional.</span></span>

<span data-ttu-id="e137d-104">Ja šis līdzeklis nav nepieciešams šim lietotājam:</span><span class="sxs-lookup"><span data-stu-id="e137d-104">If this feature is not needed on this user:</span></span>

1. <span data-ttu-id="e137d-105">Dodieties uz [Teams administrēšanas centru](https://admin.teams.microsoft.com/policies/calling).</span><span class="sxs-lookup"><span data-stu-id="e137d-105">Go to [Teams Admin center](https://admin.teams.microsoft.com/policies/calling).</span></span>
1. <span data-ttu-id="e137d-106">Kreisās puses navigācijas joslā **balss**  >  **zvanu politika**  >  **pārvalda** **zvanīšanas politikas** politikas.</span><span class="sxs-lookup"><span data-stu-id="e137d-106">On the left rail navigate **Voice** > **Calling policies** > **Manage Policies** on the **Calling Policy**.</span></span>
1. <span data-ttu-id="e137d-107">Atlasiet **lietotāju pārvaldība**.</span><span class="sxs-lookup"><span data-stu-id="e137d-107">Select **Manage Users**.</span></span>
1. <span data-ttu-id="e137d-108">Meklējiet lietotāju un mainiet zvanīšanas politiku uz tādu, kas ir aizņemta ar **aizņemts, ir pieejams, kad zvana** uz **izslēgts**.</span><span class="sxs-lookup"><span data-stu-id="e137d-108">Search for user and change the Calling Policy to one that has **Busy on Busy is available when in a call** to **Off**.</span></span>
1. <span data-ttu-id="e137d-109">Noklikšķiniet uz **Lietot**.</span><span class="sxs-lookup"><span data-stu-id="e137d-109">Click **Apply**.</span></span>
> [!NOTE]
> <span data-ttu-id="e137d-110">Politikas izmaiņas var ilgt līdz pat 24 stundām.</span><span class="sxs-lookup"><span data-stu-id="e137d-110">Changes to policies can take up to 24 hours to replicate.</span></span>

<span data-ttu-id="e137d-111">Lai iegūtu papildinformāciju par šo līdzekli, skatiet tēmu: [aizņemts ar aizņemts ir pieejams sarunas laikā](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span><span class="sxs-lookup"><span data-stu-id="e137d-111">For more information on this feature refer to: [Busy on Busy is available while in a call](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span></span>
