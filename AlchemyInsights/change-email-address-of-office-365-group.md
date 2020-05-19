---
title: Microsoft 365 grupas e-pasta adreses maiņa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/27/2020
ms.locfileid: "44282927"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a>Microsoft 365 grupas e-pasta adreses maiņa

Varat mainīt e-pasta adresi Microsoft 365 grupas, izmantojot administrēšanas centrs. Vienkārši izvēlieties grupu un izvēlieties @edit e-pasta adresi.

Var izmantot arī pēc EXO PowerShell komandu mainīt primārā SMTP adrese Microsoft 365 grupas:

Set-UnifiedGroup <Group Name> -primarysmtpaddress<new SMTP Address>

Piemērs:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
