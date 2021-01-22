---
title: NDI tehnoloģijas ieslēgšana
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
ms.openlocfilehash: ea694898baffa50fca71957175eba3664dece44e
ms.sourcegitcommit: 112f18dce8257b98fab32d44910ee879efb44cb8
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935131"
---
# <a name="turn-on-ndi-technology"></a>NDI tehnoloģijas ieslēgšana

NDI tehnoloģijai lietotājam ir jāveic divas darbības:

1. Nomnieka administratoram ir jāiespējo rekvizīts "AllowNDIStreaming" programmā CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Pēc tam, kad šīs izmaiņas ir apdzīvotas, lietotājam ir jāieslēdz NDI® tehnoloģijas konkrētajam klientam no **iestatījumiem > atļaujām**.

Papildinformāciju skatiet rakstā [NDI tehnoloģijas izmantošana pakalpojumā Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).
