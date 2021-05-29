---
title: 1:1 zvanu ierakstīšana
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: 8cdadf34a059856338d7f40528446b70373465e4
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702097"
---
# <a name="11-call-recording"></a><span data-ttu-id="30cd4-102">1:1 zvanu ierakstīšana</span><span class="sxs-lookup"><span data-stu-id="30cd4-102">1:1 call recording</span></span>

<span data-ttu-id="30cd4-103">Ja poga **Sākt ierakstīšanu** 1:1 zvanā ir pelēkota, ir jāmaina ietekmētā lietotāja politikas iestatījumi.</span><span class="sxs-lookup"><span data-stu-id="30cd4-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span> <span data-ttu-id="30cd4-104">Lai pārbaudītu politikas iestatījumu, palaidiet diagnostiku ietekmētā lietotājam, ierakstot **Diag: Teams 1:1 Zvana** ierakstīšana.</span><span class="sxs-lookup"><span data-stu-id="30cd4-104">To check the policy setting, run the Diagnostic for the impacted user by typing **Diag: Teams 1:1 Call Recording** above.</span></span>     

<span data-ttu-id="30cd4-105">Sākot ar 2021. gada 31. maiju, sāksim ieviest jaunu zvanīšanas Teams *AllowCloudRecordingForCalls*.</span><span class="sxs-lookup"><span data-stu-id="30cd4-105">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="30cd4-106">Pirms šo izmaiņu 1:1 zvana ierakstu kontrolē *AllowCloudRecording* Teams sapulces politika.</span><span class="sxs-lookup"><span data-stu-id="30cd4-106">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="30cd4-107">Šīs izmaiņas ir dokumentētas ziņojumu centra ziņā: [(Atjaunināts) 1:1 Zvanu ierakstīšanas politikas ievads.](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)</span><span class="sxs-lookup"><span data-stu-id="30cd4-107">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="30cd4-108">*AllowCloudRecordingForCalls*   zvanu politikas opcija pēc **$False** ir iestatīta.</span><span class="sxs-lookup"><span data-stu-id="30cd4-108">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="30cd4-109">Ja vēlaties visiem lietotājiem bloķēt 1:1 zvanu ierakstīšanu, jums nav jāveic nekādas darbības.</span><span class="sxs-lookup"><span data-stu-id="30cd4-109">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="30cd4-110">Lai iespējotu zvanu ierakstīšanu visiem lietotājiem 1:1 zvanos, izmantojiet [Teams PowerShell,](/microsoftteams/teams-powershell-install) lai izpildītu šādu cmdlet komandu:</span><span class="sxs-lookup"><span data-stu-id="30cd4-110">To enable call recording for all users in 1:1 calls use [Teams PowerShell](/microsoftteams/teams-powershell-install) to run the following cmdlet:</span></span> 

<span data-ttu-id="30cd4-111">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="30cd4-111">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="30cd4-112">Vai arī varat izveidot jaunu politiku un iestatīt **failu -AllowCloudRecordingForCalls** **$true** piešķirt šo politiku saviem lietotājiem.</span><span class="sxs-lookup"><span data-stu-id="30cd4-112">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="30cd4-113">Papildinformāciju skatiet rakstā Zvana ierakstīšanas politikas vadīklas [1:1 (gandrīz!) Šeit.](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668)</span><span class="sxs-lookup"><span data-stu-id="30cd4-113">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>
