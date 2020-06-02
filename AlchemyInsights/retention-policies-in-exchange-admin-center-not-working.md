---
title: Saglabāšanas politikas Exchange administrēšanas centrs nedarbojas
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 3040365b9d686bcbcce60977ee9bdbbaffc70b24
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502614"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Saglabāšanas politikas Exchange administrēšanas centrs

 **Issue:** Jaunizveidoto vai atjaunināto saglabāšanas politikas Exchange administrēšanas centrs neattiecas uz pastkastēm vai vienumiem netiek pārvietoti uz arhīva pastkaste vai dzēsts. 
  
 **Cēloņus:**
  
- Iespējams, ka **pārvaldāmās mapes palīgs** nav apstrādājis lietotāja pastkasti. Pārvaldīto mapju palīgs mēģina katru septiņu dienu laikā apstrādāt visas pastkastes mākonī bāzētu organizācijā. Ja maināt saglabāšanas tagu vai lietot citu saglabāšanas politikas pastkasti, varat pagaidīt, līdz pārvaldītā mapē Assist apstrādā pastkasti vai sākt ManagedFolderAssistant cmdlet palaist, lai startētu pārvaldīto mapi palīgs apstrādāt noteiktu pastkasti. Palaižot šo cmdlet ir noderīga pārbaudes vai problēmu novēršanas saglabāšanas politikas vai saglabāšanas tagu iestatījumus. Lai iegūtu papildinformāciju, apmeklējiet [palaist pārvaldīto mapju palīgu](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Risinājums:** Palaidiet tālāk minēto komandu, lai startētu pārvaldītā mapē palīgs konkrētu pastkasti:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Tas var notikt arī tad, ja ir **iespējota** **Retentionhold** pastkastē. Ja pastkastē ir novietots RetentionHold, saglabāšanas politika pastkastē netiks apstrādāti šajā laikā. Vairāk informācijas par RetentionHold iestatījumu skatiet: [pastkastes saglabāšanas aizturēšana](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Risinājums:**
    
  - Pārbaudiet statusu RetentionHold konkrētu pastkasti [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)iestatījumu:
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Palaidiet tālāk norādītās komandas, lai **atspējotu** retentionhold noteiktā pastkastē:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Tagad atkārtoti palaidiet pārvaldīto mapju palīgu:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Piezīme:** Ja pastkaste ir mazāka par 10 MB, pārvaldītā mapē palīgs netiks automātiski apstrādāt pastkasti.
 
Lai iegūtu papildinformāciju par saglabāšanas politikas Exchange administrēšanas centrs, skatiet:
- [Saglabāšanas tagi un saglabāšanas politikas](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Saglabāšanas politikas lietošanas pastkastēm](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Saglabāšanas tagu pievienošana vai noņemšana](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Kā identificēt pastkastē ievietoto aiztura tipu](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
