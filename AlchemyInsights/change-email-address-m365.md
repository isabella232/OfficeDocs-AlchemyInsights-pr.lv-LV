---
title: Microsoft 365 grupas vai Microsoft Teams e-pasta adreses maiņa
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
ms.openlocfilehash: acb343553bfb7e100c03d0e7046ed5cbdd6b739b9a61e3faf17768bd8aadff34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995629"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Microsoft 365 grupas vai Microsoft Teams e-pasta adreses maiņa

Microsoft 365 grupas vai Microsoft Teams e-pasta adresi varat mainīt, izmantojot [Microsoft 365 administrēšanas centru](https://admin.microsoft.com/). Vienkārši atlasiet grupu un atlasiet @edit e-pasta adresi.

Varat arī izmantot tālāk norādīto EXO PowerShell komandu, lai mainītu Microsoft 365 Group/Teams primārā SMTP adresi:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Piemērs:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
