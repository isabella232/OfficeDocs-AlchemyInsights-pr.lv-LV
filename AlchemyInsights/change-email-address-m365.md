---
title: Microsoft 365 grupas e-pasta adreses maiņa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: f54ca5df09d0604f6d58c6c8a41dc907485e1f04
ms.sourcegitcommit: beb9715ac0c8e8333fef6764ecd346b7401a2612
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 10/10/2020
ms.locfileid: "48461944"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Microsoft 365 grupas e-pasta adreses maiņa

Varat mainīt Microsoft 365 grupas e-pasta adresi, izmantojot administrēšanas centru. Vienkārši atlasiet grupu un atlasiet @edit e-pasta adresi.

Varat arī izmantot komandu EXO PowerShell, lai mainītu Microsoft 365 grupas primāro SMTP adresi:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Piemēram

`et-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
