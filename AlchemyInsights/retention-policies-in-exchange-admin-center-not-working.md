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
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 56c2bea5e205358d0ef29fa937e36a88ffc46a1e
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/07/2019
ms.locfileid: "34761589"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="428b5-102">Saglabāšanas politikas maiņas administrēšanas centrā</span><span class="sxs-lookup"><span data-stu-id="428b5-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="428b5-103">**Jautājums:** Jaunizveidotajām vai atjaunināto saglabāšanas politikas maiņas administrēšanas centrā nav piemērotu pastkastēs vai vienumus nevar pārvietot uz arhīva pastkasti vai izdzēst.</span><span class="sxs-lookup"><span data-stu-id="428b5-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="428b5-104">**Galvenie cēloņi:**</span><span class="sxs-lookup"><span data-stu-id="428b5-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="428b5-105">Iespējams, ka **Pārvaldītas mapes palīgu** ir apstrādāts lietotāja pastkastē.</span><span class="sxs-lookup"><span data-stu-id="428b5-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="428b5-106">Pārvaldītas mapes palīgu mēģinās apstrādāt katru pastkastes mākonis balstītas organizācijas reizi septiņās dienās.</span><span class="sxs-lookup"><span data-stu-id="428b5-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="428b5-107">Mainot glabāšanas tag vai piemērot citu saglabāšanas politiku ar pastkasti, var pagaidīt, kamēr pārvaldītas mapes palīdz procesus pastkasti vai var palaist Start ManagedFolderAssistant cmdlet, lai sāktu pārvaldīt mapes palīgu apstrādāt noteiktu pastkasti.</span><span class="sxs-lookup"><span data-stu-id="428b5-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="428b5-108">Darbojas šī cmdlet noder testēšanu vai problēmrisināšanai saglabāšanas politiku vai saglabāšanas tagu iestatījumi.</span><span class="sxs-lookup"><span data-stu-id="428b5-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="428b5-109">Lai iegūtu vairāk informācijas, apmeklējiet [palaist pārvaldītas mapes palīgs](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="428b5-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="428b5-110">**Solution:** Palaidiet tālāk norādīto komandu, lai sāktu pārvaldīt mapes palīgu uz norādīto pastkasti.</span><span class="sxs-lookup"><span data-stu-id="428b5-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span> 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="428b5-111">Tas var notikt, ja **RetentionHold** ir **iespējots** uz pastkasti.</span><span class="sxs-lookup"><span data-stu-id="428b5-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="428b5-112">Ja pastkaste ir piešķirtas RetentionHold, saglabāšanas politiku uz pastkasti nevar apstrādāt šajā laikā.</span><span class="sxs-lookup"><span data-stu-id="428b5-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="428b5-113">Lai iegūtu informāciju par iestatījumu skatiet RetentionHold: [Pastkastes uzglabāšanas turiet](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="428b5-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="428b5-114">**Risinājums:**</span><span class="sxs-lookup"><span data-stu-id="428b5-114">**Solution:**</span></span>
    
  - <span data-ttu-id="428b5-115">RetentionHold iestatījumus uz norādīto pastkasti [EXO](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)PowerShell statusa pārbaude:</span><span class="sxs-lookup"><span data-stu-id="428b5-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="428b5-116">Palaist šādu komandu, lai **atspējotu** RetentionHold uz norādīto pastkasti:</span><span class="sxs-lookup"><span data-stu-id="428b5-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span> 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="428b5-117">Tagad vēlreiz palaidiet pārvaldītā mapē palīgs:</span><span class="sxs-lookup"><span data-stu-id="428b5-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="428b5-118">**Piezīme:** Ja pastkaste ir mazāka par 10 MB, pārvaldītas mapes palīgu automātiski neapstrādās pastkasti.</span><span class="sxs-lookup"><span data-stu-id="428b5-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span> 
  

