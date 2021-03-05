---
title: Noskaidrojiet, kurš iestatīja pārsūtīšanu pastkastē un kā
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482301"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a><span data-ttu-id="4e567-102">Noskaidrojiet, kurš iestatīja pārsūtīšanu pastkastē un kā</span><span class="sxs-lookup"><span data-stu-id="4e567-102">Find out who set up forwarding on a mailbox, and how</span></span>

<span data-ttu-id="4e567-103">Ja uz pastkastes ir iestatīta ārējā pārsūtīšana, aktivitāte tiek auditēta kā daļa no Set-Mailbox cmdlet.</span><span class="sxs-lookup"><span data-stu-id="4e567-103">If external forwarding was set on a mailbox, the activity is audited as part of the Set-Mailbox cmdlet.</span></span> <span data-ttu-id="4e567-104">Tālāk ir aprakstīts, kā atrast aktivitāti audita žurnālfailā.</span><span class="sxs-lookup"><span data-stu-id="4e567-104">Here's how to find the activity in the audit log:</span></span>

1. <span data-ttu-id="4e567-105">Dodieties uz [Office 365 drošības & atbilstības centru](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="4e567-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="4e567-106">Atlasiet **meklēšanas** >  **audita žurnālu meklēšana**.</span><span class="sxs-lookup"><span data-stu-id="4e567-106">Select **Search**> **Audit log search**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="4e567-107">Ja redzat paziņojumu par to, ka ir jāieslēdz auditēšana, pārejiet uz priekšu un ieslēdziet to tūlīt.</span><span class="sxs-lookup"><span data-stu-id="4e567-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="4e567-108">Ja šis līdzeklis nav ieslēgts, meklēšanas rezultātos nevarēs paņemt datus no iepriekšējiem datumiem.</span><span class="sxs-lookup"><span data-stu-id="4e567-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="4e567-109">Pārliecinieties, vai lauks **aktivitātes** ir iestatīts uz **Rādīt rezultātus visās aktivitātēs** (noklusējums).</span><span class="sxs-lookup"><span data-stu-id="4e567-109">Make sure the **Activities** field is set to **Show results for all activities** (the default).</span></span> <span data-ttu-id="4e567-110">Norādiet datumu diapazonu.</span><span class="sxs-lookup"><span data-stu-id="4e567-110">Specify the date range.</span></span> <span data-ttu-id="4e567-111">Nav jānorāda lietotājvārds.</span><span class="sxs-lookup"><span data-stu-id="4e567-111">You don't need to specify a username.</span></span>
1. <span data-ttu-id="4e567-112">Atlasiet **Meklēt**.</span><span class="sxs-lookup"><span data-stu-id="4e567-112">Select **Search**.</span></span> <span data-ttu-id="4e567-113">Darbības būs redzamas sadaļā **rezultāti**.</span><span class="sxs-lookup"><span data-stu-id="4e567-113">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="4e567-114">Atlasiet **filtra rezultāti** un pēc tam laukā **darbību** filtrs ievadiet **Set-pastkaste** .</span><span class="sxs-lookup"><span data-stu-id="4e567-114">Select **Filter Results**, and then enter **Set-mailbox** in the **Activity** filter field.</span></span> <span data-ttu-id="4e567-115">Tas atgriež visas **iestatītās pastkastes** darbības.</span><span class="sxs-lookup"><span data-stu-id="4e567-115">This returns all **Set-Mailbox** activities.</span></span>
1. <span data-ttu-id="4e567-116">Lai skatītu detalizētu informāciju, atlasiet aktivitāti un pēc tam atlasiet **Papildinformācija**.</span><span class="sxs-lookup"><span data-stu-id="4e567-116">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="4e567-117">Sadaļā **Parametri** varat redzēt pāradresēšanas e-pasta adresi, kas tika iestatīta pastkastē.</span><span class="sxs-lookup"><span data-stu-id="4e567-117">Under **Parameters** you can see the forwarding email address that was set on the mailbox.</span></span> <span data-ttu-id="4e567-118">Lietotāja **ID** norāda lietotāju, kurš ir iestatījis ārējo pārsūtīšanu pastkastē.</span><span class="sxs-lookup"><span data-stu-id="4e567-118">The **UserID** represents the user who set up external forwarding on the mailbox.</span></span>
<span data-ttu-id="4e567-119">Lai uzzinātu vairāk, skatiet rakstu [meklēšana Office 365 audita žurnālu, lai novērstu raksturīgākos scenārijus](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="4e567-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>