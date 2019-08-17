---
title: Saglabāšanas politikas maiņas administrēšanas centrā, nedarbojas
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: d0af4c933f262fe1ec4c2a6ff16d5f6195398b0d
ms.sourcegitcommit: e98443a049108e0dc83d63895af66944bdb1f108
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/16/2019
ms.locfileid: "36444815"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Saglabāšanas politikas maiņas administrēšanas centrā

 **Jautājums:** Jaunizveidotajām vai atjaunināto saglabāšanas politikas maiņas administrēšanas centrā nav piemērotu pastkastēs vai vienumus nevar pārvietot uz arhīva pastkasti vai izdzēst. 
  
 **Galvenie cēloņi:**
  
- Iespējams, ka **Pārvaldītas mapes palīgu** ir apstrādāts lietotāja pastkastē. Pārvaldītas mapes palīgu mēģinās apstrādāt katru pastkastes mākonis balstītas organizācijas reizi septiņās dienās. Mainot glabāšanas tag vai piemērot citu saglabāšanas politiku ar pastkasti, var pagaidīt, kamēr pārvaldītas mapes palīdz procesus pastkasti vai var palaist Start ManagedFolderAssistant cmdlet, lai sāktu pārvaldīt mapes palīgu apstrādāt noteiktu pastkasti. Darbojas šī cmdlet noder testēšanu vai problēmrisināšanai saglabāšanas politiku vai saglabāšanas tagu iestatījumi. Lai iegūtu vairāk informācijas, apmeklējiet [palaist pārvaldītas mapes palīgs](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Solution:** Palaidiet tālāk norādīto komandu, lai sāktu pārvaldīt mapes palīgu uz norādīto pastkasti.
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Tas var notikt, ja **RetentionHold** ir **iespējots** uz pastkasti. Ja pastkaste ir piešķirtas RetentionHold, saglabāšanas politiku uz pastkasti nevar apstrādāt šajā laikā. Lai iegūtu informāciju par iestatījumu skatiet RetentionHold: [Pastkastes uzglabāšanas turiet](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Risinājums:**
    
  - RetentionHold iestatījumus uz norādīto pastkasti [EXO](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)PowerShell statusa pārbaude:
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Palaist šādu komandu, lai **atspējotu** RetentionHold uz norādīto pastkasti:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Tagad vēlreiz palaidiet pārvaldītā mapē palīgs:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Piezīme:** Ja pastkaste ir mazāka par 10 MB, pārvaldītas mapes palīgu automātiski neapstrādās pastkasti.
 
Lai iegūtu vairāk informācijas par saglabāšanas politikas maiņas administrēšanas centrā, skatīt:
- [Aiztures tagus un saglabāšanas politika](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Saglabāšanas politiku lietot pastkastēm](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Pievienojiet vai noņemiet atzīmes izdalīšanas](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Kā noteikt kravas veida likts uz pastkasti](https://docs.microsoft.com/en-us/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
