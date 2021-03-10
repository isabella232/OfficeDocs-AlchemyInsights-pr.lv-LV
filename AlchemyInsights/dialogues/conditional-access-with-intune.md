---
title: Ierobežotas piekļuves izmantošana ar Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693579"
---
# <a name="using-conditional-access-with-intune"></a><span data-ttu-id="d4e4d-102">Ierobežotas piekļuves izmantošana ar Intune</span><span class="sxs-lookup"><span data-stu-id="d4e4d-102">Using Conditional Access with Intune</span></span>

<span data-ttu-id="d4e4d-103">Ierobežotas piekļuves izmantošanai ar Intune ir jāveic 3 darbības:</span><span class="sxs-lookup"><span data-stu-id="d4e4d-103">Using Conditional Access with Intune requires 3 steps:</span></span>

- [<span data-ttu-id="d4e4d-104">Izveidojiet atbilstības politiku, lai definētu iestatījumus, kas jāizpilda, pirms ierīce tiek uzskatīta par atbilstošu. Piemēram, ierīcei ir jābūt vismaz 6 ciparu spraudīti, pirms tā tiek uzskatīta par atbilstošu.</span><span class="sxs-lookup"><span data-stu-id="d4e4d-104">Create a Compliance Policy to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [<span data-ttu-id="d4e4d-105">Izveidojiet nosacījuma piekļuves politiku, kas nosaka, kādi resursi tiek aizsargāti, un kādi nosacījumi ir jāievēro, lai piekļūtu šiem resursiem. Piemēram, ierīcei ir jābūt savietojamai, pirms piekļūstat korporatīvajam e-pastam.</span><span class="sxs-lookup"><span data-stu-id="d4e4d-105">Create a Conditional Access Policy that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span>](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [<span data-ttu-id="d4e4d-106">Nodrošināt, lai atbilstības politikas un ierobežotas piekļuves politikas būtu paredzētas vajadzīgajām lietotāju grupām. Tam var būt nepieciešama noteiktu lietotāju grupu izveide Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d4e4d-106">Ensure both Compliance Policies and Conditional Access Policies are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[<span data-ttu-id="d4e4d-107">Papildinformācija...</span><span class="sxs-lookup"><span data-stu-id="d4e4d-107">Read more...</span></span>](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
