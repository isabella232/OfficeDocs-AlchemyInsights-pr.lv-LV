---
title: Ierobežotas piekļuves kontroli
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 756c5e98ed3e9cedd0152b5747ea6bf1ed31778e
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/12/2019
ms.locfileid: "29902360"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="be358-102">Ierobežotas piekļuves kontroli</span><span class="sxs-lookup"><span data-stu-id="be358-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="be358-p101">Lietotāju mērķauditorija ar ierobežotas piekļuves saņems paziņojumu e-pastu, ja tās neatbilst jūsu uzņēmuma piekļuves prasības. Lai atrisinātu, mēs iesakām vienu vai vairākus no šiem risinājumiem:</span><span class="sxs-lookup"><span data-stu-id="be358-p101">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements. To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="be358-p102">Ja tiek uzskatīts, ka ierīce tiks uzņemti, konsultēt lietotāja Web vietas uzņēmuma portāls app iet un pārbaudiet, vai tas parādās uzņēmuma portālā. Ja tā nav, lietotājam vajadzētu uzņemt ierīci.</span><span class="sxs-lookup"><span data-stu-id="be358-p102">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal. If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="be358-p103">Debeszils portālā iet uz **Intune \> ierīces atbilstību**. Zem **monitora** noklikšķiniet uz **ierīces atbilstību**. Skatīt ierīces atbilstības ziņojumu, pārliecināties, ka lietotāja ierīces ir atzīmēta kā atbilstošu.</span><span class="sxs-lookup"><span data-stu-id="be358-p103">In the Azure portal go to **Intune \> Device compliance**. Under **Monitor** click **Device compliance**. View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="be358-p104">Debeszils portālā iet uz **Intune \> ierīces atbilstību**. Zem **Pārvaldīt**noklikšķiniet uz **politiku**. Atbilstības politikas sarakstā pārliecinieties, ka profils ir piešķirts jūsu lietotāja ierīces. Ja ir piešķirts neviens profils, tad Intune nevarēs apstiprināt ierīces atbilstības statusu.</span><span class="sxs-lookup"><span data-stu-id="be358-p104">In the Azure portal go to **Intune \> Device compliance**. Under **Manage**, click **Policies**. In the list of compliance policies, verify that a profile is assigned to your user's device. If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="be358-114">Rediģēt lietotāja nosacījuma piekļuves piešķiršana.</span><span class="sxs-lookup"><span data-stu-id="be358-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="be358-115">Debeszils portālā iet uz **Intune \> ierobežotas piekļuves \> politikas**</span><span class="sxs-lookup"><span data-stu-id="be358-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="be358-116">Sarakstā atlasiet politiku</span><span class="sxs-lookup"><span data-stu-id="be358-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="be358-117">Noklikšķiniet uz **lietotāji un grupas**</span><span class="sxs-lookup"><span data-stu-id="be358-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="be358-p105">Lai virzītu politiku, ir kāds, pievienot tos sarakstā **iekļaut** . Lai nodrošinātu, ka persona ir izlaists no politikas, pievienot tos sarakstā **neiekļaut** .</span><span class="sxs-lookup"><span data-stu-id="be358-p105">To target a certain policy at someone, add them to the **Include** list. To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="be358-120">Lasīt tālāk: [kā monitors ierobežotas piekļuves iekārtu](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="be358-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

