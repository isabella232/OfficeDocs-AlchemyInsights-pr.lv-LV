---
title: Sveiciena ziņojums līdzeklī Microsoft 365 grupas
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "5685"
ms.openlocfilehash: 6c46ba1b2c2c94e21d7c76e45df1d416ba423faf
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806413"
---
# <a name="welcome-message-in-microsoft-365-groups"></a>Sveiciena ziņojums līdzeklī Microsoft 365 grupas

Jauni lietotāji, kuri pievienosies Microsoft 365 grupai, saņems sveiciena e-pasta ziņojumu, ja rekvizīta UnifiedGroupWelcomeMessageEnabled vērtība ir True (Patiess).

Ja vēlaties atspējot sveiciena ziņojumu, izmantojiet šādu [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) komandu:

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
