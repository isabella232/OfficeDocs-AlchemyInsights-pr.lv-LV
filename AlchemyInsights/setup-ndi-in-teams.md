---
title: Ieslēgt NDI tehnoloģiju
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
- "9004403"
- "7947"
ms.openlocfilehash: ed932592aae1158bc0c0da4817467b69d20208533bc080cb0e424f552af8601a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54023529"
---
# <a name="turn-on-ndi-technology"></a>Ieslēgt NDI tehnoloģiju

Lai lietotājam ieslēgtu NDI tehnoloģiju, ir jāveic divas darbības:

1. Nomnieka administratoram ir jāiespējo rekvizīts "AllowNDIStreaming" CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Kad šīs izmaiņas ir aizpildītas, lietotājam ir jāieslēdz NDI® tehnoloģija konkrētam klientam, izmantojot **Iestatījumi > atļaujas.**

Papildinformāciju skatiet rakstā [NDI tehnoloģijas izmantošana Microsoft Teams.](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)
