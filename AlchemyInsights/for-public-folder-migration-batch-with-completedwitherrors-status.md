---
title: Publisko mapju migrācijas paketei ar statusu CompletedWithErrors
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: 9ed21bfb9069b56a4fc59b201bb3ad94c6bb6712
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812471"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="3c7b6-102">Publisko mapju migrācijas paketei ar statusu CompletedWithErrors</span><span class="sxs-lookup"><span data-stu-id="3c7b6-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="3c7b6-103">Lai pabeigtu paketi, izlaižot lielus/sliktos vienumus, veiciet šādas darbības:</span><span class="sxs-lookup"><span data-stu-id="3c7b6-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="3c7b6-104">Apstipriniet izlaistos vienumus migrācijas paketē:</span><span class="sxs-lookup"><span data-stu-id="3c7b6-104">Approve the skipped items on migration batch:</span></span>

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. <span data-ttu-id="3c7b6-105">Izmantojiet šo komandu, lai apstiprinātu izlaistos vienumus migrācijas pieprasījumos, kas ir sinhronizēti, bet nav pabeigti:</span><span class="sxs-lookup"><span data-stu-id="3c7b6-105">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. <span data-ttu-id="3c7b6-106">Migrācijas paketei un pieprasījumiem būtu jāturpinās un jāpabeidz pēc dažām minūtēm.</span><span class="sxs-lookup"><span data-stu-id="3c7b6-106">The migration batch and requests should resume and complete in a few minutes.</span></span>

