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
# <a name="change-email-address-of-an-microsoft-365-group"></a><span data-ttu-id="771cf-102">Microsoft 365 grupas e-pasta adreses maiņa</span><span class="sxs-lookup"><span data-stu-id="771cf-102">Change email address of an Microsoft 365 group</span></span>

<span data-ttu-id="771cf-103">Varat mainīt e-pasta adresi Microsoft 365 grupas, izmantojot administrēšanas centrs.</span><span class="sxs-lookup"><span data-stu-id="771cf-103">You can change the email address of an Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="771cf-104">Vienkārši izvēlieties grupu un izvēlieties @edit e-pasta adresi.</span><span class="sxs-lookup"><span data-stu-id="771cf-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="771cf-105">Var izmantot arī pēc EXO PowerShell komandu mainīt primārā SMTP adrese Microsoft 365 grupas:</span><span class="sxs-lookup"><span data-stu-id="771cf-105">You can also use following the EXO PowerShell command to change the primary SMTP address of an Microsoft 365 group:</span></span>

<span data-ttu-id="771cf-106">Set-UnifiedGroup <Group Name> -primarysmtpaddress<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="771cf-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="771cf-107">Piemērs:</span><span class="sxs-lookup"><span data-stu-id="771cf-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
