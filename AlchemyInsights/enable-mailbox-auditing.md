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
# <a name="enable-mailbox-auditing"></a>Iespējot pastkastes auditēšanu

Lai iespējotu pastkastes auditēšanas vienam lietotājam vai visam uzņēmumam, no attālās barošanas čaulas ir jāpalaiž šādi cmdlet:
  
 **Viena lietotāja**
  
Set-pastkaste-identitāte "Jane Dow"-AuditEnabled $true
  
 **Organizācija**
  
Get-Pastkaste-ResultSize neierobežots-filtrs {RecipientTypeDetails-EQ "UserMailbox"} | Set-pastkaste-AuditEnabled $true
  
[apgūt vairāk](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

