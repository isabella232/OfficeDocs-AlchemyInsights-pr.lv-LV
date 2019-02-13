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
<span data-ttu-id="776aa-p101">Problēmas, arhivēšanas vienumus uz arhīva pastkasti. Pārliecinieties, vai ir veiktas šādas darbības:</span><span class="sxs-lookup"><span data-stu-id="776aa-p101">Having problems archiving items to the Archive mailbox. Make sure you have performed the following steps:</span></span>
  
1. <span data-ttu-id="776aa-p102">Apstipriniet, ka **arhīva pastkaste** ir iespējota. Ja tā nenotiek, izmantojiet soļi [šajā](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) pantā iespējot arhīva pastkasti.</span><span class="sxs-lookup"><span data-stu-id="776aa-p102">Confirm that an **Archive mailbox** has been enabled. If not, use steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span> 
    
2. <span data-ttu-id="776aa-106">Exchange administratoru centrā, izvēlieties **Saglabāšanas Tags** saskaņā ar **Atbilstības pārvaldības**, izveidot **saglabāšanas tag** **Pārvietot uz arhīvu** darbības satur vēlamo **Saglabāšanas vecuma**.</span><span class="sxs-lookup"><span data-stu-id="776aa-106">In the Exchange Admin Center, select **Retention Tags** under **Compliance Management**, create a **Retention tag** with the **Move to Archive** action containing the desired **Retention Age**.</span></span>
    
3. <span data-ttu-id="776aa-107">Exchange administratoru centrā, atlasiet **Saglabāšanas politiku**, izveidot **Saglabāšanas politiku** un **Pārvietot uz arhīvu** saglabāšanas atzīmi pievienotu šo politiku.</span><span class="sxs-lookup"><span data-stu-id="776aa-107">In the Exchange Admin Center, select **Retention Policies**, create a **Retention Policy** and add your **Move to Archive** retention tag to that policy.</span></span> 
    
4. <span data-ttu-id="776aa-p103">Noteiktu lietotāja pastkastē [piešķirt saglabāšanas politiku](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) . Pašu politiku piemēros **primāro** un **arhīva** pastkasti.</span><span class="sxs-lookup"><span data-stu-id="776aa-p103">[Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox. The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="776aa-p104">Lietotāja pastkastē tagad ir arhīva politikas, lai pārvietotu vienumus uz arhīva pastkasti. Var būt nepieciešams, lai piespiestu pārvaldītas mapes palīgs (MFA) palaist un lietot jaunos iestatījumus, lietotāja pastkasti. Palaidiet tālāk norādīto komandu kamēr [pievienots EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) sākt pārvaldītas mapes palīgu uz norādīto pastkasti.</span><span class="sxs-lookup"><span data-stu-id="776aa-p104">The user's mailbox should now have an Archive policy to move items to the Archive mailbox. It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox. Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="776aa-113">Vēlaties vairāk informācijas par arhīvu politikas iestatīšanu skatiet [Set Arhīvs un dzēšanas politiku pastkastēm](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="776aa-113">Want more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  

