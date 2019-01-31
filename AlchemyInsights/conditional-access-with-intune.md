---
title: Ierobežotu piekļuvi ar Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 3b50bc96a879017b62e42e1849f72e68408a0d9d
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/30/2019
ms.locfileid: "29662334"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="0a21c-102">Ierobežotu piekļuvi ar Intune</span><span class="sxs-lookup"><span data-stu-id="0a21c-102">Conditional Access with Intune</span></span>

<span data-ttu-id="0a21c-103">Izmantojot **Ierobežotas piekļuves** ar Intune prasa 3 soļi:</span><span class="sxs-lookup"><span data-stu-id="0a21c-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="0a21c-p101">Izveidot **Ierobežotas piekļuves politikas** , kas nosaka, kādi resursi ir aizsargāta un nosacījumu nepieciešamību, ir jāievēro, lai piekļūtu šiem resursiem. Piemēram, ierīcei jābūt atbilstošiem pirms piekļūstat korporatīvo e-pastu.</span><span class="sxs-lookup"><span data-stu-id="0a21c-p101">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="0a21c-p102">Izveidot **Atbilstība politikas** definēt uzstādījumus, kas jāizpilda, pirms ierīce tiek uzskatīta par atbilstošu. Piemēram, ierīce, pirms tas tiek uzskatīts par atbilstošu, jābūt vismaz 6 ciparu pin.</span><span class="sxs-lookup"><span data-stu-id="0a21c-p102">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="0a21c-p103">Nodrošinot gan **Atbilstības** un **Ierobežotas piekļuves politiku** ir mērķētas uz vajadzīgo lietotāju grupām. Tas var prasīt konkrētu lietotāju grupas izveide Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0a21c-p103">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="0a21c-110">Lasīt vairāk:</span><span class="sxs-lookup"><span data-stu-id="0a21c-110">Read more:</span></span>
  
- [<span data-ttu-id="0a21c-111">Ierobežotas piekļuves labākās prakses</span><span class="sxs-lookup"><span data-stu-id="0a21c-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="0a21c-112">Darba sākšana ar ierobežotas piekļuves</span><span class="sxs-lookup"><span data-stu-id="0a21c-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

