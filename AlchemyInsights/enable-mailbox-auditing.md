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
ms.openlocfilehash: 1ef60017f1ea656296bc7b2aa3bc5365646f11f3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527618"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="5a354-102">Ļauj pastkastē auditēšana</span><span class="sxs-lookup"><span data-stu-id="5a354-102">Enable mailbox auditing</span></span>

<span data-ttu-id="5a354-103">Lai pastkastes atsevišķam lietotājam vai visam uzņēmumam šādas cmdlet jādarbojas no attālās enerģijas Shell:</span><span class="sxs-lookup"><span data-stu-id="5a354-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="5a354-104">**Viena lietotāja**</span><span class="sxs-lookup"><span data-stu-id="5a354-104">**Single User**</span></span>
  
<span data-ttu-id="5a354-105">Komplekts-Mailbox - identitāte "Jane Dow" - AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="5a354-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="5a354-106">**Organizācija**</span><span class="sxs-lookup"><span data-stu-id="5a354-106">**Organization**</span></span>
  
<span data-ttu-id="5a354-107">Get-Pastkaste - ResultSize neierobežots - filtru {RecipientTypeDetails - eq "UserMailbox"} | Komplekts-Mailbox - AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="5a354-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="5a354-108">apgūt vairāk</span><span class="sxs-lookup"><span data-stu-id="5a354-108">Learn more</span></span>](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  

