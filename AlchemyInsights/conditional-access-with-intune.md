---
title: Ierobežota piekļuve ar Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931443"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="f8be3-102">Ierobežota piekļuve ar Intune</span><span class="sxs-lookup"><span data-stu-id="f8be3-102">Conditional Access with Intune</span></span>

<span data-ttu-id="f8be3-103">Ierobežotas **piekļuves ar** Intune izmantošanai ir jāveic 3 darbības:</span><span class="sxs-lookup"><span data-stu-id="f8be3-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="f8be3-104">Izveidojiet **atbilstības politiku** [(Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)), lai definētu iestatījumus, kas ir jāizpilda, pirms ierīce tiek uzskatīta par atbilstošu.</span><span class="sxs-lookup"><span data-stu-id="f8be3-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="f8be3-105">Piemēram, ierīces pin jābūt vismaz 6 ciparu kontaktam, pirms to uzskata par atbilstošu.</span><span class="sxs-lookup"><span data-stu-id="f8be3-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="f8be3-106">Izveidojiet **ierobežotas piekļuves politiku,** kas definē, kādi resursi tiek aizsargāti un kādi nosacījumi ir jāizpilda, lai piekļūtu šiem resursiem.</span><span class="sxs-lookup"><span data-stu-id="f8be3-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="f8be3-107">[Piemēram, ierīcei](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) ir jābūt saderīgai pirms piekļuves uzņēmuma e-pastam.</span><span class="sxs-lookup"><span data-stu-id="f8be3-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="f8be3-108">Pārliecinieties, vai **atbilstības politikas** **un ierobežotas piekļuves** politikas ir paredzētas vēlamajās lietotāju grupās.</span><span class="sxs-lookup"><span data-stu-id="f8be3-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="f8be3-109">Tas var būt nepieciešams izveidot noteiktas lietotāju grupas Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f8be3-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="f8be3-110">**Noderīgas saites:**</span><span class="sxs-lookup"><span data-stu-id="f8be3-110">**Helpful links:**</span></span>

[<span data-ttu-id="f8be3-111">Ierīces atbilstības pārskats</span><span class="sxs-lookup"><span data-stu-id="f8be3-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="f8be3-112">Ca problēmu novēršana</span><span class="sxs-lookup"><span data-stu-id="f8be3-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="f8be3-113">Problēmu novēršanas politika</span><span class="sxs-lookup"><span data-stu-id="f8be3-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="f8be3-114">Lai aizsargātu e-pastu (Exchange online) no piekļuves nesaderīgām ierīcēm, jāievēro abi dokumenti:</span><span class="sxs-lookup"><span data-stu-id="f8be3-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="f8be3-115">E-pasta piekļuves aizsardzība no ierīcēm, izmantojot EAS</span><span class="sxs-lookup"><span data-stu-id="f8be3-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="f8be3-116">E-pasta piekļuves aizsardzība no ierīcēm, izmantojot mūsdienu autentifikācijas klientus, piemēram, Outlook</span><span class="sxs-lookup"><span data-stu-id="f8be3-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)