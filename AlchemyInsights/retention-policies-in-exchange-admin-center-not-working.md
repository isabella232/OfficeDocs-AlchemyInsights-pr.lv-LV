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
ms.openlocfilehash: e2fb22f872be0eefc3b4b78b18cd09baffa66cda
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742440"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="bccb0-102">Saglabāšanas politikas Exchange administrēšanas centrs</span><span class="sxs-lookup"><span data-stu-id="bccb0-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="bccb0-103">**Issue:** Jaunizveidoto vai atjaunināto saglabāšanas politikas Exchange administrēšanas centrs neattiecas uz pastkastēm vai vienumiem netiek pārvietoti uz arhīva pastkaste vai dzēsts.</span><span class="sxs-lookup"><span data-stu-id="bccb0-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="bccb0-104">**Cēloņus:**</span><span class="sxs-lookup"><span data-stu-id="bccb0-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="bccb0-105">Iespējams, ka **pārvaldāmās mapes palīgs** nav apstrādājis lietotāja pastkasti.</span><span class="sxs-lookup"><span data-stu-id="bccb0-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="bccb0-106">Pārvaldīto mapju palīgs mēģina katru septiņu dienu laikā apstrādāt visas pastkastes mākonī bāzētu organizācijā.</span><span class="sxs-lookup"><span data-stu-id="bccb0-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="bccb0-107">Ja maināt saglabāšanas tagu vai lietot citu saglabāšanas politikas pastkasti, varat pagaidīt, līdz pārvaldītā mapē Assist apstrādā pastkasti vai sākt ManagedFolderAssistant cmdlet palaist, lai startētu pārvaldīto mapi palīgs apstrādāt noteiktu pastkasti.</span><span class="sxs-lookup"><span data-stu-id="bccb0-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="bccb0-108">Palaižot šo cmdlet ir noderīga pārbaudes vai problēmu novēršanas saglabāšanas politikas vai saglabāšanas tagu iestatījumus.</span><span class="sxs-lookup"><span data-stu-id="bccb0-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="bccb0-109">Lai iegūtu papildinformāciju, apmeklējiet [palaist pārvaldīto mapju palīgu](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="bccb0-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="bccb0-110">**Risinājums:** Palaidiet tālāk minēto komandu, lai startētu pārvaldītā mapē palīgs konkrētu pastkasti:</span><span class="sxs-lookup"><span data-stu-id="bccb0-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="bccb0-111">Tas var notikt arī tad, ja ir **iespējota** **Retentionhold** pastkastē.</span><span class="sxs-lookup"><span data-stu-id="bccb0-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="bccb0-112">Ja pastkastē ir novietots RetentionHold, saglabāšanas politika pastkastē netiks apstrādāti šajā laikā.</span><span class="sxs-lookup"><span data-stu-id="bccb0-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="bccb0-113">Vairāk informācijas par RetentionHold iestatījumu skatiet: [pastkastes saglabāšanas aizturēšana](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="bccb0-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="bccb0-114">**Risinājums:**</span><span class="sxs-lookup"><span data-stu-id="bccb0-114">**Solution:**</span></span>
    
  - <span data-ttu-id="bccb0-115">Pārbaudiet statusu RetentionHold konkrētu pastkasti [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)iestatījumu:</span><span class="sxs-lookup"><span data-stu-id="bccb0-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="bccb0-116">Palaidiet tālāk norādītās komandas, lai **atspējotu** retentionhold noteiktā pastkastē:</span><span class="sxs-lookup"><span data-stu-id="bccb0-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="bccb0-117">Tagad atkārtoti palaidiet pārvaldīto mapju palīgu:</span><span class="sxs-lookup"><span data-stu-id="bccb0-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="bccb0-118">**Piezīme:** Ja pastkaste ir mazāka par 10 MB, pārvaldītā mapē palīgs netiks automātiski apstrādāt pastkasti.</span><span class="sxs-lookup"><span data-stu-id="bccb0-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="bccb0-119">Lai iegūtu papildinformāciju par saglabāšanas politikas Exchange administrēšanas centrs, skatiet:</span><span class="sxs-lookup"><span data-stu-id="bccb0-119">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="bccb0-120">Saglabāšanas tagi un saglabāšanas politikas</span><span class="sxs-lookup"><span data-stu-id="bccb0-120">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="bccb0-121">Saglabāšanas politikas lietošanas pastkastēm</span><span class="sxs-lookup"><span data-stu-id="bccb0-121">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="bccb0-122">Saglabāšanas tagu pievienošana vai noņemšana</span><span class="sxs-lookup"><span data-stu-id="bccb0-122">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="bccb0-123">Kā identificēt pastkastē ievietoto aiztura tipu</span><span class="sxs-lookup"><span data-stu-id="bccb0-123">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
