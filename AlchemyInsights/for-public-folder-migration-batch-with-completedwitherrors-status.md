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
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Publisko mapju migrācijas paketei ar statusu CompletedWithErrors

Lai pabeigtu paketi, izlaižot lielus/sliktos vienumus, veiciet šādas darbības: 
1. Apstipriniet izlaistos vienumus migrācijas paketē:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Izmantojiet šo komandu, lai apstiprinātu izlaistos vienumus migrācijas pieprasījumos, kas ir sinhronizēti, bet nav pabeigti:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Migrācijas paketei un pieprasījumiem būtu jāturpinās un jāpabeidz pēc dažām minūtēm.

