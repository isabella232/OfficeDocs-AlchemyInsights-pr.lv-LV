---
title: Saglabāšanas politikas Exchange administrēšanas centrā nedarbojas
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
ms.openlocfilehash: 4d3ca121c8d22a0900f136f7f2a754dfb5b435f5
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522814"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="c300b-102">Saglabāšanas politikas Exchange administrēšanas centrā</span><span class="sxs-lookup"><span data-stu-id="c300b-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="c300b-103">Ja vēlaties, lai mēs veiktu automatizētās pārbaudes par tālāk norādītajiem iestatījumiem, atlasiet pogu atpakaļ < — šīs lapas augšdaļā un pēc tam ievadiet tā lietotāja e-pasta adresi, kuram ir problēmas ar saglabāšanas politikām.</span><span class="sxs-lookup"><span data-stu-id="c300b-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="c300b-104">**Problēma:** Jaunizveidotās vai atjauninātās saglabāšanas politikas Exchange administrēšanas centrā neattiecas uz pastkastēm vai vienumiem netiek pārvietoti uz arhīva pastkasti vai izdzēsti.</span><span class="sxs-lookup"><span data-stu-id="c300b-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="c300b-105">**Saknes cēloņi:**</span><span class="sxs-lookup"><span data-stu-id="c300b-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="c300b-106">Tas, iespējams, ir tāpēc, ka **pārvaldītā mapes palīgs** nav apstrādājis lietotāja pastkasti.</span><span class="sxs-lookup"><span data-stu-id="c300b-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="c300b-107">Pārvaldītā mapes palīgs mēģina apstrādāt katru pastkasti mākonī savā organizācijā ik pēc septiņām dienām.</span><span class="sxs-lookup"><span data-stu-id="c300b-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="c300b-108">Ja pastkastē maināt saglabāšanas atzīmi vai lietojat citu saglabāšanas politiku, varat nogaidīt līdz brīdim, kad pārvaldītā mape atbalsta šo pastkasti, vai arī varat palaist sākuma ManagedFolderAssistant cmdlet, lai startētu pārvaldīto mapju palīgu, lai apstrādātu noteiktu pastkasti.</span><span class="sxs-lookup"><span data-stu-id="c300b-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="c300b-109">Šī cmdlet darbība ir noderīga saglabāšanas politikas vai saglabāšanas atzīmju iestatījumu pārbaudei vai problēmu novēršanai.</span><span class="sxs-lookup"><span data-stu-id="c300b-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="c300b-110">Lai iegūtu papildinformāciju, skatiet rakstu [pārvaldītā mapes palīga palaišana](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="c300b-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="c300b-111">**Risinājums:** Palaidiet tālāk norādīto komandu, lai startētu pārvaldīto mapju palīgu noteiktai pastkastei.</span><span class="sxs-lookup"><span data-stu-id="c300b-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="c300b-112">Tas var arī rasties, ja pastkastē ir **iespējota** **RetentionHold** .</span><span class="sxs-lookup"><span data-stu-id="c300b-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="c300b-113">Ja pastkaste ir ievietota RetentionHold, saglabāšanas politika pastkastē netiks apstrādāta šajā laikā.</span><span class="sxs-lookup"><span data-stu-id="c300b-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="c300b-114">Lai iegūtu vairāk instalāciju par RetentionHold iestatījumu, skatiet rakstu [pastkastes aiztures aizturēšana](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="c300b-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="c300b-115">**Risinājumu**</span><span class="sxs-lookup"><span data-stu-id="c300b-115">**Solution:**</span></span>
    
  - <span data-ttu-id="c300b-116">Pārbaudiet RetentionHold statusu noteiktā pastkastē programmā [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="c300b-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="c300b-117">Lai **atspējotu** RetentionHold noteiktā pastkastē, izpildiet šādu komandu:</span><span class="sxs-lookup"><span data-stu-id="c300b-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="c300b-118">Tagad atkārtoti palaidiet pārvaldītās mapes palīgu:</span><span class="sxs-lookup"><span data-stu-id="c300b-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="c300b-119">**Piezīme:** Ja pastkaste ir mazāka par 10 MB, pārvaldītā mapes palīgs automātiski neapstrādās pastkasti.</span><span class="sxs-lookup"><span data-stu-id="c300b-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="c300b-120">Papildinformāciju par saglabāšanas politikām Exchange administrēšanas centrā skatiet šeit:</span><span class="sxs-lookup"><span data-stu-id="c300b-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="c300b-121">Saglabāšanas tagi un saglabāšanas politikas</span><span class="sxs-lookup"><span data-stu-id="c300b-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="c300b-122">Saglabāšanas politikas lietošana pastkastēm</span><span class="sxs-lookup"><span data-stu-id="c300b-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="c300b-123">Saglabāšanas atzīmju pievienošana un noņemšana</span><span class="sxs-lookup"><span data-stu-id="c300b-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="c300b-124">Kā noteikt pastkastes aizturēšanas tipu</span><span class="sxs-lookup"><span data-stu-id="c300b-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
