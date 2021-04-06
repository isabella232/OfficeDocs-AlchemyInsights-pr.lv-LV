---
title: Pakalpojumu diagnostikas rīks Windows virtuālajai darbvirsmai
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595867"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="d8af8-102">Pakalpojumu diagnostikas rīks Windows virtuālajai darbvirsmai</span><span class="sxs-lookup"><span data-stu-id="d8af8-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="d8af8-103">Windows virtuālā darbvirsma (Windows Virtual Desktop — WVD) piedāvā diagnostikas rīku, kas administratoriem ļauj identificēt kļūdas, izmantojot vienu interfeisu.</span><span class="sxs-lookup"><span data-stu-id="d8af8-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="d8af8-104">Šis rīks reģistrē ar diagnostiku saistītu informāciju ikreiz, kad WVD izmanto kāds lietotājs, kuram piešķirta WVD loma.</span><span class="sxs-lookup"><span data-stu-id="d8af8-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="d8af8-105">Katrā žurnālā ir iekļauta informācija par darbībā iesaistīto WVD lomu, sesijas laikā parādītajiem kļūdu ziņojumiem un informāciju par nomnieku un lietotāju.</span><span class="sxs-lookup"><span data-stu-id="d8af8-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="d8af8-106">Azure Log Analytics var konfigurēt, lai tvertu diagnostikas rīka izveidoto darbību žurnālu, izpildot šīs darbības:</span><span class="sxs-lookup"><span data-stu-id="d8af8-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool by following these steps:</span></span>

1. <span data-ttu-id="d8af8-107">Izveidojiet Log Analytics darbvietu [Azure portālā vai](https://go.microsoft.com/fwlink/?linkid=2129500) [pakalpojumā Azure PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)</span><span class="sxs-lookup"><span data-stu-id="d8af8-107">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>

1. <span data-ttu-id="d8af8-108">[Windows datoru savienošana ar Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="d8af8-108">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="d8af8-109">Iegūstiet darbvietas ID un darbvietas primāro atslēgu.</span><span class="sxs-lookup"><span data-stu-id="d8af8-109">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="d8af8-110">Iestatīšanas vednim ir nepieciešama šī informācija, lai pareizi konfigurētu aģentu un nodrošinātu, ka tas var sazināties ar Azure Monitor.</span><span class="sxs-lookup"><span data-stu-id="d8af8-110">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>

1. <span data-ttu-id="d8af8-111">[Pašpiegādes diagnostika datus uz jūsu darbvietu.](https://go.microsoft.com/fwlink/?linkid=2128284)</span><span class="sxs-lookup"><span data-stu-id="d8af8-111">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="d8af8-112">Varat pašpiegādes diagnostikas datus no sava WVD nomnieka uz darbvietas žurnālu analīzi.</span><span class="sxs-lookup"><span data-stu-id="d8af8-112">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>

1. <span data-ttu-id="d8af8-113">[Identificējiet un diagnosticējiet](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) problēmas, kas ir iekšējas vai ārējas attiecībā pret WVD.</span><span class="sxs-lookup"><span data-stu-id="d8af8-113">[Identify and diagnose](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) issues that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="d8af8-114">Lai uzzinātu vairāk par pakalpojumu diagnostikas rīka konfigurēšanu WVD, skatiet rakstu Log Analytics izmantošana diagnostikas līdzeklim.</span><span class="sxs-lookup"><span data-stu-id="d8af8-114">To learn more about configuring the service diagnostics tool for WVD, see Use Log Analytics for the diagnostics feature.</span></span>