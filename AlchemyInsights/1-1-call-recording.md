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
# <a name="11-call-recording"></a>1:1 izsaukumu ierakstīšana

Administratoriem ir jāveic darbības tūlīt, lai turpinātu atļaut lietotājiem ierakstīt 1:1 zvanus.
 
Sākot ar 12. aprīli, 2021, mēs sāksim īstenot jaunu grupu zvana politikas opciju *AllowCloudRecordingForCalls*. 

Pašlaik 1:1 izsaukumu ierakstīšanas iespējas kontrolē *AllowCloudRecording* opcija grupu sapulču politikās. Ja lietotājiem ir atļauts ierakstīt grupu sapulces, tās var arī ierakstīt 1:1 zvanus.

Ja vēlaties bloķēt visu lietotāju ierakstīšanu 1:1 zvaniem, jums nav jāveic nekādas darbības. *AllowCloudRecordingForCalls* zvanīšanas politikas opcija tiks $FALSE pēc noklusējuma.

Šīs izmaiņas ir dokumentētas tālāk redzamajā ziņojumu centra izrakstā: [(atjaunināts) 1:1 zvana ieraksta politikas Ievads](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) par grupu zvanīšanas politikas opcijas iestatīšanu, izmantojot [komandu PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).

**Lai iespējotu zvanu ierakstīšanu 1:1** zvanos: Set-CsTeamsCallingPolicy-Identity Global-AllowCloudRecordingForCalls $TRUE

**Lai atspējotu zvanu ierakstīšanu 1:1** zvanos: Set-CsTeamsCallingPolicy-Identity Global-AllowCloudRecordingForCalls $FALSE

