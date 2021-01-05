---
title: Microsoft 365 grupas vai Microsoft Teams e-pasta adreses maiņa
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
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756564"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Microsoft 365 grupas vai Microsoft Teams e-pasta adreses maiņa

Microsoft 365 grupas vai Microsoft Teams e-pasta adresi varat mainīt, izmantojot [Microsoft 365 administrēšanas centru](https://admin.microsoft.com/). Vienkārši atlasiet grupu un atlasiet @edit e-pasta adresi.

Varat arī izmantot tālāk norādīto EXO PowerShell komandu, lai mainītu Microsoft 365 Group/Teams primārā SMTP adresi:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Piemērs:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
