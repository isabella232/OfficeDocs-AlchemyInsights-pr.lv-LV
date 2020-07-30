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
ms.openlocfilehash: 9af8a4d3ce72fd901ff2f3a1aae0654c7213dd7e
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522778"
---
# <a name="move-email-to-the-archive-mailbox"></a>E-pasta pārvietošana uz arhīva pastkasti

Ja vēlaties, lai mēs veiktu automatizētās pārbaudes par tālāk norādītajiem iestatījumiem, atlasiet pogu atpakaļ < — šīs lapas augšdaļā un pēc tam ievadiet tā lietotāja e-pasta adresi, kuram ir problēmas ar e-pasta pārvietošanu uz viņu arhīva pastkasti.

1. Apstipriniet, ka **arhīva pastkaste** ir iespējota. Ja ne, veiciet [šajā rakstā](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) norādītās darbības, lai iespējotu arhīva pastkasti.

2. Lai automātiski arhivētu ziņojumus arhīva pastkastei, saglabāšanas tagam ar darbību **Pārvietot uz arhivēšanu** ir jāiestata **automātiski lietot visam pastkastes (noklusējuma) tagam**. Veiciet šeit norādītās darbības, lai izveidotu atzīmi: [Arhivēt noklusējuma atzīmi](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Pēc tam pievienojiet **arhīva** atzīmi savam saglabāšanas politikai. Exchange administrēšanas centrā izvēlieties **saglabāšanas politikas** > pievienot **pāriešanai uz arhīva atzīmi** politikas > **Saglabāt**.

4. Tagad [Piešķiriet saglabāšanas politiku](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) konkrētam lietotāja pastkastei. Viena un tā pati politika tiek lietota gan **primārajai** , gan **arhīva** pastkastei.

Iespējams, ka ir jāspiež pārvaldītā mapes asistents (MFA), lai palaistu un lietotu jaunos iestatījumus lietotāja pastkastē. Izpildiet šādu komandu, kamēr ir [izveidots savienojums ar EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) , lai startētu pārvaldīto mapju palīgu noteiktai pastkastei.
  
Start-ManagedFolderAssistant-Identity<name of the mailbox>

Papildinformāciju par arhīva politikas iestatīšanu skatiet rakstā [arhivēšanas un dzēšanas politikas iestatīšana pastkastēm](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  