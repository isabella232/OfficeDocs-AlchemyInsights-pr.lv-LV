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
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: fb5745b60d42e1f7d7bb9b7a336a51b62c2ff92a
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762372"
---
# <a name="move-email-to-the-archive-mailbox"></a>Pārvietot e-pastu uz arhīva pastkasti
 
1. Apstipriniet, ka **arhīva pastkaste** ir iespējota. Ja ne, izpildiet [šajā](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) pantā iespējot arhīva pastkastes.

2. Lai arhivētu ziņojumus automātiski arhīva pastkastē, aiztures tagu ar **Pārvietot uz arhīvu** darbība jāiestata uz **automātiski piemērot visu pastkasti (noklusējums) tag**. Izmantot darbības šeit, lai izveidotu tagu: [tag arhīvu noklusējuma](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).
    
3. Tālāk, pievienot tagu **arhīvu** saglabāšanas politiku. Exchange administratoru centrā, izvēlēties **Saglabāšanas politikas** > pievienot, **Pārvietot uz arhīva tagu** politikas > **Saglabāt**. 
    
4. Tagad [piešķirt saglabāšanas politiku](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) noteiktu lietotāja pastkastē. Pašu politiku piemēros **primāro** un **arhīva** pastkasti. 
    
Var būt nepieciešams, lai piespiestu pārvaldītas mapes palīgs (MFA) palaist un lietot jaunos iestatījumus, lietotāja pastkasti. Palaidiet tālāk norādīto komandu kamēr [pievienots EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) sākt pārvaldītas mapes palīgu uz norādīto pastkasti. 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Plašāku informāciju par arhīva politiku iestatīšanu skatiet [Set Arhīvs un dzēšanas politiku pastkastēm](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

