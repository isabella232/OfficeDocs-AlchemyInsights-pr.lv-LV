---
title: Satura meklēšanas/eksportēšanas laikā netiek atgriezti rezultāti
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
- "3200003"
- "7463"
ms.openlocfilehash: 8786f11f170edb151879235e19caa38b50f3f06e
ms.sourcegitcommit: 3d662e1a1440ba74b5347896347d03bb8c8f3af5
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/22/2020
ms.locfileid: "49727230"
---
# <a name="no-results-returned-during-content-searchexport"></a><span data-ttu-id="5757f-102">Satura meklēšanas/eksportēšanas laikā netiek atgriezti rezultāti</span><span class="sxs-lookup"><span data-stu-id="5757f-102">No results returned during Content Search/Export</span></span>

<span data-ttu-id="5757f-103">Ja rodas problēmas ar šādiem e-datu atklāšanas scenārijiem:</span><span class="sxs-lookup"><span data-stu-id="5757f-103">If you are experiencing issues with the following eDiscovery scenarios:</span></span>

- <span data-ttu-id="5757f-104">Satura meklēšana/eksportēšana neatgriež datus vai negaidītus datus</span><span class="sxs-lookup"><span data-stu-id="5757f-104">Content Search/Export returns no data or unexpected data</span></span>
- <span data-ttu-id="5757f-105">e-datu atklāšanas meklēšana vai eksportēšana nav sekmīga</span><span class="sxs-lookup"><span data-stu-id="5757f-105">eDiscovery Search or Export fails</span></span>

<span data-ttu-id="5757f-106">To var izraisīt daži atbilstības drošības filtri, ko iestatīja konkrēts administrators un kas nav paziņoti visiem administratoriem.</span><span class="sxs-lookup"><span data-stu-id="5757f-106">This may be due to certain Compliance Security Filters that were setup by a specific Admin and not been communicated to all Admins.</span></span>

<span data-ttu-id="5757f-107">Lai atrisinātu šo problēmu, pārbaudiet, vai pastāv atbilstības drošības filtri, kas var izraisīt šādas problēmas:</span><span class="sxs-lookup"><span data-stu-id="5757f-107">To resolve this, check if there are any Compliance Security Filters that may be causing these issues:</span></span>

1. <span data-ttu-id="5757f-108">Savienojuma izveide ar drošības un atbilstības centra PowerShell</span><span class="sxs-lookup"><span data-stu-id="5757f-108">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="5757f-109">Palaidiet šādu commandlets:</span><span class="sxs-lookup"><span data-stu-id="5757f-109">Run the following commandlets:</span></span>

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

<span data-ttu-id="5757f-110">Papildu informāciju par atbilstības drošības filtriem skatiet rakstā [atļauju filtrēšana satura meklēšanai](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span><span class="sxs-lookup"><span data-stu-id="5757f-110">For additional information on Compliance Security Filters, see [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span></span>
