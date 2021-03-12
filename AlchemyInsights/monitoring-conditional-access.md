---
title: Ierobežotas piekļuves pārraudzība
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708681"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="0ec5d-102">Ierobežotas piekļuves Exchange pārraudzība</span><span class="sxs-lookup"><span data-stu-id="0ec5d-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="0ec5d-103">Lietotāji, kuru mērķis ir ierobežotas piekļuves tiesības, saņem paziņojumu e-pasta ziņojumu, ja tie neatbilst jūsu organizācijas piekļuves prasībām.</span><span class="sxs-lookup"><span data-stu-id="0ec5d-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="0ec5d-104">Lai atrisinātu šo problēmu, iesakām vienu vai vairākus no šiem risinājumiem:</span><span class="sxs-lookup"><span data-stu-id="0ec5d-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="0ec5d-105">Ja ierīce ir uzskatāma par piereģistrētu, informējiet lietotāju, ka esat pieteicies uzņēmuma portāla programmā, un pārbaudiet, vai tā ir redzama uzņēmuma portālā.</span><span class="sxs-lookup"><span data-stu-id="0ec5d-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="0ec5d-106">Ja tā nav, lietotājam ir jāreģistrē ierīce.</span><span class="sxs-lookup"><span data-stu-id="0ec5d-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="0ec5d-107">Azure portālā dodieties uz Intune > ierīces atbilstība.</span><span class="sxs-lookup"><span data-stu-id="0ec5d-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="0ec5d-108">Sadaļā Monitora noklikšķiniet uz ierīces atbilstība.</span><span class="sxs-lookup"><span data-stu-id="0ec5d-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="0ec5d-109">Skatīt ierīces atbilstības atskaiti, lai pārliecinātos, vai lietotāja ierīce ir atzīmēta kā atbilstoša.</span><span class="sxs-lookup"><span data-stu-id="0ec5d-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="0ec5d-110">Azure portālā dodieties uz Intune > ierīces atbilstība.</span><span class="sxs-lookup"><span data-stu-id="0ec5d-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="0ec5d-111">Sadaļā pārvaldība noklikšķiniet uz politikas.</span><span class="sxs-lookup"><span data-stu-id="0ec5d-111">Under Manage, click Policies.</span></span> <span data-ttu-id="0ec5d-112">Atbilstības politiku sarakstā pārbaudiet, vai profils ir piešķirts jūsu lietotāja ierīcei.</span><span class="sxs-lookup"><span data-stu-id="0ec5d-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="0ec5d-113">Ja nav piešķirts neviens profils, Intune nevarēs apstiprināt ierīces atbilstības statusu.</span><span class="sxs-lookup"><span data-stu-id="0ec5d-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="0ec5d-114">Rediģējiet lietotāja nosacījuma piekļuves uzdevumu.</span><span class="sxs-lookup"><span data-stu-id="0ec5d-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="0ec5d-115">Azure portālā dodieties uz **Intune**  >  **ierobežotas piekļuves**  >  **politikām**.</span><span class="sxs-lookup"><span data-stu-id="0ec5d-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="0ec5d-116">Sarakstā atlasiet politiku.</span><span class="sxs-lookup"><span data-stu-id="0ec5d-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="0ec5d-117">Noklikšķiniet uz lietotāji un grupas.</span><span class="sxs-lookup"><span data-stu-id="0ec5d-117">Click Users and groups.</span></span>
4. <span data-ttu-id="0ec5d-118">Lai noteiktu konkrētu politiku, pievienojiet to sarakstam iekļaut.</span><span class="sxs-lookup"><span data-stu-id="0ec5d-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="0ec5d-119">Lai nodrošinātu to, ka politika nav izlaista, pievienojiet tās sarakstam neiekļaut.</span><span class="sxs-lookup"><span data-stu-id="0ec5d-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="0ec5d-120">Noderīgas saites:</span><span class="sxs-lookup"><span data-stu-id="0ec5d-120">Helpful links:</span></span>

[<span data-ttu-id="0ec5d-121">Ierīces atbilstības pārskats</span><span class="sxs-lookup"><span data-stu-id="0ec5d-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="0ec5d-122">Problēmu novēršana CA</span><span class="sxs-lookup"><span data-stu-id="0ec5d-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="0ec5d-123">Problēmu novēršanas politika</span><span class="sxs-lookup"><span data-stu-id="0ec5d-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="0ec5d-124">Intune ierīces atbilstības pārraudzība</span><span class="sxs-lookup"><span data-stu-id="0ec5d-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="0ec5d-125">Piezīme: šīs darbības ir noderīgas tikai pakalpojuma Azure Active Directory līdzekļu problēmu novēršanai.</span><span class="sxs-lookup"><span data-stu-id="0ec5d-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="0ec5d-126">Varat arī karantīnā ievietot ierīci, lai bloķētu e-pasta piekļuvi ar Exchange politiku.</span><span class="sxs-lookup"><span data-stu-id="0ec5d-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="0ec5d-127">Plašāku informāciju par Exchange ierīču pārvaldību var atrast [šeit] ( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .</span><span class="sxs-lookup"><span data-stu-id="0ec5d-127">More information on Exchange device management can be found [here](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141).</span></span>
