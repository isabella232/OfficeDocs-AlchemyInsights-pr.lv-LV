---
title: Iesūtnes kārtulās veikto notikumu meklēšana
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
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430009"
---
# <a name="find-events-performed-on-inbox-rules"></a><span data-ttu-id="a7d9b-102">Iesūtnes kārtulās veikto notikumu meklēšana</span><span class="sxs-lookup"><span data-stu-id="a7d9b-102">Find events performed on inbox rules</span></span>

<span data-ttu-id="a7d9b-103">Kad iesūtnes kārtulas ir izveidotas, mainītas vai izdzēstas, notikumi tiek ierakstīti audita žurnālu.</span><span class="sxs-lookup"><span data-stu-id="a7d9b-103">When inbox rules are created, changed, or deleted, the events are recorded in the audit log.</span></span> <span data-ttu-id="a7d9b-104">Tālāk ir aprakstīts, kā tās pārskatīt.</span><span class="sxs-lookup"><span data-stu-id="a7d9b-104">Here's how to review them:</span></span>

1. <span data-ttu-id="a7d9b-105">Dodieties uz [Office 365 drošības & atbilstības centru](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="a7d9b-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="a7d9b-106">Atlasiet Meklēt > audita žurnālu meklēšana.</span><span class="sxs-lookup"><span data-stu-id="a7d9b-106">Select Search > Audit log search.</span></span>

    > [!NOTE]
    > <span data-ttu-id="a7d9b-107">Ja redzat paziņojumu par to, ka ir jāieslēdz auditēšana, pārejiet uz priekšu un ieslēdziet to tūlīt.</span><span class="sxs-lookup"><span data-stu-id="a7d9b-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="a7d9b-108">Ja šis līdzeklis nav ieslēgts, meklēšanas rezultātos nevarēs paņemt datus no iepriekšējiem datumiem.</span><span class="sxs-lookup"><span data-stu-id="a7d9b-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="a7d9b-109">Atlasiet lauku aktivitātes un atrodiet Exchange pastkastes darbības un pēc tam atlasiet New-InboxRule izveidot iesūtnes kārtulu no Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="a7d9b-109">Select the Activities field and find Exchange mailbox activities, and then select New-InboxRule Create inbox rule from Outlook Web App.</span></span> <span data-ttu-id="a7d9b-110">Kad tas ir paveikts, noklikšķiniet ārpus rūts, lai minimizētu rūti aktivitātes.</span><span class="sxs-lookup"><span data-stu-id="a7d9b-110">When you're done, click outside of the pane to minimize the Activities pane.</span></span>
1. <span data-ttu-id="a7d9b-111">Norādiet datumu diapazonu un pēc tam laukā lietotāji atlasiet tā lietotāja lietotājvārdu, kuru vēlaties izpētīt.</span><span class="sxs-lookup"><span data-stu-id="a7d9b-111">Specify the date range, and then in the Users field, select the username for the user you want to investigate.</span></span> <span data-ttu-id="a7d9b-112">Vienlaikus varat atlasīt vairākus lietotājus.</span><span class="sxs-lookup"><span data-stu-id="a7d9b-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="a7d9b-113">Atlasiet Meklēt.</span><span class="sxs-lookup"><span data-stu-id="a7d9b-113">Select Search.</span></span> <span data-ttu-id="a7d9b-114">Darbības būs redzamas sadaļā rezultāti.</span><span class="sxs-lookup"><span data-stu-id="a7d9b-114">The activities appear under Results.</span></span>
1. <span data-ttu-id="a7d9b-115">Lai skatītu detalizētu informāciju, atlasiet aktivitāti un pēc tam atlasiet Papildinformācija.</span><span class="sxs-lookup"><span data-stu-id="a7d9b-115">To view details, select an activity, and then select More Information.</span></span> <span data-ttu-id="a7d9b-116">Sadaļā parametri varat skatīt kārtulas nosaukumu, iestatītos nosacījumus un veicamās darbības.</span><span class="sxs-lookup"><span data-stu-id="a7d9b-116">Under the Parameters section you can see the name of the rule, conditions set, and the actions that the rule will take.</span></span>

<span data-ttu-id="a7d9b-117">Lai uzzinātu vairāk, skatiet rakstu meklēšana Office 365 audita žurnālu, lai novērstu raksturīgākos scenārijus.</span><span class="sxs-lookup"><span data-stu-id="a7d9b-117">To learn more, see Search the Office 365 audit log to troubleshoot common scenarios.</span></span>