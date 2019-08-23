---
title: E-pasta ziņojumi tiks pārvietoti uz arhīva pastkastes
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: ce52df446fc4c23c06476e8836ade6a6810d158f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/22/2019
ms.locfileid: "36549010"
---
# <a name="move-email-to-the-archive-mailbox"></a>Pārvietot e-pastu uz arhīva pastkasti

1. Apstipriniet, ka **arhīva pastkaste** ir iespējota. Ja ne, izpildiet [šajā](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) pantā iespējot arhīva pastkastes.

2. Lai arhivētu ziņojumus automātiski arhīva pastkastē, aiztures tagu ar **Pārvietot uz arhīvu** darbība jāiestata uz **automātiski piemērot visu pastkasti (noklusējums) tag**. Izmantot darbības šeit, lai izveidotu tagu: [tag arhīvu noklusējuma](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).

3. Tālāk, pievienot tagu **arhīvu** saglabāšanas politiku. Exchange administratoru centrā, izvēlēties **Saglabāšanas politikas** > pievienot, **Pārvietot uz arhīva tagu** politikas > **saglabāt**.

4. Tagad [piešķirt saglabāšanas politiku](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) noteiktu lietotāja pastkastē. Pašu politiku piemēros **primāro** un **arhīva** pastkasti.

Var būt nepieciešams, lai piespiestu pārvaldītas mapes palīgs (MFA) palaist un lietot jaunos iestatījumus, lietotāja pastkasti. Palaidiet tālāk norādīto komandu kamēr [pievienots EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) sākt pārvaldītas mapes palīgu uz norādīto pastkasti.
  
Sākums-ManagedFolderAssistant-Identity<name of the mailbox>

Plašāku informāciju par arhīva politiku iestatīšanu skatiet [Set Arhīvs un dzēšanas politiku pastkastēm](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  