---
title: Satura meklēšana nav rezultātu
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
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816855"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="61b22-102">Nav rezultātu no satura meklēšanas/eksportēšanas</span><span class="sxs-lookup"><span data-stu-id="61b22-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="61b22-103">Problēmas ar satura meklēšanu/eksportēšanu neatgriež nekādus datus, iespējams, izraisa konkrēts administrators iestatīts atbilstības drošības filtrs, kas netika darīts zināmu visiem administratoriem.</span><span class="sxs-lookup"><span data-stu-id="61b22-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="61b22-104">Lai novērstu šo problēmu, pārbaudiet, vai ir kāds atbilstības drošības filtrs, kas varētu izraisīt šo problēmu:</span><span class="sxs-lookup"><span data-stu-id="61b22-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="61b22-105">Savienojuma izveide ar drošības un atbilstības centra Powershell</span><span class="sxs-lookup"><span data-stu-id="61b22-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="61b22-106">Palaidiet šādus komandsīklietotņus:</span><span class="sxs-lookup"><span data-stu-id="61b22-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="61b22-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="61b22-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="61b22-108">Get-ComplianceSecurityFilter organizācijas $org</span><span class="sxs-lookup"><span data-stu-id="61b22-108">Get-ComplianceSecurityFilter -Organization $org</span></span>