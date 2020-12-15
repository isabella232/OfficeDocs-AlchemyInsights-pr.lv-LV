---
title: Pakalpojuma diagnostikas rīks Windows virtuālajai darbvirsmai
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/14/2020
ms.locfileid: "49678624"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="89061-102">Pakalpojuma diagnostikas rīks Windows virtuālajai darbvirsmai</span><span class="sxs-lookup"><span data-stu-id="89061-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="89061-103">Windows virtuālā darbvirsma (WVD) piedāvā diagnostikas rīku, kas administratoriem ļauj noteikt kļūdas, izmantojot vienu interfeisu.</span><span class="sxs-lookup"><span data-stu-id="89061-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="89061-104">Šis rīks reģistrē diagnostiku ar diagnostikas informāciju, kad WVD izmanto kāds, kam ir piešķirta WVD loma.</span><span class="sxs-lookup"><span data-stu-id="89061-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="89061-105">Katrā žurnālfailā ir iekļauta informācija par aktivitāti iesaistīto WVD lomu, kļūdu ziņojumi, kas tiek parādīti sesijas laikā, kā arī informācija par nomnieku un lietotāju.</span><span class="sxs-lookup"><span data-stu-id="89061-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="89061-106">Azure LG Analytics var konfigurēt, lai tvertu diagnostikas rīka izveidoto darbību žurnālu.</span><span class="sxs-lookup"><span data-stu-id="89061-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool.</span></span> <span data-ttu-id="89061-107">Tālāk aprakstīts, kā to paveikt.</span><span class="sxs-lookup"><span data-stu-id="89061-107">Here's how:</span></span>

1. <span data-ttu-id="89061-108">Izveidojiet žurnālu analīzes darbvietu ar [Azure portālu](https://go.microsoft.com/fwlink/?linkid=2129500) vai [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span><span class="sxs-lookup"><span data-stu-id="89061-108">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>
1. <span data-ttu-id="89061-109">[Windows datoru savienošana ar Azure monitoru](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="89061-109">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="89061-110">Iegūstiet darbvietas ID un darbvietas primāro atslēgu.</span><span class="sxs-lookup"><span data-stu-id="89061-110">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="89061-111">Iestatīšanas vednim ir nepieciešama šī informācija, lai pareizi konfigurētu aģentu un nodrošinātu, ka tas var sazināties ar Azure monitoru.</span><span class="sxs-lookup"><span data-stu-id="89061-111">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>
1. <span data-ttu-id="89061-112">[Stumiet diagnostikas datus darbvietā](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="89061-112">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="89061-113">Varat push diagnostikas datus no sava WVD nomnieka uz savas darbvietas žurnālu analīzi.</span><span class="sxs-lookup"><span data-stu-id="89061-113">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>
1. <span data-ttu-id="89061-114">[Identificējiet un diagnosticējiet problēmas](https://go.microsoft.com/fwlink/?linkid=2128338) , kas ir iekšējas vai ārējas saistībā ar WVD.</span><span class="sxs-lookup"><span data-stu-id="89061-114">[Identify and diagnose issues](https://go.microsoft.com/fwlink/?linkid=2128338) that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="89061-115">Lai uzzinātu vairāk par pakalpojumu diagnostikas rīka konfigurēšanu programmai WVD, skatiet rakstu [diagnostikas līdzekļa žurnālu analīzes lietošana](https://go.microsoft.com/fwlink/?linkid=2128084).</span><span class="sxs-lookup"><span data-stu-id="89061-115">To learn more about configuring the service diagnostics tool for WVD, see [Use Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2128084).</span></span>
