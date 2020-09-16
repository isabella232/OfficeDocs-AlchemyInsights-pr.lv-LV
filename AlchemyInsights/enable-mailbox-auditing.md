---
title: Pastkastes auditēšanas iespējošana
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 404ef9ecd824541f98471bb8797f5f6e025012b7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806298"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="bd06f-102">Pastkastes auditēšanas iespējošana</span><span class="sxs-lookup"><span data-stu-id="bd06f-102">Enable mailbox auditing</span></span>

<span data-ttu-id="bd06f-103">Lai iespējotu pastkastes auditēšanu vienam lietotājam vai visai organizācijai, no attālā Power Shell ir jāpalaiž tālāk norādītie cmdlet:</span><span class="sxs-lookup"><span data-stu-id="bd06f-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="bd06f-104">**Viens lietotājs**</span><span class="sxs-lookup"><span data-stu-id="bd06f-104">**Single User**</span></span>
  
<span data-ttu-id="bd06f-105">Set-Mailbox-Identity "Jane Dow"-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="bd06f-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="bd06f-106">**Organizācijas**</span><span class="sxs-lookup"><span data-stu-id="bd06f-106">**Organization**</span></span>
  
<span data-ttu-id="bd06f-107">Get-Pastkaste — ResultSize Unlimited-Filter {RecipientTypeDetails-EQ "UserMailbox"} | Iestatīt-pastkaste — AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="bd06f-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="bd06f-108">apgūt vairāk</span><span class="sxs-lookup"><span data-stu-id="bd06f-108">Learn more</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

