---
title: Ierobežotas piekļuves tiesības ar Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807666"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="31e2c-102">Ierobežotas piekļuves tiesības ar Intune</span><span class="sxs-lookup"><span data-stu-id="31e2c-102">Conditional Access with Intune</span></span>

<span data-ttu-id="31e2c-103">**Ierobežotas piekļuves** izmantošanai ar Intune ir jāveic 3 darbības:</span><span class="sxs-lookup"><span data-stu-id="31e2c-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="31e2c-104">Izveidojiet  **atbilstības politiku**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)), lai definētu iestatījumus, kas jāizpilda, pirms ierīce tiek uzskatīta par atbilstošu.</span><span class="sxs-lookup"><span data-stu-id="31e2c-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="31e2c-105">Piemēram, ierīcei ir jābūt vismaz 6 ciparu spraudīti, pirms tā tiek uzskatīta par atbilstošu.</span><span class="sxs-lookup"><span data-stu-id="31e2c-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="31e2c-106">Izveidojiet **nosacījuma piekļuves politiku**  , kas nosaka, kādi resursi tiek aizsargāti, un kādi nosacījumi ir jāievēro, lai piekļūtu šiem resursiem.</span><span class="sxs-lookup"><span data-stu-id="31e2c-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="31e2c-107">[Piemēram,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  ierīcei ir jābūt savietojamai, pirms piekļūstat korporatīvajam e-pastam.</span><span class="sxs-lookup"><span data-stu-id="31e2c-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="31e2c-108">Nodrošināt, lai **atbilstības politikas**  un  **ierobežotas piekļuves politikas**  būtu paredzētas vajadzīgajām lietotāju grupām.</span><span class="sxs-lookup"><span data-stu-id="31e2c-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="31e2c-109">Tam var būt nepieciešama noteiktu lietotāju grupu izveide Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="31e2c-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="31e2c-110">**Noderīgas saites:**</span><span class="sxs-lookup"><span data-stu-id="31e2c-110">**Helpful links:**</span></span>

[<span data-ttu-id="31e2c-111">Ierīces atbilstības pārskats</span><span class="sxs-lookup"><span data-stu-id="31e2c-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="31e2c-112">Problēmu novēršana CA</span><span class="sxs-lookup"><span data-stu-id="31e2c-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="31e2c-113">Problēmu novēršanas politika</span><span class="sxs-lookup"><span data-stu-id="31e2c-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="31e2c-114">Lai aizsargātu e-pastu (Exchange Online) no piekļuves nesavietojamās ierīcēs, ir jāievēro abi dokumenti:</span><span class="sxs-lookup"><span data-stu-id="31e2c-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="31e2c-115">E-pasta piekļuves aizsardzība no ierīcēm, kas izmanto EAS</span><span class="sxs-lookup"><span data-stu-id="31e2c-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="31e2c-116">E-pasta piekļuves aizsardzība no ierīcēm, kas izmanto modernās autentifikācijas klientus, piemēram, Outlook</span><span class="sxs-lookup"><span data-stu-id="31e2c-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)