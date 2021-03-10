---
title: Offboard, kas nav Windows ierīces, no Microsoft Defender Advanced Threat Protection (ATP)
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
- "9000760"
- "7391"
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693817"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a><span data-ttu-id="dfc25-102">Offboard, kas nav Windows ierīces, no Microsoft Defender Advanced Threat Protection (ATP)</span><span class="sxs-lookup"><span data-stu-id="dfc25-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span></span>

<span data-ttu-id="dfc25-103">Tālāk aprakstīts, kā to paveikt.</span><span class="sxs-lookup"><span data-stu-id="dfc25-103">Here's how:</span></span>

1. <span data-ttu-id="dfc25-104">Izpildiet trešo pušu dokumentāciju, lai atvienotu trešo personu risinājumu no Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="dfc25-104">Follow the third-party documentation for disconnecting the third-party solution from Microsoft Defender ATP.</span></span>
2. <span data-ttu-id="dfc25-105">Azure Active Directory nomniekā noņemiet trešo pušu risinājuma atļaujas:</span><span class="sxs-lookup"><span data-stu-id="dfc25-105">From your Azure Active Directory tenant, remove permissions for the third-party solution:</span></span>

    1. <span data-ttu-id="dfc25-106">Pierakstieties [Azure portālā](https://go.microsoft.com/fwlink/?linkid=2125612).</span><span class="sxs-lookup"><span data-stu-id="dfc25-106">Sign in to the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span></span>
    1. <span data-ttu-id="dfc25-107">Atlasiet **visas pakalpojumu**  >  **Azure Active Directory**  >  **uzņēmuma lietojumprogrammas**.</span><span class="sxs-lookup"><span data-stu-id="dfc25-107">Select **All services** > **Azure Active Directory** > **Enterprise Applications**.</span></span>
    1. <span data-ttu-id="dfc25-108">Atlasiet lietojumprogrammu, kuru vēlaties offboard.</span><span class="sxs-lookup"><span data-stu-id="dfc25-108">Select the application you'd like to offboard.</span></span>
    1. <span data-ttu-id="dfc25-109">Atlasiet **Dzēst**.</span><span class="sxs-lookup"><span data-stu-id="dfc25-109">Select **Delete**.</span></span>

<span data-ttu-id="dfc25-110">Lai uzzinātu vairāk, skatiet rakstu [offboard, kas nav Windows ierīces](https://go.microsoft.com/fwlink/?linkid=2143630).</span><span class="sxs-lookup"><span data-stu-id="dfc25-110">To learn more, see [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span></span>
