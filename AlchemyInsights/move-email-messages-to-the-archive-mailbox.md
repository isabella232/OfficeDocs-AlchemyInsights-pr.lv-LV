---
title: E-pasta ziņojumu pārvietošana uz arhīva pastkasti
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: a5ad81e97df0ed5c337a622126173df94af80bb8
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713653"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="22721-102">Pārvietot e-pastu uz arhīva pastkasti</span><span class="sxs-lookup"><span data-stu-id="22721-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="22721-103">Apstipriniet, ka ir iespējota **arhīva pastkaste** .</span><span class="sxs-lookup"><span data-stu-id="22721-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="22721-104">Ja tā nav, izmantojiet [šajā rakstā](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) aprakstītās darbības, lai iespējotu arhīva pastkaste.</span><span class="sxs-lookup"><span data-stu-id="22721-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="22721-105">Arhivēt ziņojumus automātiski arhīva pastkaste, saglabāšanas tagu ar **Pārvietot uz arhīva** darbība ir jāiestata **automātiski tiek lietots visu pastkastes (noklusējums) tagu**.</span><span class="sxs-lookup"><span data-stu-id="22721-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="22721-106">Lai izveidotu tagu, izmantojiet tālāk aprakstītās darbības. [noklusējuma taga arhivēšana](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="22721-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="22721-107">Pēc tam pievienojiet **arhīva** tagu saglabāšanas politikas.</span><span class="sxs-lookup"><span data-stu-id="22721-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="22721-108">Exchange administrēšanas centrs, izvēlieties **saglabāšanas politikas** > pievienot uz **arhīva tagu** politikas > **saglabāt**.</span><span class="sxs-lookup"><span data-stu-id="22721-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="22721-109">Tagad [piešķirt saglabāšanas politikas](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) konkrēta lietotāja pastkastei.</span><span class="sxs-lookup"><span data-stu-id="22721-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="22721-110">Viena un tā pati politika tiks lietota gan **primārajai** , gan **arhīva** pastkastei.</span><span class="sxs-lookup"><span data-stu-id="22721-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="22721-111">Var būt nepieciešams, lai palaistu pārvaldīto mapju palīgs (MFA) palaist un lietot jaunos iestatījumus lietotāja pastkastei.</span><span class="sxs-lookup"><span data-stu-id="22721-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="22721-112">Palaidiet tālāk minēto komandu, kad [izveidots savienojums ar EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) sākt pārvaldītā mapē palīgs konkrētu pastkasti:</span><span class="sxs-lookup"><span data-stu-id="22721-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="22721-113">Sākuma ManagedFolderAssistant-identitātes<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="22721-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="22721-114">Lai iegūtu papildinformāciju par arhivēšanas politikas iestatīšanu, skatiet [arhīva un dzēšanas politikas iestatīšana pastkastēm](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="22721-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  