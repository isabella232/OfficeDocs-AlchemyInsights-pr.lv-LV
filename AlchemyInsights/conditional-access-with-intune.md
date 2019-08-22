---
title: Ierobežotu piekļuvi ar Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/22/2019
ms.locfileid: "36505001"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="c4aa7-102">Ierobežotu piekļuvi ar Intune</span><span class="sxs-lookup"><span data-stu-id="c4aa7-102">Conditional Access with Intune</span></span>

<span data-ttu-id="c4aa7-103">Izmantojot **Ierobežotas piekļuves** ar Intune prasa 3 soļi:</span><span class="sxs-lookup"><span data-stu-id="c4aa7-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="c4aa7-104">Izveidot **Ierobežotas piekļuves politikas** , kas nosaka, kādi resursi ir aizsargāta un nosacījumu nepieciešamību, ir jāievēro, lai piekļūtu šiem resursiem.</span><span class="sxs-lookup"><span data-stu-id="c4aa7-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="c4aa7-105">Piemēram, ierīcei jābūt atbilstošiem pirms piekļūstat korporatīvo e-pastu.</span><span class="sxs-lookup"><span data-stu-id="c4aa7-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="c4aa7-106">Izveidot **Atbilstība politikas** definēt uzstādījumus, kas jāizpilda, pirms ierīce tiek uzskatīta par atbilstošu.</span><span class="sxs-lookup"><span data-stu-id="c4aa7-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="c4aa7-107">Piemēram, ierīce, pirms tas tiek uzskatīts par atbilstošu, jābūt vismaz 6 ciparu pin.</span><span class="sxs-lookup"><span data-stu-id="c4aa7-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="c4aa7-108">Nodrošinot gan **Atbilstības** un **Ierobežotas piekļuves politiku** ir mērķētas uz vajadzīgo lietotāju grupām.</span><span class="sxs-lookup"><span data-stu-id="c4aa7-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="c4aa7-109">Tas var prasīt konkrētu lietotāju grupas izveide Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c4aa7-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="c4aa7-110">Lasīt vairāk:</span><span class="sxs-lookup"><span data-stu-id="c4aa7-110">Read more:</span></span>
  
- [<span data-ttu-id="c4aa7-111">Ierobežotas piekļuves labākās prakses</span><span class="sxs-lookup"><span data-stu-id="c4aa7-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="c4aa7-112">Darba sākšana ar ierobežotas piekļuves</span><span class="sxs-lookup"><span data-stu-id="c4aa7-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

