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
ms.openlocfilehash: 4d70e92a7c1bf8f3cc62d4a310aa140ee2dfdef4c798ae17faa961736d9db500
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055561"
---
# <a name="how-to-enable-hosted-voicemail"></a>Viesota balss pasta iespējošana

Lai iespējotu balss pastu, **ir jābūt iestatītam HostedVoicemail** uz $true.

Rekvizīts **HostedVoicemail** lietotājam, kas izmanto Remote PowerShell (RPS).

Papildinformāciju par savienojuma izveidi ar RPS skatiet [rakstā Microsoft Teams PowerShell pārskats,](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) lai iegūtu papildinformāciju par savienojuma izveidi ar RPS.

1. Teams administrēšanai ir jāpiesakās Remote PowerShell Teams.
1. Izmantojot PowerShell, Teams administrators var palaist **set-csuser user@contoso.com -HostedVoiceMail $true,** kur attiecīgā lietotāja sip uri ir.

> [!NOTE]
> Var paiet līdz pat 24 stundām, līdz politiku izmaiņas tiks kopētas.