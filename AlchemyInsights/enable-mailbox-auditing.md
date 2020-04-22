---
title: Iespējot pastkastes auditēšanu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: ae11d6be0789a5662d202b85268480a3d42922c4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703578"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="2f029-102">Iespējot pastkastes auditēšanu</span><span class="sxs-lookup"><span data-stu-id="2f029-102">Enable mailbox auditing</span></span>

<span data-ttu-id="2f029-103">Lai iespējotu pastkastes auditēšanas vienam lietotājam vai visam uzņēmumam, no attālās barošanas čaulas ir jāpalaiž šādi cmdlet:</span><span class="sxs-lookup"><span data-stu-id="2f029-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="2f029-104">**Viena lietotāja**</span><span class="sxs-lookup"><span data-stu-id="2f029-104">**Single User**</span></span>
  
<span data-ttu-id="2f029-105">Set-pastkaste-identitāte "Jane Dow"-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="2f029-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="2f029-106">**Organizācija**</span><span class="sxs-lookup"><span data-stu-id="2f029-106">**Organization**</span></span>
  
<span data-ttu-id="2f029-107">Get-Pastkaste-ResultSize neierobežots-filtrs {RecipientTypeDetails-EQ "UserMailbox"} | Set-pastkaste-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="2f029-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="2f029-108">apgūt vairāk</span><span class="sxs-lookup"><span data-stu-id="2f029-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

