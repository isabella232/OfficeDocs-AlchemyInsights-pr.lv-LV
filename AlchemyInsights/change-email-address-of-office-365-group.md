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
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="527d6-102">Microsoft 365 grupas e-pasta adreses maiņa</span><span class="sxs-lookup"><span data-stu-id="527d6-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="527d6-103">Microsoft 365 grupas e-pasta adresi varat mainīt, izmantojot administrēšanas centru.</span><span class="sxs-lookup"><span data-stu-id="527d6-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="527d6-104">Vienkārši atlasiet grupu un atlasiet @rediģēt e-pasta adresi.</span><span class="sxs-lookup"><span data-stu-id="527d6-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="527d6-105">Varat arī izmantot šādu EXO PowerShell komandu, lai mainītu Microsoft 365 grupas primāro SMTP adresi:</span><span class="sxs-lookup"><span data-stu-id="527d6-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="527d6-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="527d6-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="527d6-107">Piemērs:</span><span class="sxs-lookup"><span data-stu-id="527d6-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
