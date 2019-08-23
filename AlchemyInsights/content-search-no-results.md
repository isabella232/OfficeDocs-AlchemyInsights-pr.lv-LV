---
title: Satura meklēšana rezultāti
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516786"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="8ba27-102">Nekādi rezultāti no satura meklēšanas/eksports</span><span class="sxs-lookup"><span data-stu-id="8ba27-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="8ba27-103">Problēmas ar satura meklēšanas/eksports nav atgriežot datus var izraisīt noteiktu atbilstību drošības filtrs, kas bija setup īpašas Admin un nav to paziņot visiem Admins.</span><span class="sxs-lookup"><span data-stu-id="8ba27-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="8ba27-104">Lai atrisinātu šo problēmu, pārbaudiet, lai redzētu, vai pastāv atbilstība drošības filtrus, kas izraisa šo:</span><span class="sxs-lookup"><span data-stu-id="8ba27-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="8ba27-105">Drošības un atbilstības centrā Powershell savienojumu</span><span class="sxs-lookup"><span data-stu-id="8ba27-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="8ba27-106">Palaist šādu commandlets:</span><span class="sxs-lookup"><span data-stu-id="8ba27-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="8ba27-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="8ba27-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="8ba27-108">Iegūt ComplianceSecurityFilter-organizācija $org</span><span class="sxs-lookup"><span data-stu-id="8ba27-108">Get-ComplianceSecurityFilter -Organization $org</span></span>