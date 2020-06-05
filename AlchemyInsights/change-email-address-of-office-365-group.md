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
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580664"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Microsoft 365 grupas e-pasta adreses maiņa

Microsoft 365 grupas e-pasta adresi var mainīt, izmantojot administrēšanas centrs. Vienkārši izvēlieties grupu un izvēlieties @edit e-pasta adresi.

Var izmantot arī pēc EXO PowerShell komandu mainīt primārā SMTP adrese Microsoft 365 grupas:

Set-UnifiedGroup <Group Name> -primarysmtpaddress<new SMTP Address>

Piemērs:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
