---
title: Saglabāšanas politikas maiņas administrēšanas centrā, nedarbojas
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: c9061fa728edaab6575a7b1027783e56739a6d14
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/12/2019
ms.locfileid: "29934999"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="57433-102">Saglabāšanas politikas maiņas administrēšanas centrā</span><span class="sxs-lookup"><span data-stu-id="57433-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="57433-103">**Jautājums:** Jaunizveidotajām vai atjaunināto saglabāšanas politikas maiņas administrēšanas centrā nav piemērotu pastkastēs vai vienumus nevar pārvietot uz arhīva pastkasti vai izdzēst.</span><span class="sxs-lookup"><span data-stu-id="57433-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="57433-104">**Galvenie cēloņi:**</span><span class="sxs-lookup"><span data-stu-id="57433-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="57433-p101">Iespējams, ka **Pārvaldītas mapes palīgu** ir apstrādāts lietotāja pastkastē. Pārvaldītas mapes palīgu mēģinās apstrādāt katru pastkastes mākonis balstītas organizācijas reizi septiņās dienās. Mainot glabāšanas tag vai piemērot citu saglabāšanas politiku ar pastkasti, var pagaidīt, kamēr pārvaldītas mapes palīdz procesus pastkasti vai var palaist Start ManagedFolderAssistant cmdlet, lai sāktu pārvaldīt mapes palīgu apstrādāt noteiktu pastkasti. Darbojas šī cmdlet noder testēšanu vai problēmrisināšanai saglabāšanas politiku vai saglabāšanas tagu iestatījumi. Lai iegūtu vairāk informācijas, apmeklējiet [palaist pārvaldītas mapes palīgs](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="57433-p101">This may be because the **Managed Folder Assistant** has not processed the user's mailbox. The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days. If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox. Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings. For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="57433-110">**Solution:** Palaidiet tālāk norādīto komandu, lai sāktu pārvaldīt mapes palīgu uz norādīto pastkasti.</span><span class="sxs-lookup"><span data-stu-id="57433-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span> 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="57433-p102">Tas var notikt, ja **RetentionHold** ir **iespējots** uz pastkasti. Ja pastkaste ir piešķirtas RetentionHold, saglabāšanas politiku uz pastkasti nevar apstrādāt šajā laikā. Lai iegūtu informāciju par iestatījumu skatiet RetentionHold: [Pastkastes uzglabāšanas turiet](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="57433-p102">This may also be occur if **RetentionHold** has been **enabled** on the mailbox. If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time. For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="57433-114">**Risinājums:**</span><span class="sxs-lookup"><span data-stu-id="57433-114">**Solution:**</span></span>
    
  - <span data-ttu-id="57433-115">RetentionHold iestatījumus uz norādīto pastkasti [EXO](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)PowerShell statusa pārbaude:</span><span class="sxs-lookup"><span data-stu-id="57433-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="57433-116">Palaist šādu komandu, lai **atspējotu** RetentionHold uz norādīto pastkasti:</span><span class="sxs-lookup"><span data-stu-id="57433-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span> 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="57433-117">Tagad vēlreiz palaidiet pārvaldītā mapē palīgs:</span><span class="sxs-lookup"><span data-stu-id="57433-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="57433-118">**Piezīme:** Ja pastkaste ir mazāka par 10 MB, pārvaldītas mapes palīgu automātiski neapstrādās pastkasti.</span><span class="sxs-lookup"><span data-stu-id="57433-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span> 
  

