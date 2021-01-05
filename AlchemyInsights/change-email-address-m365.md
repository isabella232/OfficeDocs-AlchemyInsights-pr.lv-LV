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
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a><span data-ttu-id="8787b-102">Microsoft 365 grupas vai Microsoft Teams e-pasta adreses maiņa</span><span class="sxs-lookup"><span data-stu-id="8787b-102">Change email address of a Microsoft 365 group or Microsoft Teams</span></span>

<span data-ttu-id="8787b-103">Microsoft 365 grupas vai Microsoft Teams e-pasta adresi varat mainīt, izmantojot [Microsoft 365 administrēšanas centru](https://admin.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="8787b-103">You can change the email address of a Microsoft 365 group or Microsoft Teams by using the [Microsoft 365 admin center](https://admin.microsoft.com/).</span></span> <span data-ttu-id="8787b-104">Vienkārši atlasiet grupu un atlasiet @edit e-pasta adresi.</span><span class="sxs-lookup"><span data-stu-id="8787b-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="8787b-105">Varat arī izmantot tālāk norādīto EXO PowerShell komandu, lai mainītu Microsoft 365 Group/Teams primārā SMTP adresi:</span><span class="sxs-lookup"><span data-stu-id="8787b-105">You can also use the following EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group/Teams:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="8787b-106">Piemērs:</span><span class="sxs-lookup"><span data-stu-id="8787b-106">Example:</span></span>

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
