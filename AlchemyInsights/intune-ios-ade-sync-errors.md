---
title: Apple automātiskās ierīču reģistrācijas sinhronizācijas kļūdas
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/17/2020
ms.locfileid: "49714831"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="09cf7-102">Apple automātiskās ierīču reģistrācijas sinhronizācijas kļūdas</span><span class="sxs-lookup"><span data-stu-id="09cf7-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="09cf7-103">"Mēs noteikuši, ka jums ir viena vai vairākas ADE/DEP marķierierīces, kas ir kļūdas stāvoklī.</span><span class="sxs-lookup"><span data-stu-id="09cf7-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="09cf7-104">Līdz kļūdas stāvokļa atrisināšanai katrai ietekmētajai pilnvarai, ADE funkcionalitāte nedarbosies tajā pašā ".</span><span class="sxs-lookup"><span data-stu-id="09cf7-104">Until the error state is resolved for each affected token, the ADE functionality will not work for the same”.</span></span>

<span data-ttu-id="09cf7-105">Šī kļūda var izpausties vairākos veidos, tostarp:</span><span class="sxs-lookup"><span data-stu-id="09cf7-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="09cf7-106">Ierīces var netikt sinhronizētas no ABM/ASM uz Intune</span><span class="sxs-lookup"><span data-stu-id="09cf7-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="09cf7-107">Reģistrācijas profila uzdevumi var neizdoties</span><span class="sxs-lookup"><span data-stu-id="09cf7-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="09cf7-108">Ierīces var neveiksmīgi pabeigt ADE pieteikšanos</span><span class="sxs-lookup"><span data-stu-id="09cf7-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="09cf7-109">Meklējiet sinhronizācijas kļūdu, kas tiek ziņota Intune konsolē sadaļā **ierīces, > reģistrēt ierīces > Apple reģistrācijas > reģistrācijas programmas pilnvaras** un pārskatīt šo dokumentāciju, lai skatītu iespējamo atlīdzināšanu:</span><span class="sxs-lookup"><span data-stu-id="09cf7-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens** and review the following documentation to see any potential remediation:</span></span>

[<span data-ttu-id="09cf7-110">ABM/ASM sinhronizācijas kļūdas iOS/iPadOS un macOS automatizētās ierīču reģistrācijas marķierierīcēs</span><span class="sxs-lookup"><span data-stu-id="09cf7-110">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
