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
 <span data-ttu-id="cb852-102">**Jautājums:** Jaunizveidotajām vai atjaunināto saglabāšanas politikas maiņas administrēšanas centrā nav piemērotu pastkastēs vai vienumus nevar pārvietot uz arhīva pastkasti vai izdzēst.</span><span class="sxs-lookup"><span data-stu-id="cb852-102">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="cb852-103">**Galvenie cēloņi:**</span><span class="sxs-lookup"><span data-stu-id="cb852-103">**Root Causes:**</span></span>
  
- <span data-ttu-id="cb852-p101">Iespējams, ka **Pārvaldītas mapes palīgu** ir apstrādāts lietotāja pastkastē. Pārvaldītas mapes palīgu mēģinās apstrādāt katru pastkastes mākonis balstītas organizācijas reizi septiņās dienās. Mainot glabāšanas tag vai piemērot citu saglabāšanas politiku ar pastkasti, var pagaidīt, kamēr pārvaldītas mapes palīdz procesus pastkasti vai var palaist Start ManagedFolderAssistant cmdlet, lai sāktu pārvaldīt mapes palīgu apstrādāt noteiktu pastkasti. Darbojas šī cmdlet noder testēšanu vai problēmrisināšanai saglabāšanas politiku vai saglabāšanas tagu iestatījumi. Lai iegūtu vairāk informācijas, apmeklējiet [palaist pārvaldītas mapes palīgs](https://msdn.microsoft.com/en-us/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="cb852-p101">This may be because the **Managed Folder Assistant** has not processed the user's mailbox. The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days. If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox. Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings. For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/en-us/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="cb852-109">**Solution:** Palaidiet tālāk norādīto komandu, lai sāktu pārvaldīt mapes palīgu uz norādīto pastkasti.</span><span class="sxs-lookup"><span data-stu-id="cb852-109">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span> 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="cb852-p102">Tas var notikt, ja **RetentionHold** ir **iespējots** uz pastkasti. Ja pastkaste ir piešķirtas RetentionHold, saglabāšanas politiku uz pastkasti nevar apstrādāt šajā laikā. Lai iegūtu informāciju par iestatījumu skatiet RetentionHold: [Pastkastes uzglabāšanas turiet](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="cb852-p102">This may also be occur if **RetentionHold** has been **enabled** on the mailbox. If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time. For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="cb852-113">**Risinājums:**</span><span class="sxs-lookup"><span data-stu-id="cb852-113">**Solution:**</span></span>
    
  - <span data-ttu-id="cb852-114">RetentionHold iestatījumus uz norādīto pastkasti [EXO](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)PowerShell statusa pārbaude:</span><span class="sxs-lookup"><span data-stu-id="cb852-114">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="cb852-115">Palaist šādu komandu, lai **atspējotu** RetentionHold uz norādīto pastkasti:</span><span class="sxs-lookup"><span data-stu-id="cb852-115">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span> 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="cb852-116">Tagad vēlreiz palaidiet pārvaldītā mapē palīgs:</span><span class="sxs-lookup"><span data-stu-id="cb852-116">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="cb852-117">**Piezīme:** Ja pastkaste ir mazāka par 10 MB, pārvaldītas mapes palīgu automātiski neapstrādās pastkasti.</span><span class="sxs-lookup"><span data-stu-id="cb852-117">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span> 
  

