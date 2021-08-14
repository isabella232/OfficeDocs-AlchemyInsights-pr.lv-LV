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
ms.openlocfilehash: 6bd9301b983d09f6a0058fee17577b9fc695458ed205f96aacf79a87e4a91e34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930736"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Microsoft 365 grupas e-pasta adreses maiņa

Microsoft 365 grupas e-pasta adresi varat mainīt, izmantojot administrēšanas centru. Vienkārši atlasiet grupu un atlasiet @rediģēt e-pasta adresi.

Varat arī izmantot šādu EXO PowerShell komandu, lai mainītu Microsoft 365 grupas primāro SMTP adresi:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Piemērs:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
