---
title: E-pasta ziņojumu pārvietošana uz arhīva pastkasti
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 7e72766f441e210a81fcfd6c07b1801f6c0474afb02a70edf2ad8dbb571f3d2a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974964"
---
# <a name="move-email-to-the-archive-mailbox"></a>E-pasta pārvietošana uz arhīva pastkasti

Ja vēlaties, lai mēs automatizēti meklētu tālāk minētos iestatījumus, atlasiet pogu Atpakaļ <- šīs lapas augšdaļā un pēc tam ievadiet tā lietotāja e-pasta adresi, kuram radušās problēmas ar e-pasta pārvietošanu uz arhīva pastkasti.

1. Pārliecinieties, **vai arhīva** pastkaste ir iespējota. Ja tā nav, veiciet šajā rakstā [norādītās darbības,](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) lai iespējotu arhīva pastkasti.

2. Lai ziņojumus automātiski arhivētu arhīva pastkastē, saglabāšanas atzīmei ar darbību Pārvietot uz arhivēšanu jābūt iestatītai automātiskai visai pastkastei **(noklusējuma) atzīmei**.  Veiciet šeit norādītās darbības, lai izveidotu atzīmi: [Arhivēšanas noklusējuma atzīme](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Pēc tam saglabāšanas politikai **pievienojiet** atzīmi Arhīvs. Administrēšanas Exchange izvēlieties Saglabāšanas **politikas** un > pievienot atzīmi Pārvietot uz **arhīvu** politikas lapā > **Saglabāt.**

4. Tagad [piešķiriet saglabāšanas](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) politiku konkrētā lietotāja pastkastei. Viena un tā pati politika tiks lietota gan **primārajai,** gan **arhīva pastkastei.**

Iespējams, būs nepieciešams piespiest pārvaldīto mapju palīgu (Managed Folder Assistant - MFA), lai palaistu un lietotu jaunos iestatījumus lietotāja pastkastē. Izpildiet šādu komandu, kamēr [ir izveidots savienojums ar EXO PowerShell,](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) lai startētu pārvaldāmās mapes palīgu konkrētai pastkastei:
  
Start-ManagedFolderAssistant -Identity <name of the mailbox>

Papildinformāciju par arhīva politikas iestatīšanu skatiet rakstā [Arhīva un dzēšanas politikas iestatīšana pastkastēm.](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)
  