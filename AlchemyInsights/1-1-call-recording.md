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
# <a name="11-call-recording"></a>1:1 zvanu ierakstīšana

Ja poga **Sākt ierakstīšanu** 1:1 zvanā ir pelēkota, ir jāmaina ietekmētā lietotāja politikas iestatījumi. Lai pārbaudītu politikas iestatījumu, palaidiet diagnostiku ietekmētā lietotājam, ierakstot **Diag: Teams 1:1 Zvana** ierakstīšana.     

Sākot ar 2021. gada 31. maiju, sāksim ieviest jaunu zvanīšanas Teams *AllowCloudRecordingForCalls*. Pirms šo izmaiņu 1:1 zvana ierakstu kontrolē *AllowCloudRecording* Teams sapulces politika. Šīs izmaiņas ir dokumentētas ziņojumu centra ziņā: [(Atjaunināts) 1:1 Zvanu ierakstīšanas politikas ievads.](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)  

*AllowCloudRecordingForCalls*   zvanu politikas opcija pēc **$False** ir iestatīta. Ja vēlaties visiem lietotājiem bloķēt 1:1 zvanu ierakstīšanu, jums nav jāveic nekādas darbības.  

Lai iespējotu zvanu ierakstīšanu visiem lietotājiem 1:1 zvanos, izmantojiet [Teams PowerShell,](/microsoftteams/teams-powershell-install) lai izpildītu šādu cmdlet komandu: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Vai arī varat izveidot jaunu politiku un iestatīt **failu -AllowCloudRecordingForCalls** **$true** piešķirt šo politiku saviem lietotājiem. 

Papildinformāciju skatiet rakstā Zvana ierakstīšanas politikas vadīklas [1:1 (gandrīz!) Šeit.](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668)
