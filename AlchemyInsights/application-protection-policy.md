---
title: Lietojumprogrammu aizsardzības politika
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 7fed65e6749f72e6264070b360a52e72968fc8da
ms.sourcegitcommit: 6f7cbf1dc28c0693009ddf03d9768c1c65018964
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/22/2020
ms.locfileid: "45423596"
---
# <a name="application-protection-policy"></a><span data-ttu-id="b39cc-102">Lietojumprogrammu aizsardzības politika</span><span class="sxs-lookup"><span data-stu-id="b39cc-102">Application protection policy</span></span>

<span data-ttu-id="b39cc-103">Ja esat iesācējs programmas aizsardzības politikā (APP), skatiet rakstu [lietojumprogrammu aizsardzības politikas pārskats](https://docs.microsoft.com/intune/apps/app-protection-policy).</span><span class="sxs-lookup"><span data-stu-id="b39cc-103">If you're new to Application protection policy (APP), check out the [App protection policies overview](https://docs.microsoft.com/intune/apps/app-protection-policy).</span></span>

<span data-ttu-id="b39cc-104">Lai sāktu izmantot programmu, Uzziniet, [kā izveidot un piešķirt lietojumprogrammu aizsardzības politikas](https://docs.microsoft.com/intune/app-protection-policies).</span><span class="sxs-lookup"><span data-stu-id="b39cc-104">To start using APP, see [How to create and assign app protection policies](https://docs.microsoft.com/intune/app-protection-policies).</span></span>

<span data-ttu-id="b39cc-105">Lietojumprogrammas aizsardzības politikas prasības:</span><span class="sxs-lookup"><span data-stu-id="b39cc-105">Application protection policy requirements:</span></span>

- <span data-ttu-id="b39cc-106">Lietotājam ir Intune vai EMS licence.</span><span class="sxs-lookup"><span data-stu-id="b39cc-106">User has an Intune or EMS license.</span></span>
- <span data-ttu-id="b39cc-107">Lietotājs pieder grupai, ko nosaka lietojumprogrammu aizsardzības politikas.</span><span class="sxs-lookup"><span data-stu-id="b39cc-107">User belongs to a group targeted by application protection policies.</span></span>
- <span data-ttu-id="b39cc-108">Tikai viens korporatīvais lietotājs ir pierakstījies aizsargātās programmās ierīcē.</span><span class="sxs-lookup"><span data-stu-id="b39cc-108">Only one corporate user is signed into protected apps on a device.</span></span>
- <span data-ttu-id="b39cc-109">Lietojumprogramma ir ieviesusi [INTUNE SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span><span class="sxs-lookup"><span data-stu-id="b39cc-109">The application has implemented the [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span></span> <span data-ttu-id="b39cc-110">Sarakstu ar programmām, kas atbalsta SDK, skatiet rakstā [Microsoft Intune aizsargātas lietojumprogrammas](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span><span class="sxs-lookup"><span data-stu-id="b39cc-110">For a list of apps that support the SDK, see [Microsoft Intune protected apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span></span>

<span data-ttu-id="b39cc-111">Politikas tiek lietotas pēc tam, kad lietotājs, kas atbilst iepriekšminētajām prasībām, paraksta Windows Intune SDK iespējotā lietojumprogrammā.</span><span class="sxs-lookup"><span data-stu-id="b39cc-111">Policies apply after a user who meets the above requirements signs into an Intune SDK enabled app.</span></span> <span data-ttu-id="b39cc-112">Vienkāršākais veids, kā noteikt, vai ir lietota politika, ir pieprasot lietotājam iestatīt PIN kodu.</span><span class="sxs-lookup"><span data-stu-id="b39cc-112">The easiest way to determine if a policy is applied is by requiring that the user set a pin in the policy.</span></span> 

<span data-ttu-id="b39cc-113">Papildinformāciju skatiet rakstā:</span><span class="sxs-lookup"><span data-stu-id="b39cc-113">For more information, see:</span></span>

[<span data-ttu-id="b39cc-114">Bieži uzdotie jautājumi par programmu/MAM problēmu novēršanu</span><span class="sxs-lookup"><span data-stu-id="b39cc-114">APP/MAM troubleshooting FAQ</span></span>](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[<span data-ttu-id="b39cc-115">Programmu aizsardzības politikas iestatīšanas pārbaude</span><span class="sxs-lookup"><span data-stu-id="b39cc-115">How to validate your app protection policy setup</span></span>](https://docs.microsoft.com/intune/app-protection-policies-validate)

[<span data-ttu-id="b39cc-116">Izpratne par programmu aizsardzības politikas piegādes laiku</span><span class="sxs-lookup"><span data-stu-id="b39cc-116">Understand App Protection Policy delivery timing</span></span>](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[<span data-ttu-id="b39cc-117">Programmu aizsardzības politikas pārraudzība</span><span class="sxs-lookup"><span data-stu-id="b39cc-117">How to monitor app protection policies</span></span>](https://docs.microsoft.com/intune/app-protection-policies-monitor)