---
title: Apple automātiskās ierīču reģistrācijas sinhronizācijas kļūdas
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448929"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="77746-102">Apple automātiskās ierīču reģistrācijas sinhronizācijas kļūdas</span><span class="sxs-lookup"><span data-stu-id="77746-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="77746-103">"Mēs noteikuši, ka jums ir viena vai vairākas ADE/DEP marķierierīces, kas ir kļūdas stāvoklī.</span><span class="sxs-lookup"><span data-stu-id="77746-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="77746-104">Līdz kļūdas stāvokļa atrisināšanai katrai ietekmētajai pilnvarai, funkcija ADE nedarbojas, kā paredzēts.</span><span class="sxs-lookup"><span data-stu-id="77746-104">Until the error state is resolved for each affected token, the ADE functionality will not work as expected.”.</span></span>

<span data-ttu-id="77746-105">Šī kļūda var izpausties vairākos veidos, tostarp:</span><span class="sxs-lookup"><span data-stu-id="77746-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="77746-106">Ierīces var netikt sinhronizētas no ABM/ASM uz Intune</span><span class="sxs-lookup"><span data-stu-id="77746-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="77746-107">Reģistrācijas profila uzdevumi var neizdoties</span><span class="sxs-lookup"><span data-stu-id="77746-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="77746-108">Ierīces var neveiksmīgi pabeigt ADE pieteikšanos</span><span class="sxs-lookup"><span data-stu-id="77746-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="77746-109">Meklējiet sinhronizācijas kļūdu, kas tiek ziņota Intune konsolē sadaļā **ierīces > reģistrēt ierīces > Apple reģistrācijas > reģistrācijas programmas pilnvaras**.</span><span class="sxs-lookup"><span data-stu-id="77746-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens**.</span></span>

<span data-ttu-id="77746-110">Viens no biežākajiem sinhronizācijas kļūdas iemesliem ir pašreizējās marķierierīces derīguma termiņš.</span><span class="sxs-lookup"><span data-stu-id="77746-110">One of the most common causes of sync error is expiration of the current token.</span></span> <span data-ttu-id="77746-111">Daudzi gadījumi atrisinās ietekmētās marķierierīces problēmu.</span><span class="sxs-lookup"><span data-stu-id="77746-111">In many cases,renewal of the affected token will resolve the issue.</span></span>

<span data-ttu-id="77746-112">Ja vienai vai vairākām pilnvarām ir beidzies derīgums, skatiet tālāk norādītās dokumentācijas, kas palīdzēs tās atjaunot, ja nepieciešams.</span><span class="sxs-lookup"><span data-stu-id="77746-112">If one or more of your tokens has expired,  see the following documentation to help you renew them as appropriate:</span></span>

[<span data-ttu-id="77746-113">Automātiskas reģistrācijas marķierierīces atjaunošana</span><span class="sxs-lookup"><span data-stu-id="77746-113">Renew an Automated Device Enrollment token</span></span>](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

<span data-ttu-id="77746-114">Turklāt varat skatīt tālāk norādīto dokumentāciju, lai skatītu iespējamās atrisināšanas iespējas citām kļūdām, kas izraisa marķiera sinhronizācijas kļūdas:</span><span class="sxs-lookup"><span data-stu-id="77746-114">In addition, you can see the following documentation to see potential remediations for other errors causing token synchronization failures:</span></span>

[<span data-ttu-id="77746-115">ABM/ASM sinhronizācijas kļūdas iOS/iPadOS un macOS automatizētās ierīču reģistrācijas marķierierīcēs</span><span class="sxs-lookup"><span data-stu-id="77746-115">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[<span data-ttu-id="77746-116">ABM/ASM sinhronizācijas kļūdas iOS/iPadOS un macOS automatizētās ierīču reģistrācijas marķierierīcēs</span><span class="sxs-lookup"><span data-stu-id="77746-116">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
