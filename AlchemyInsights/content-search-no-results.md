---
title: Satura meklēšana bez rezultātiem
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
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680654"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="910d4-102">Nav rezultātu no satura meklēšanas/eksportēšanas</span><span class="sxs-lookup"><span data-stu-id="910d4-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="910d4-103">Problēmas saistībā ar satura meklēšanu/eksportēšanu, kas neatgriež datus, var būt saistīti ar noteiktu atbilstības drošības filtru, ko iestatīja konkrēts administrators un kas to nedara visiem administratoriem.</span><span class="sxs-lookup"><span data-stu-id="910d4-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="910d4-104">Lai atrisinātu šo problēmu, pārbaudiet, vai pastāv atbilstības drošības filtri, kas var izraisīt šādu situāciju:</span><span class="sxs-lookup"><span data-stu-id="910d4-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="910d4-105">Savienojuma izveide ar drošības un atbilstības centra PowerShell</span><span class="sxs-lookup"><span data-stu-id="910d4-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="910d4-106">Palaidiet šādu commandlets:</span><span class="sxs-lookup"><span data-stu-id="910d4-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="910d4-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="910d4-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="910d4-108">Get-ComplianceSecurityFilter-Organization $org</span><span class="sxs-lookup"><span data-stu-id="910d4-108">Get-ComplianceSecurityFilter -Organization $org</span></span>