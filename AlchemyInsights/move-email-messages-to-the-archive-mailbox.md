---
title: E-pasta ziņojumu pārvietošana uz arhīva pastkasti
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 35c11f1bfb7c61b28a64f0128c29ddf7b4fce939
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511047"
---
# <a name="move-email-to-the-archive-mailbox"></a>Pārvietot e-pastu uz arhīva pastkasti

1. Apstipriniet, ka ir iespējota **arhīva pastkaste** . Ja tā nav, izmantojiet [šajā rakstā](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) aprakstītās darbības, lai iespējotu arhīva pastkaste.

2. Arhivēt ziņojumus automātiski arhīva pastkaste, saglabāšanas tagu ar **Pārvietot uz arhīva** darbība ir jāiestata **automātiski tiek lietots visu pastkastes (noklusējums) tagu**. Lai izveidotu tagu, izmantojiet tālāk aprakstītās darbības. [noklusējuma taga arhivēšana](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Pēc tam pievienojiet **arhīva** tagu saglabāšanas politikas. Exchange administrēšanas centrs, izvēlieties **saglabāšanas politikas** > pievienot uz **arhīva tagu** politikas > **saglabāt**.

4. Tagad [piešķirt saglabāšanas politikas](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) konkrēta lietotāja pastkastei. Viena un tā pati politika tiks lietota gan **primārajai** , gan **arhīva** pastkastei.

Var būt nepieciešams, lai palaistu pārvaldīto mapju palīgs (MFA) palaist un lietot jaunos iestatījumus lietotāja pastkastei. Palaidiet tālāk minēto komandu, kad [izveidots savienojums ar EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) sākt pārvaldītā mapē palīgs konkrētu pastkasti:
  
Sākuma ManagedFolderAssistant-identitātes<name of the mailbox>

Lai iegūtu papildinformāciju par arhivēšanas politikas iestatīšanu, skatiet [arhīva un dzēšanas politikas iestatīšana pastkastēm](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  