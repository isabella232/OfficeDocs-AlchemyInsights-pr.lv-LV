---
title: Ierobežotas piekļuves pārraudzība
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713725"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="e0433-102">Ierobežotas pieejamības pārraudzība Exchange</span><span class="sxs-lookup"><span data-stu-id="e0433-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="e0433-103">Lietotāji, kuriem ir ierobežotas piekļuves tiesības, saņems e-pasta paziņojumu, ja tie neatbilst jūsu organizācijas piekļuves prasībām.</span><span class="sxs-lookup"><span data-stu-id="e0433-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="e0433-104">Lai atrisinātu problēmu, iesakām izmantot vienu vai vairākus no šiem risinājumiem:</span><span class="sxs-lookup"><span data-stu-id="e0433-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="e0433-105">Ja tiek uzskatīts, ka ierīce ir reģistrēta, ieteikt lietotājam doties uz uzņēmuma portāla lietojumprogrammu un pārliecināties, ka tā parādās uzņēmuma portālā.</span><span class="sxs-lookup"><span data-stu-id="e0433-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="e0433-106">Ja tā nav, lietotājam vajadzētu uzņemt ierīci.</span><span class="sxs-lookup"><span data-stu-id="e0433-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="e0433-107">Azure portālā atveriet \*\* \> InTune ierīces atbilstību\*\*.</span><span class="sxs-lookup"><span data-stu-id="e0433-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="e0433-108">Sadaļā **monitors** noklikšķiniet uz **ierīces atbilstība**.</span><span class="sxs-lookup"><span data-stu-id="e0433-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="e0433-109">Skatiet ierīces atbilstības pārskatu, lai pārbaudītu, vai lietotāja ierīce ir atzīmēta kā atbilstoša.</span><span class="sxs-lookup"><span data-stu-id="e0433-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="e0433-110">Azure portālā atveriet \*\* \> InTune ierīces atbilstību\*\*.</span><span class="sxs-lookup"><span data-stu-id="e0433-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="e0433-111">Zem **pārvaldīt**noklikšķiniet uz **politikas**.</span><span class="sxs-lookup"><span data-stu-id="e0433-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="e0433-112">Atbilstības politiku sarakstā pārbaudiet, vai lietotāja ierīcei ir piešķirts profils.</span><span class="sxs-lookup"><span data-stu-id="e0433-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="e0433-113">Ja profils nav piešķirts, InTune nevarēs apstiprināt ierīces atbilstības statusu.</span><span class="sxs-lookup"><span data-stu-id="e0433-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="e0433-114">Rediģējiet lietotāja ierobežotas piekļuves piešķiri.</span><span class="sxs-lookup"><span data-stu-id="e0433-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="e0433-115">Azure portālā atveriet **InTune \> ierobežotas piekļuves \> politikas**</span><span class="sxs-lookup"><span data-stu-id="e0433-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="e0433-116">Atlasiet politiku no saraksta</span><span class="sxs-lookup"><span data-stu-id="e0433-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="e0433-117">Noklikšķiniet uz **lietotāji un grupas**</span><span class="sxs-lookup"><span data-stu-id="e0433-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="e0433-118">Lai adresēt noteiktu politiku kādam, pievienojiet tos sarakstam **iekļaut** .</span><span class="sxs-lookup"><span data-stu-id="e0433-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="e0433-119">Lai nodrošinātu, ka no politikas tiek izlaista kāda persona, pievienojiet tās **izņēmumu** sarakstam.</span><span class="sxs-lookup"><span data-stu-id="e0433-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="e0433-120">Lasīt tālāk: [kā pārraudzīt ierobežotas piekļuves ierīces](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="e0433-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

