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
ms.openlocfilehash: 4243cdf0170fed1eadac6560d2a04e1a861c63e5
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/15/2020
ms.locfileid: "42043601"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Publiskās mapes migrācijas paketes ar CompletedWithErrors statuss

Lai pabeigtu partiju, izlaižot lielos/sliktos vienumus, veiciet tālāk norādītās darbības. 
1. Apstipriniet izlaistos vienumus migrācijas paketes:

    Kopa MigrationBatch \<grupas nosaukums>-ApproveSkippedItems 
2. Izmantojiet šo komandu, lai apstiprinātu izlaistos vienumus migrācijas pieprasījumi, kas ir "sinhronizēta", bet nav pabeigta:

    $pf = get-PublicFolderMailboxMigrationRequest | Iegūt PublicFolderMailboxMigrationRequestStatistics-IncludeReport; ForEach ($i $pf) {if ($i. LargeItemsEncountered-gt 0-vai $i. BadItemsEncountered-gt 0) {Set-PublicFolderMailboxMigrationRequest $i. Identity. IdentifyingGuid-SkippedItemApprovalTime $ ([DateTime]: UtcNow)}}
3. Migrācijas paketes un pieprasījumi būtu atsākt un pabeigt pēc dažām minūtēm.

