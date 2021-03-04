---
title: IP adreses atrašana audita žurnālfailā
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
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429783"
---
# <a name="find-the-ip-address-in-audit-log"></a><span data-ttu-id="3d96c-102">IP adreses atrašana audita žurnālfailā</span><span class="sxs-lookup"><span data-stu-id="3d96c-102">Find the IP address in audit log</span></span>

1. <span data-ttu-id="3d96c-103">Audita žurnālos tiek parādīta tā IP adrese, kas atbilst lietotāja vai administratora veiktajai darbībai.</span><span class="sxs-lookup"><span data-stu-id="3d96c-103">The IP address that corresponds to an activity performed by a user or administrator is shown in the audit logs.</span></span> <span data-ttu-id="3d96c-104">Tiek reģistrēta arī klienta informācija.</span><span class="sxs-lookup"><span data-stu-id="3d96c-104">The client information is also logged.</span></span> <span data-ttu-id="3d96c-105">Lai noteiktu IP adresi, rīkojieties šādi:</span><span class="sxs-lookup"><span data-stu-id="3d96c-105">Here's how to identify the IP address:</span></span>

1. <span data-ttu-id="3d96c-106">Dodieties uz [Office 365 drošības & atbilstības centru](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="3d96c-106">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="3d96c-107">Atlasiet **meklēšanas**  >  **[audita žurnālu meklēšana](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span><span class="sxs-lookup"><span data-stu-id="3d96c-107">Select **Search** > **[Audit log search](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="3d96c-108">Ja redzat paziņojumu par to, ka ir jāieslēdz auditēšana, pārejiet uz priekšu un ieslēdziet to tūlīt.</span><span class="sxs-lookup"><span data-stu-id="3d96c-108">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="3d96c-109">Ja šis līdzeklis nav iespējots, meklēšanas rezultātos nevarēs paņemt datus no iepriekšējiem datumiem.</span><span class="sxs-lookup"><span data-stu-id="3d96c-109">If this feature isn't enabled, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="3d96c-110">Ja esat ieinteresēts noteiktā aktivitātē, atlasiet to sarakstā **aktivitātes** . Pretējā gadījumā pēc noklusējuma visi darbi tiks atgriezti atlasītajam lietotājam.</span><span class="sxs-lookup"><span data-stu-id="3d96c-110">If you're interested in a specific activity, select it from the **Activities** list; otherwise, by default, all activities will be returned for the selected user.</span></span> <span data-ttu-id="3d96c-111">Ņemiet vērā, ka noteiktas darbības, iespējams, nav pieejamas atlases veikšanai izvēlnē **darbības** . taču šie audita vienumi tiek atgriezti, ja ir atlasīts **Rādīt rezultātus visām darbībām** (noklusējuma iestatījums).</span><span class="sxs-lookup"><span data-stu-id="3d96c-111">Note that certain activities might not be available for selection from the **Activities** menu; however, those audit items will be returned if **Show results for all activities** is selected (default setting).</span></span>
1. <span data-ttu-id="3d96c-112">Norādiet datumu diapazonu un laukā **lietotāji** atlasiet tā lietotāja lietotājvārdu, kuru vēlaties izpētīt.</span><span class="sxs-lookup"><span data-stu-id="3d96c-112">Specify the date range, and in the **Users** field, select the username for the user you want to investigate.</span></span>
1. <span data-ttu-id="3d96c-113">Atlasiet **Meklēt**.</span><span class="sxs-lookup"><span data-stu-id="3d96c-113">Select **Search**.</span></span> <span data-ttu-id="3d96c-114">Darbības būs redzamas sadaļā **rezultāti**.</span><span class="sxs-lookup"><span data-stu-id="3d96c-114">The activities appear under **Results**.</span></span> <span data-ttu-id="3d96c-115">Katrai darbībai varat redzēt IP adresi.</span><span class="sxs-lookup"><span data-stu-id="3d96c-115">You can see the IP address for each activity.</span></span>
1. <span data-ttu-id="3d96c-116">Lai skatītu detalizētu informāciju, atlasiet aktivitāti un pēc tam atlasiet **Papildinformācija**.</span><span class="sxs-lookup"><span data-stu-id="3d96c-116">To view details, select an activity, and then select **More Information**.</span></span>

<span data-ttu-id="3d96c-117">Lai uzzinātu vairāk, skatiet rakstu meklēšana [Office 365 audita žurnālu, lai novērstu raksturīgākos scenārijus](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="3d96c-117">To learn more, see Search the [Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>