---
title: Publiskās mapes migrācijas paketi ar CompletedWithErrors statusu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: cbf5237fdb5c660057465e67702e35f68e545ddb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744120"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Publiskās mapes migrācijas paketi ar CompletedWithErrors statusu

Lai pabeigtu paketi, veiciet tālāk norādītās darbības, lai izlaistu lielos/sliktos vienumus: 
1. Apstiprināt izlaistos vienumus migrācijas paketē:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Izmantojiet šo komandu, lai apstiprinātu izlaistos vienumus migrācijas pieprasījumos, kas ir sinhronizēti, bet nav pabeigti.

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Migrācijas paketei un pieprasījumiem ir jāatsāk un jāpabeidz dažas minūtes.

