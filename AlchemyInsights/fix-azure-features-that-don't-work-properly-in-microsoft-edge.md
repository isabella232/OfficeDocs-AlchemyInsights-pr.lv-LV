---
title: Kā rīkoties, ja Azure līdzekļi nedarbojas pareizi pārlūkprogrammā Microsoft Edge
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583458"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a><span data-ttu-id="93d69-102">Kā rīkoties, ja Azure līdzekļi nedarbojas pareizi pārlūkprogrammā Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="93d69-102">What to do if Azure features don't work properly in Microsoft Edge</span></span>

<span data-ttu-id="93d69-103">Pārlūkprogrammā Microsoft Edge ir [zināmās problēmas](https://go.microsoft.com/fwlink/?linkid=2140608) , kas saistītas ar drošības zonām, un tās var ietekmēt to, kā Azure lietotāji piesakās Windows administrēšanas centrā.</span><span class="sxs-lookup"><span data-stu-id="93d69-103">Microsoft Edge has [known issues](https://go.microsoft.com/fwlink/?linkid=2140608) that are related to security zones and might affect how Azure users log in to Windows Admin Center.</span></span> <span data-ttu-id="93d69-104">Ja rodas problēmas ar Azure līdzekļu lietošanu, izmantojot Microsoft Edge, izmēģiniet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="93d69-104">If you're having trouble using Azure features with Microsoft Edge, try the following steps:</span></span>

1. <span data-ttu-id="93d69-105">**Sākuma** izvēlnē meklējiet **interneta opcijas** un atlasiet to.</span><span class="sxs-lookup"><span data-stu-id="93d69-105">In the **Start** menu, search for **Internet Options** and select it.</span></span>
2. <span data-ttu-id="93d69-106">Dialoglodziņā **Interneta rekvizīti** dodieties uz cilni **Drošība** .</span><span class="sxs-lookup"><span data-stu-id="93d69-106">In the **Internet Properties** dialog box, go to the **Security** tab.</span></span>
3. <span data-ttu-id="93d69-107">Atlasiet **uzticamo vietņu** zonu un pēc tam atlasiet pogu **vietnes** .</span><span class="sxs-lookup"><span data-stu-id="93d69-107">Select the **Trusted sites** zone and then select the **Sites** button.</span></span>
4. <span data-ttu-id="93d69-108">Dialoglodziņā **uzticamās vietnes** pievienojiet vārtejas vietrādi URL, kā arī [https://login.microsoftonline.com](https://login.microsoftonline.com) un [https://login.live.com](https://login.live.com) pēc tam atlasiet **aizvērts**.</span><span class="sxs-lookup"><span data-stu-id="93d69-108">In the **Trusted sites** dialog box, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
5. <span data-ttu-id="93d69-109">Dialoglodziņā **Interneta rekvizīti** dodieties uz cilni **Konfidencialitāte** .</span><span class="sxs-lookup"><span data-stu-id="93d69-109">In the **Internet Properties** dialog box, go to the **Privacy** tab.</span></span>
6. <span data-ttu-id="93d69-110">**Uznirstošo logu bloķētāja** sadaļā atlasiet **Iestatījumi**.</span><span class="sxs-lookup"><span data-stu-id="93d69-110">In the **Pop-up Blocker** section, select **Settings**.</span></span> <span data-ttu-id="93d69-111">Dialoglodziņā, kas tiek atvērts, pievienojiet vārtejas vietrādi URL, kā arī [https://login.microsoftonline.com](https://login.microsoftonline.com) un [https://login.live.com](https://login.live.com) pēc tam atlasiet **aizvērts**.</span><span class="sxs-lookup"><span data-stu-id="93d69-111">In the dialog box that opens, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
