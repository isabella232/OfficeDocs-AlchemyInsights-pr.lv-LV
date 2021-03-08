---
title: Audita žurnālu lomas piešķiršana Office 365 drošības & atbilstības centrā
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 0eb470b6c17def5517db2f866ef40898b36662ed
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526522"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a><span data-ttu-id="effe9-102">Audita žurnālu lomas piešķiršana Office 365 drošības & atbilstības centrā</span><span class="sxs-lookup"><span data-stu-id="effe9-102">Assign an Audit Log role in the Office 365 Security & Compliance Center</span></span>

<span data-ttu-id="effe9-103">Lai meklētu Office 365 audita žurnālā, administratoram jābūt piešķirtai **tikai skatīšanas audita žurnālu** lomai vai **audita žurnālu** lomai pakalpojumā Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="effe9-103">To search the Office 365 audit log, an administrator must be assigned the **View-Only Audit Logs** role or the **Audit Logs** role in Exchange Online.</span></span> <span data-ttu-id="effe9-104">Pēc noklusējuma šīs lomas ir piešķirtas atbilstības pārvaldības un organizācijas pārvaldības lomu grupām.</span><span class="sxs-lookup"><span data-stu-id="effe9-104">These roles are assigned to the Compliance Management and Organization Management role groups by default.</span></span> <span data-ttu-id="effe9-105">Globālie administratori pakalpojumā Office 365 un Microsoft 365 tiek automātiski pievienoti kā organizācijas pārvaldības lomu grupas dalībnieki.</span><span class="sxs-lookup"><span data-stu-id="effe9-105">Global administrators in Office 365 and Microsoft 365 are automatically added as members of the Organization Management role group.</span></span>

<span data-ttu-id="effe9-106">Lai lietotājam atļautu meklēt ar minimālajiem atļauju līmeņiem, izveidojiet pielāgotu lomu grupu pakalpojumā Exchange Online, pievienojiet **tikai skatīšanas audita žurnālu** lomu vai **audita žurnālus** un pēc tam pievienojiet lietotāju kā jaunās lomu grupas dalībnieku.</span><span class="sxs-lookup"><span data-stu-id="effe9-106">To enable a user to search with the minimum level of privileges, create a custom role group in Exchange Online, add the **View-Only Audit Logs** role or **Audit Logs** role, and then add the user as a member of the new role group.</span></span>

<span data-ttu-id="effe9-107">Papildinformāciju skatiet rakstā [lomu grupu pārvaldība pakalpojumā Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) un [meklēšanas audita žurnāls drošības & atbilstības centrā](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span><span class="sxs-lookup"><span data-stu-id="effe9-107">For more information, see [Manage role groups in Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) and [Search the audit log in the Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>