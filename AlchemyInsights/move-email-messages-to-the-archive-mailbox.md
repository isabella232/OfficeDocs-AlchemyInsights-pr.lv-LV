---
title: E-pasta ziņojumi tiks pārvietoti uz arhīva pastkastes
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 41d6825b568263fb7b09066b65235aa348415bae
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/24/2019
ms.locfileid: "29479421"
---
<span data-ttu-id="e991e-p101">Problēmas, arhivēšanas vienumus uz arhīva pastkasti. Pārliecinieties, vai ir veiktas šādas darbības:</span><span class="sxs-lookup"><span data-stu-id="e991e-p101">Having problems archiving items to the Archive mailbox. Make sure you have performed the following steps:</span></span>
  
1. <span data-ttu-id="e991e-p102">Apstipriniet, ka **arhīva pastkaste** ir iespējota. Ja tā nenotiek, izmantojiet soļi [šajā](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) pantā iespējot arhīva pastkasti.</span><span class="sxs-lookup"><span data-stu-id="e991e-p102">Confirm that an **Archive mailbox** has been enabled. If not, use steps in [this article](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span> 
    
2. <span data-ttu-id="e991e-106">Exchange administratoru centrā, izvēlieties **Saglabāšanas Tags** saskaņā ar **Atbilstības pārvaldības**, izveidot **saglabāšanas tag** **Pārvietot uz arhīvu** darbības satur vēlamo **Saglabāšanas vecuma**.</span><span class="sxs-lookup"><span data-stu-id="e991e-106">In the Exchange Admin Center, select **Retention Tags** under **Compliance Management**, create a **Retention tag** with the **Move to Archive** action containing the desired **Retention Age**.</span></span>
    
3. <span data-ttu-id="e991e-107">Exchange administratoru centrā, atlasiet **Saglabāšanas politiku**, izveidot **Saglabāšanas politiku** un **Pārvietot uz arhīvu** saglabāšanas atzīmi pievienotu šo politiku.</span><span class="sxs-lookup"><span data-stu-id="e991e-107">In the Exchange Admin Center, select **Retention Policies**, create a **Retention Policy** and add your **Move to Archive** retention tag to that policy.</span></span> 
    
4. <span data-ttu-id="e991e-p103">Noteiktu lietotāja pastkastē [piešķirt saglabāšanas politiku](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) . Pašu politiku piemēros **primāro** un **arhīva** pastkasti.</span><span class="sxs-lookup"><span data-stu-id="e991e-p103">[Assign the Retention Policy](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox. The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="e991e-p104">Lietotāja pastkastē tagad ir arhīva politikas, lai pārvietotu vienumus uz arhīva pastkasti. Var būt nepieciešams, lai piespiestu pārvaldītas mapes palīgs (MFA) palaist un lietot jaunos iestatījumus, lietotāja pastkasti. Palaidiet tālāk norādīto komandu kamēr [pievienots EXO PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) sākt pārvaldītas mapes palīgu uz norādīto pastkasti.</span><span class="sxs-lookup"><span data-stu-id="e991e-p104">The user's mailbox should now have an Archive policy to move items to the Archive mailbox. It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox. Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="e991e-113">Vēlaties vairāk informācijas par arhīvu politikas iestatīšanu skatiet [Set Arhīvs un dzēšanas politiku pastkastēm](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="e991e-113">Want more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  

