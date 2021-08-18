---
title: Viesota balss pasta iespējošana
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 4042e042554f78febff2073fde6f14db72a6d4e0
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318655"
---
# <a name="how-to-enable-hosted-voicemail"></a>Viesota balss pasta iespējošana

Lai iespējotu balss pastu, **ir jābūt iestatītam HostedVoicemail** uz $true.

Rekvizīts **HostedVoicemail** lietotājam, kas izmanto Remote PowerShell (RPS).

Papildinformāciju par savienojuma izveidi ar RPS skatiet [rakstā Microsoft Teams PowerShell pārskats,](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) lai iegūtu papildinformāciju par savienojuma izveidi ar RPS.

1. Teams administratoram ir jāpiesakās Remote PowerShell Teams.
1. Izmantojot PowerShell, Teams administrators var palaist **set-csuser user@contoso.com -HostedVoiceMail $true,** kur attiecīgā lietotāja sip uri ir.

**Piezīme.** Var paiet līdz pat 24 stundām, līdz politiku izmaiņas tiks kopētas.