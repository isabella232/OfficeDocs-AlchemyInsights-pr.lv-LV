---
title: Intune ierobežotas piekļuves pārraudzība
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427922"
---
# <a name="monitor-intune-conditional-access"></a><span data-ttu-id="5307e-102">Intune ierobežotas piekļuves pārraudzība</span><span class="sxs-lookup"><span data-stu-id="5307e-102">Monitor Intune Conditional Access</span></span>

<span data-ttu-id="5307e-103">Lietotāji, kuru mērķis ir ierobežotas piekļuves tiesības, saņem paziņojumu e-pasta ziņojumu, ja tie neatbilst jūsu organizācijas piekļuves prasībām.</span><span class="sxs-lookup"><span data-stu-id="5307e-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="5307e-104">Lai atrisinātu šo problēmu, iesakām vienu vai vairākus no šiem risinājumiem:</span><span class="sxs-lookup"><span data-stu-id="5307e-104">To resolve, we recommend one or more of the following solutions:</span></span>

1. <span data-ttu-id="5307e-105">Ja ierīce ir uzskatāma par piereģistrētu, informējiet lietotāju, ka esat pieteicies uzņēmuma portāla programmā, un pārbaudiet, vai tā ir redzama uzņēmuma portālā.</span><span class="sxs-lookup"><span data-stu-id="5307e-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="5307e-106">Ja tā nav, lietotājam ir jāreģistrē ierīce.</span><span class="sxs-lookup"><span data-stu-id="5307e-106">If it doesn't, the user must enroll the device.</span></span>
1. <span data-ttu-id="5307e-107">Azure portālā dodieties uz **Intune**  >  **ierīces atbilstība**.</span><span class="sxs-lookup"><span data-stu-id="5307e-107">In the Azure portal go to **Intune** > **Device compliance**.</span></span> 
1. <span data-ttu-id="5307e-108">Lai skatītu ierīces atbilstības atskaiti, lai pārliecinātos, vai lietotāja ierīce ir atzīmēta kā atbilstoša, sadaļā **monitors** noklikšķiniet uz **ierīces atbilstība**.</span><span class="sxs-lookup"><span data-stu-id="5307e-108">To view your device compliance report to verify that the user's device is marked as compliant, under **Monitor**, click **Device compliance**.</span></span>
1. <span data-ttu-id="5307e-109">Azure portālā dodieties uz **Intune**  >  **ierīces atbilstība**.</span><span class="sxs-lookup"><span data-stu-id="5307e-109">In the Azure portal go to **Intune** > **Device compliance**.</span></span> <span data-ttu-id="5307e-110">Sadaļā **pārvaldība** noklikšķiniet uz **politikas**.</span><span class="sxs-lookup"><span data-stu-id="5307e-110">Under **Manage,** click **Policies**.</span></span> <span data-ttu-id="5307e-111">Atbilstības politiku sarakstā pārbaudiet, vai profils ir piešķirts jūsu lietotāja ierīcei.</span><span class="sxs-lookup"><span data-stu-id="5307e-111">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="5307e-112">Ja nav piešķirts neviens profils, Intune nevarēs apstiprināt ierīces atbilstības statusu.</span><span class="sxs-lookup"><span data-stu-id="5307e-112">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
1. <span data-ttu-id="5307e-113">Rediģējiet lietotāja nosacījuma piekļuves uzdevumu.</span><span class="sxs-lookup"><span data-stu-id="5307e-113">Edit the user's conditional access assignment.</span></span>
1. <span data-ttu-id="5307e-114">Azure portālā pārejiet uz **Intune**  >  **nosacījuma piekļuves**  >  **politikām**, sarakstā atlasiet politiku un noklikšķiniet uz **lietotāji un grupas**.</span><span class="sxs-lookup"><span data-stu-id="5307e-114">In the Azure portal, navigate to **Intune** > **Conditional access** > **Policies**, select a policy from the list, and click **Users and groups**.</span></span>
1. <span data-ttu-id="5307e-115">Lai noteiktu konkrētu politiku, pievienojiet to **sarakstam iekļaut**.</span><span class="sxs-lookup"><span data-stu-id="5307e-115">To target a certain policy at someone, add them to the **Include list**.</span></span> <span data-ttu-id="5307e-116">Lai nodrošinātu to, ka politika nav izlaista, pievienojiet tās **sarakstam neiekļaut**.</span><span class="sxs-lookup"><span data-stu-id="5307e-116">To ensure that a person is omitted from the policy, add them to the **Exclude list**.</span></span>

<span data-ttu-id="5307e-117">**Noderīgas saites:**</span><span class="sxs-lookup"><span data-stu-id="5307e-117">**Helpful links:**</span></span>

- [<span data-ttu-id="5307e-118">Ierīces atbilstības pārskats</span><span class="sxs-lookup"><span data-stu-id="5307e-118">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)
- [<span data-ttu-id="5307e-119">Problēmu novēršana CA</span><span class="sxs-lookup"><span data-stu-id="5307e-119">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [<span data-ttu-id="5307e-120">Problēmu novēršanas politika</span><span class="sxs-lookup"><span data-stu-id="5307e-120">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [<span data-ttu-id="5307e-121">Intune ierīces atbilstības pārraudzība</span><span class="sxs-lookup"><span data-stu-id="5307e-121">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> <span data-ttu-id="5307e-122">Šīs darbības ir noderīgas tikai pakalpojuma Azure Active Directory līdzekļu problēmu novēršanai.</span><span class="sxs-lookup"><span data-stu-id="5307e-122">These steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="5307e-123">Varat arī karantīnā ievietot ierīci, lai bloķētu e-pasta piekļuvi ar Exchange politiku.</span><span class="sxs-lookup"><span data-stu-id="5307e-123">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="5307e-124">Papildinformāciju par Exchange ierīču pārvaldību [**skatiet šeit**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span><span class="sxs-lookup"><span data-stu-id="5307e-124">More information on Exchange device management can be found [**here**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span></span>
