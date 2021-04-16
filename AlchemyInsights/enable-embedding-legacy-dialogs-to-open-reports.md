---
title: Mantoto dialogu iegulšanas iespējošana, lai atvērtu atskaites
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814271"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="c5898-102">Mantoto dialogu iegulšanas iespējošana, lai atvērtu atskaites</span><span class="sxs-lookup"><span data-stu-id="c5898-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="c5898-103">**Simptoms**</span><span class="sxs-lookup"><span data-stu-id="c5898-103">**Symptom**</span></span>

<span data-ttu-id="c5898-104">Lietotāji nevar atvērt atskaites.</span><span class="sxs-lookup"><span data-stu-id="c5898-104">Users are unable to open reports.</span></span> <span data-ttu-id="c5898-105">“Radās kāda kļūme.</span><span class="sxs-lookup"><span data-stu-id="c5898-105">"Something has gone wrong.</span></span> <span data-ttu-id="c5898-106">Lai iegūtu papildinformāciju, skatiet tehnisko detalizēto informāciju.”</span><span class="sxs-lookup"><span data-stu-id="c5898-106">Check technical details for more details."</span></span>

<span data-ttu-id="c5898-107">**Iemesls**</span><span class="sxs-lookup"><span data-stu-id="c5898-107">**Cause**</span></span>

<span data-ttu-id="c5898-108">Atskaites neizdodas ielādēt UCI, jo rodas kļūda “Veidlapas deskriptors ir Null vai nav definēts”.</span><span class="sxs-lookup"><span data-stu-id="c5898-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="c5898-109">UCI atskaitēm joprojām ir nepieciešami mantoti dialogi, tāpēc klienta sistēmā ir jābūt iespējotai opcijai *legacydialogsembedding*.</span><span class="sxs-lookup"><span data-stu-id="c5898-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="c5898-110">**Risinājums**</span><span class="sxs-lookup"><span data-stu-id="c5898-110">**Solution**</span></span>

1. <span data-ttu-id="c5898-111">Dodieties uz **Iestatījumi >Administrēšana > Sistēmas iestatījumi > cilne Vispārīgi**.</span><span class="sxs-lookup"><span data-stu-id="c5898-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="c5898-112">Iestatiet opcijas “Iespējot noteiktu mantoto dialogu iegulšanu vienotā interfeisa pārlūkprogrammas klientā” vērtību **Jā**.</span><span class="sxs-lookup"><span data-stu-id="c5898-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
