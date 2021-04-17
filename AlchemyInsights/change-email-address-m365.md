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
ms.openlocfilehash: 7800a447c5dfcc8397121e1149921916ff7944ac
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819087"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Microsoft 365 grupas vai Microsoft Teams e-pasta adreses maiņa

Microsoft 365 grupas vai Microsoft Teams e-pasta adresi varat mainīt, izmantojot [Microsoft 365 administrēšanas centru](https://admin.microsoft.com/). Vienkārši atlasiet grupu un atlasiet @edit e-pasta adresi.

Varat arī izmantot tālāk norādīto EXO PowerShell komandu, lai mainītu Microsoft 365 Group/Teams primārā SMTP adresi:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Piemērs:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
