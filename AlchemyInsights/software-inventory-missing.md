---
title: Trūkst programmatūras krājumu vai tas ir neprecīzi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/26/2021
ms.locfileid: "52676507"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a><span data-ttu-id="b5edf-102">Trūkst programmatūras krājumu vai tas ir neprecīzi</span><span class="sxs-lookup"><span data-stu-id="b5edf-102">Software inventory is missing or inaccurate</span></span>

<span data-ttu-id="b5edf-103">Programmatūras krājumi produktā draudu un ievainojamības pārvaldība (TVM) ir saraksts ar zināmu programmatūru jūsu organizācijā ar oficiāliem platformas uzskaitījumiem (Common Platform Enumerations — CPE).</span><span class="sxs-lookup"><span data-stu-id="b5edf-103">The software inventory in threat and vulnerability management (TVM) is a list of known software in your organization with official Common Platform Enumerations (CPE).</span></span>

<span data-ttu-id="b5edf-104">Programmatūras produktiem bez oficiālas CPE nav publicētas ievainojamības.</span><span class="sxs-lookup"><span data-stu-id="b5edf-104">Software products without an official CPE don’t have vulnerabilities published.</span></span> <span data-ttu-id="b5edf-105">Uz krājumu ir iekļauta arī informācija, piemēram, piegādātāja nosaukums, apdraudējumu skaits un atklāto ierīču skaits.</span><span class="sxs-lookup"><span data-stu-id="b5edf-105">The inventory also includes details such as the name of the vendor, number of weaknesses, threats, and number of exposed devices.</span></span>

<span data-ttu-id="b5edf-106">Programmatūras izmaiņas ierīcēs parasti tiek atspoguļotas drošības portālā divu stundu laikā.</span><span class="sxs-lookup"><span data-stu-id="b5edf-106">Software changes on devices are typically reflected in security portals within two hours.</span></span> <span data-ttu-id="b5edf-107">Tomēr dažreiz ir nepieciešams ilgāks laiks.</span><span class="sxs-lookup"><span data-stu-id="b5edf-107">However, it may sometimes take longer.</span></span> <span data-ttu-id="b5edf-108">Pašlaik nav iespējams veikt piespiedu sinhronizāciju. šis ir nepārtraukts nepārtraukts novērtējums.</span><span class="sxs-lookup"><span data-stu-id="b5edf-108">There’s currently no way to force a sync; this is an ongoing continuous assessment.</span></span>

<span data-ttu-id="b5edf-109">Ja esat veicis programmatūras izmaiņas un TVM pēc 5 stundām tās netiek precīzi atspoguļotas, veiciet šādas darbības:</span><span class="sxs-lookup"><span data-stu-id="b5edf-109">If you made a software change and the change is not accurately reflected in TVM after 5 hours, follow these steps:</span></span>

1. <span data-ttu-id="b5edf-110">Skatiet programmatūras pierādījumu sadaļu, lai saprastu, kā programmatūra tika noteikta.</span><span class="sxs-lookup"><span data-stu-id="b5edf-110">Check the software evidence section to understand how the software was detected.</span></span>
1. <span data-ttu-id="b5edf-111">Pārliecinieties, vai programmatūra tiek atbalstīta.</span><span class="sxs-lookup"><span data-stu-id="b5edf-111">Make sure that the software is supported.</span></span> <span data-ttu-id="b5edf-112">Programmatūra var būt redzama tikai ierīces līmenī pat tad, ja to pašlaik neatbalsta draudu un ievainojamības pārvaldība.</span><span class="sxs-lookup"><span data-stu-id="b5edf-112">Software may be visible only at the device level even if it is currently not supported by threat and vulnerability management.</span></span> <span data-ttu-id="b5edf-113">Tomēr ir pieejami tikai ierobežoti dati.</span><span class="sxs-lookup"><span data-stu-id="b5edf-113">However, only limited data is available.</span></span>
1. <span data-ttu-id="b5edf-114">Informāciju par darbībām, kas jāveic, lai ziņotu par ziņojuma jucību no portāla, skatiet [rakstā Ziņojuma neprecizitāte.](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy)</span><span class="sxs-lookup"><span data-stu-id="b5edf-114">For steps to report the inaccuracy from the portal, see [Report inaccuracy](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span></span>
   
    <span data-ttu-id="b5edf-115">**Piezīme.** Ziņošana par neprecizitāti no MDE portāla ir vienvirziena kanāls, kas inženierzinātnēs tiek ņemts vērā.</span><span class="sxs-lookup"><span data-stu-id="b5edf-115">**Note**: Reporting an inaccuracy from the MDE portal is a one-way channel to engineering.</span></span> <span data-ttu-id="b5edf-116">Ja problēma ir steidzama, atveriet atbalsta biļeti.</span><span class="sxs-lookup"><span data-stu-id="b5edf-116">If the issue is urgent, open a support ticket.</span></span>

<span data-ttu-id="b5edf-117">Papildinformāciju skatiet rakstā [Programmatūras krājumi — draudu un ievainojamības pārvaldība](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span><span class="sxs-lookup"><span data-stu-id="b5edf-117">For more information, see [Software inventory - threat and vulnerability management](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span></span>