---
title: Iespējot pastkastes auditēšanu
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
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736260"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="7544f-102">Iespējot pastkastes auditēšanu</span><span class="sxs-lookup"><span data-stu-id="7544f-102">Enable mailbox auditing</span></span>

<span data-ttu-id="7544f-103">Lai iespējotu pastkastes auditēšanas vienam lietotājam vai visam uzņēmumam, no attālās barošanas čaulas ir jāpalaiž šādi cmdlet:</span><span class="sxs-lookup"><span data-stu-id="7544f-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="7544f-104">**Viena lietotāja**</span><span class="sxs-lookup"><span data-stu-id="7544f-104">**Single User**</span></span>
  
<span data-ttu-id="7544f-105">Set-pastkaste-identitāte "Jane Dow"-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="7544f-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="7544f-106">**Organizācija**</span><span class="sxs-lookup"><span data-stu-id="7544f-106">**Organization**</span></span>
  
<span data-ttu-id="7544f-107">Get-Pastkaste-ResultSize neierobežots-filtrs {RecipientTypeDetails-EQ "UserMailbox"} | Set-pastkaste-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="7544f-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="7544f-108">apgūt vairāk</span><span class="sxs-lookup"><span data-stu-id="7544f-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

