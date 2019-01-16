---
title: Saglabāšanas politikas maiņas administrēšanas centrā, nedarbojas
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 0ceb1737040f0304bfe8b611241ce1deef487652
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/15/2019
ms.locfileid: "28299891"
---
 **Jautājums:** Jaunizveidotajām vai atjaunināto saglabāšanas politikas maiņas administrēšanas centrā nav piemērotu pastkastēs vai vienumus nevar pārvietot uz arhīva pastkasti vai izdzēst. 
  
 **Galvenie cēloņi:**
  
- Iespējams, ka **Pārvaldītas mapes palīgu** ir apstrādāts lietotāja pastkastē. Pārvaldītas mapes palīgu mēģinās apstrādāt katru pastkastes mākonis balstītas organizācijas reizi septiņās dienās. Mainot glabāšanas tag vai piemērot citu saglabāšanas politiku ar pastkasti, var pagaidīt, kamēr pārvaldītas mapes palīdz procesus pastkasti vai var palaist Start ManagedFolderAssistant cmdlet, lai sāktu pārvaldīt mapes palīgu apstrādāt noteiktu pastkasti. Darbojas šī cmdlet noder testēšanu vai problēmrisināšanai saglabāšanas politiku vai saglabāšanas tagu iestatījumi. Lai iegūtu vairāk informācijas, apmeklējiet [palaist pārvaldītas mapes palīgs](https://msdn.microsoft.com/en-us/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Solution:** Palaidiet tālāk norādīto komandu, lai sāktu pārvaldīt mapes palīgu uz norādīto pastkasti. 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Tas var notikt, ja **RetentionHold** ir **iespējots** uz pastkasti. Ja pastkaste ir piešķirtas RetentionHold, saglabāšanas politiku uz pastkasti nevar apstrādāt šajā laikā. Lai iegūtu informāciju par iestatījumu skatiet RetentionHold: [Pastkastes uzglabāšanas turiet](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Risinājums:**
    
  - RetentionHold iestatījumus uz norādīto pastkasti [EXO](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)PowerShell statusa pārbaude:
    
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
  

