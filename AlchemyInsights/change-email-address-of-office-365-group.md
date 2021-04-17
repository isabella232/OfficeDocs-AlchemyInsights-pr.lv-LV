---
title: Microsoft 365 grupas e-pasta adreses maiņa
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
- "4704"
ms.openlocfilehash: 8eaafae8650a8072cdfbec281afe6d5e93fea655
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819051"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Microsoft 365 grupas e-pasta adreses maiņa

Microsoft 365 grupas e-pasta adresi varat mainīt, izmantojot administrēšanas centru. Vienkārši atlasiet grupu un atlasiet @rediģēt e-pasta adresi.

Varat arī izmantot šādu EXO PowerShell komandu, lai mainītu Microsoft 365 grupas primāro SMTP adresi:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Piemērs:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
