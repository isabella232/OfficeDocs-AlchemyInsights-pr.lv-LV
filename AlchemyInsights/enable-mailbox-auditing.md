---
title: Ļauj pastkastē auditēšana
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 81041685cf383a231a9a9739d6daffd6039b4602
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/22/2019
ms.locfileid: "30757825"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="b871c-102">Ļauj pastkastē auditēšana</span><span class="sxs-lookup"><span data-stu-id="b871c-102">Enable mailbox auditing</span></span>

<span data-ttu-id="b871c-103">Lai pastkastes atsevišķam lietotājam vai visam uzņēmumam šādas cmdlet jādarbojas no attālās enerģijas Shell:</span><span class="sxs-lookup"><span data-stu-id="b871c-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="b871c-104">**Viena lietotāja**</span><span class="sxs-lookup"><span data-stu-id="b871c-104">**Single User**</span></span>
  
<span data-ttu-id="b871c-105">Komplekts-Mailbox - identitāte "Jane Dow" - AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="b871c-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="b871c-106">**Organizācija**</span><span class="sxs-lookup"><span data-stu-id="b871c-106">**Organization**</span></span>
  
<span data-ttu-id="b871c-107">Get-Pastkaste - ResultSize neierobežots - filtru {RecipientTypeDetails - eq "UserMailbox"} | Komplekts-Mailbox - AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="b871c-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="b871c-108">apgūt vairāk</span><span class="sxs-lookup"><span data-stu-id="b871c-108">Learn more</span></span>](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  

