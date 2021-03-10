---
title: Transporta kārtulu labošana
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
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694155"
---
# <a name="fix-transport-rules"></a><span data-ttu-id="680c6-102">Transporta kārtulu labošana</span><span class="sxs-lookup"><span data-stu-id="680c6-102">Fix transport rules</span></span>

<span data-ttu-id="680c6-103">Šis ziņojums ietekmēja pielāgotu pasta plūsmas kārtulu.</span><span class="sxs-lookup"><span data-stu-id="680c6-103">A custom mail flow rule affected this message.</span></span> <span data-ttu-id="680c6-104">Lai pārskatītu precīzu kārtulu, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="680c6-104">To review the exact rule, do the following:</span></span>

1. <span data-ttu-id="680c6-105">Iesniegšanas rezultātu sadaļā **Papildinformācija** pievērsiet uzmanību **GUID** vai **politikas nosaukumam**.</span><span class="sxs-lookup"><span data-stu-id="680c6-105">In the submission results, under **Additional information**, note the **GUID** or the **Policy Name**.</span></span>
2. <span data-ttu-id="680c6-106">Palaidiet Exchange pārvaldības čaulu.</span><span class="sxs-lookup"><span data-stu-id="680c6-106">Launch Exchange Management Shell.</span></span> <span data-ttu-id="680c6-107">Papildinformāciju skatiet rakstā [Exchange pārvaldības čaulas atvēršana](https://go.microsoft.com/fwlink/?linkid=2101432).</span><span class="sxs-lookup"><span data-stu-id="680c6-107">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
3. <span data-ttu-id="680c6-108">Izpildīt šo komandu (izmantojot jūsu iesniegto GUID):  **Get-TransportRule-Identity "GUID" | FL \* apraksts**\*</span><span class="sxs-lookup"><span data-stu-id="680c6-108">Run this command (using the GUID from your submission):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span></span>
4. <span data-ttu-id="680c6-109">Pārskatiet aprakstu, lai redzētu konfigurētos nosacījumus, kas ietekmēja ziņojumu.</span><span class="sxs-lookup"><span data-stu-id="680c6-109">Review the description to see the configured conditions that affected the message.</span></span>

<span data-ttu-id="680c6-110">Papildinformāciju skatiet rakstā [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span><span class="sxs-lookup"><span data-stu-id="680c6-110">To learn more, see [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span></span>
