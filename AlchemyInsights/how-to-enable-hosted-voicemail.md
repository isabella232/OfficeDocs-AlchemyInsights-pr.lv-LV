---
title: Viesotā balss pasta iespējošana
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
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/09/2020
ms.locfileid: "49677997"
---
# <a name="how-to-enable-hosted-voicemail"></a>Viesotā balss pasta iespējošana

Lai iespējotu balss pastu, **HostedVoicemail** ir jābūt iestatītai uz $True.

Rekvizīts **HostedVoicemail** lietotājam, kas izmanto attālo POWERSHELL (RPS).

Lai iegūtu papildinformāciju par savienojuma izveidi ar RPS, skatiet rakstu [Microsoft Teams PowerShell pārskats](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) , lai iegūtu papildinformāciju par savienojuma izveidi ar RPS.

1. Teams administratoram ir jāpiesakās attālajā PowerShell darbam ar Teams.
1. No PowerShell uzvednes Teams administrators var palaist **Set-csuser user@contoso.com-HostedVoiceMail $True** , kur SIP URI ir lietotāja jautājums.

> [!NOTE]
> Politikas izmaiņas var ilgt līdz pat 24 stundām.