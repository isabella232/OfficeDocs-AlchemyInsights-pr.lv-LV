---
title: E-pasta ziņojumi tiks pārvietoti uz arhīva pastkastes
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: a631af20e28a531a40f078e290239a372c38ab74
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/12/2019
ms.locfileid: "29941721"
---
Problēmas, arhivēšanas vienumus uz arhīva pastkasti. Pārliecinieties, vai ir veiktas šādas darbības:
  
1. Apstipriniet, ka **arhīva pastkaste** ir iespējota. Ja tā nenotiek, izmantojiet soļi [šajā](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) pantā iespējot arhīva pastkasti. 
    
2. Exchange administratoru centrā, izvēlieties **Saglabāšanas Tags** saskaņā ar **Atbilstības pārvaldības**, izveidot **saglabāšanas tag** **Pārvietot uz arhīvu** darbības satur vēlamo **Saglabāšanas vecuma**.
    
3. Exchange administratoru centrā, atlasiet **Saglabāšanas politiku**, izveidot **Saglabāšanas politiku** un **Pārvietot uz arhīvu** saglabāšanas atzīmi pievienotu šo politiku. 
    
4. Noteiktu lietotāja pastkastē [piešķirt saglabāšanas politiku](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) . Pašu politiku piemēros **primāro** un **arhīva** pastkasti. 
    
Lietotāja pastkastē tagad ir arhīva politikas, lai pārvietotu vienumus uz arhīva pastkasti. Var būt nepieciešams, lai piespiestu pārvaldītas mapes palīgs (MFA) palaist un lietot jaunos iestatījumus, lietotāja pastkasti. Palaidiet tālāk norādīto komandu kamēr [pievienots EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) sākt pārvaldītas mapes palīgu uz norādīto pastkasti. 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Vēlaties vairāk informācijas par arhīvu politikas iestatīšanu skatiet [Set Arhīvs un dzēšanas politiku pastkastēm](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

