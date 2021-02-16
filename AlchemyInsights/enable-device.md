---
title: Iespējot ierīci
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
- "9003257"
- "8278"
ms.openlocfilehash: 9e4b03dcba7a2c98a5d63213ee49f9ba8f91d670
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256872"
---
# <a name="enable-device"></a>Iespējot ierīci

**Lai iespējotu ierīci, izmantojot PowerShell komandu**

Izpildiet tālāk norādītās komandas.

- Lai iegūtu ierīces objektu: `Get-MsolDevice -Name <Name>`
- Lai iespējotu ierīci: `Enable-MsolDevice -DeviceId <DeviceId>`

Papildinformāciju par Hibrīdā savienojuma konfigurēšanu pārvaldītajos domēnos skatiet rakstā [Hibrīdā savienojuma konfigurēšana](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains).
