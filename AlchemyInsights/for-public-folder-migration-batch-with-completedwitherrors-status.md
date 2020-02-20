---
title: Publiskās mapes migrācijas paketes ar CompletedWithErrors statuss
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: 739e9d91f90e4c0374814d199e4372eb5625553a
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158620"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Publiskās mapes migrācijas paketes ar CompletedWithErrors statuss

Lai pabeigtu partiju, izlaižot lielos/sliktos vienumus, veiciet tālāk norādītās darbības. 
1. Apstipriniet izlaistos vienumus migrācijas paketes:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Izmantojiet šo komandu, lai apstiprinātu izlaistos vienumus migrācijas pieprasījumi, kas ir "sinhronizēta", bet nav pabeigta:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Migrācijas paketes un pieprasījumi būtu atsākt un pabeigt pēc dažām minūtēm.

