---
title: 1:1 izsaukumu ierakstīšana
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
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733856"
---
# <a name="11-call-recording"></a><span data-ttu-id="65bce-102">1:1 izsaukumu ierakstīšana</span><span class="sxs-lookup"><span data-stu-id="65bce-102">1:1 call recording</span></span>

<span data-ttu-id="65bce-103">Administratoriem ir jāveic darbības tūlīt, lai turpinātu atļaut lietotājiem ierakstīt 1:1 zvanus.</span><span class="sxs-lookup"><span data-stu-id="65bce-103">Administrators need to take action now to continue allowing users to Record 1:1 calls.</span></span>
 
<span data-ttu-id="65bce-104">Sākot ar 12. aprīli, 2021, mēs sāksim īstenot jaunu grupu zvana politikas opciju *AllowCloudRecordingForCalls*.</span><span class="sxs-lookup"><span data-stu-id="65bce-104">Beginning April 12, 2021, we will start enforcing a new Teams Calling Policy option *AllowCloudRecordingForCalls*.</span></span> 

<span data-ttu-id="65bce-105">Pašlaik 1:1 izsaukumu ierakstīšanas iespējas kontrolē *AllowCloudRecording* opcija grupu sapulču politikās.</span><span class="sxs-lookup"><span data-stu-id="65bce-105">Currently 1:1 call recording capabilities are controlled by the *AllowCloudRecording* option in Teams Meeting Policies.</span></span> <span data-ttu-id="65bce-106">Ja lietotājiem ir atļauts ierakstīt grupu sapulces, tās var arī ierakstīt 1:1 zvanus.</span><span class="sxs-lookup"><span data-stu-id="65bce-106">If your users are allowed to record Teams Meetings they can also record 1:1 calls.</span></span>

<span data-ttu-id="65bce-107">Ja vēlaties bloķēt visu lietotāju ierakstīšanu 1:1 zvaniem, jums nav jāveic nekādas darbības.</span><span class="sxs-lookup"><span data-stu-id="65bce-107">If you prefer to block all users from recording 1:1 calls, you do not need to take any action.</span></span> <span data-ttu-id="65bce-108">*AllowCloudRecordingForCalls* zvanīšanas politikas opcija tiks $FALSE pēc noklusējuma.</span><span class="sxs-lookup"><span data-stu-id="65bce-108">*AllowCloudRecordingForCalls* calling policy option will be $False by default.</span></span>

<span data-ttu-id="65bce-109">Šīs izmaiņas ir dokumentētas tālāk redzamajā ziņojumu centra izrakstā: [(atjaunināts) 1:1 zvana ieraksta politikas Ievads](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) par grupu zvanīšanas politikas opcijas iestatīšanu, izmantojot [komandu PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="65bce-109">This change is documented in the following Message Center Post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) To set the Teams Calling Policy Option you must use [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span></span>

<span data-ttu-id="65bce-110">**Lai iespējotu zvanu ierakstīšanu 1:1** zvanos: Set-CsTeamsCallingPolicy-Identity Global-AllowCloudRecordingForCalls $TRUE</span><span class="sxs-lookup"><span data-stu-id="65bce-110">**To enable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span></span>

<span data-ttu-id="65bce-111">**Lai atspējotu zvanu ierakstīšanu 1:1** zvanos: Set-CsTeamsCallingPolicy-Identity Global-AllowCloudRecordingForCalls $FALSE</span><span class="sxs-lookup"><span data-stu-id="65bce-111">**To disable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span></span>

