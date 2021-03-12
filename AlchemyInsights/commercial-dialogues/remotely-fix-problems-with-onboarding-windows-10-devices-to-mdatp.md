---
title: Attālas problēmu novēršana saistībā ar Windows 10 ierīcēm, izmantojot Microsoft Defender Advanced Threat Protection
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
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746451"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a><span data-ttu-id="b41d4-102">Attālas problēmu novēršana saistībā ar Windows 10 ierīcēm, izmantojot Microsoft Defender Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="b41d4-102">Remotely fix problems with onboarding Windows 10 devices to Microsoft Defender Advanced Threat Protection</span></span>

<span data-ttu-id="b41d4-103">Ja varat piekļūt attālajam datoram, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="b41d4-103">If you can access the remote computer, follow these steps:</span></span>

1. <span data-ttu-id="b41d4-104">Lejupielādējiet [klientu savienojamības analīzes](https://go.microsoft.com/fwlink/?linkid=2143466) diagnostikas rīku.</span><span class="sxs-lookup"><span data-stu-id="b41d4-104">Download the [Client Connectivity Analyzer](https://go.microsoft.com/fwlink/?linkid=2143466) diagnostic tool.</span></span>
2. <span data-ttu-id="b41d4-105">Izvilkt un palaist MDATPAnalyzer. cmd.</span><span class="sxs-lookup"><span data-stu-id="b41d4-105">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="b41d4-106">Atrodiet diagnostikas žurnālu mapē MDATPClientAnalyzerResult, kas ir tajā pašā mapē, kurā tika lejupielādēts analīzes rīks.</span><span class="sxs-lookup"><span data-stu-id="b41d4-106">Locate the diagnostic log in the MDATPClientAnalyzerResult folder, which is the same folder where the Analyzer tool was downloaded.</span></span>
4. <span data-ttu-id="b41d4-107">Lai atrastu problēmas ar savienojamības vai interneta starpniekservera iestatījumiem, pārskatiet žurnālfailu MDATPClientAnalyzer.txt.</span><span class="sxs-lookup"><span data-stu-id="b41d4-107">To find issues with connectivity or Internet proxy settings, review the log file MDATPClientAnalyzer.txt.</span></span>

<span data-ttu-id="b41d4-108">Lai uzzinātu vairāk, skatiet rakstu [problēmas ar borta datoriem](https://go.microsoft.com/fwlink/?linkid=2143634).</span><span class="sxs-lookup"><span data-stu-id="b41d4-108">To learn more, see [Issues with onboarding machines](https://go.microsoft.com/fwlink/?linkid=2143634).</span></span>
