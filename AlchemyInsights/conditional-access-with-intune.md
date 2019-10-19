---
title: Ierobežotas piekļuves ar InTune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 10/18/2019
ms.locfileid: "36505001"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="4c19b-102">Ierobežotas piekļuves ar InTune</span><span class="sxs-lookup"><span data-stu-id="4c19b-102">Conditional Access with Intune</span></span>

<span data-ttu-id="4c19b-103">Izmantojot **ierobežotas piekļuves** ar InTune nepieciešams 3 soļi:</span><span class="sxs-lookup"><span data-stu-id="4c19b-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="4c19b-104">Izveidojiet **ierobežotas piekļuves politiku** , kas definē, kādi resursi tiek aizsargāti, un kādi nosacījumi ir jāizpilda, lai piekļūtu šiem resursiem.</span><span class="sxs-lookup"><span data-stu-id="4c19b-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="4c19b-105">Piemēram, ierīcei jābūt saderīgai pirms piekļūšanas korporatīvajam e-pastam.</span><span class="sxs-lookup"><span data-stu-id="4c19b-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="4c19b-106">Izveidojiet **atbilstības politiku** , lai definētu iestatījumus, kas jāizpilda, pirms ierīce tiek uzskatīta par atbilstošu.</span><span class="sxs-lookup"><span data-stu-id="4c19b-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="4c19b-107">Piemēram, ierīcei jābūt vismaz 6 ciparu spraudkontaktam, pirms tas tiek uzskatīts par atbilstošu.</span><span class="sxs-lookup"><span data-stu-id="4c19b-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="4c19b-108">Gan **atbilstības politikas** , gan **ierobežotas piekļuves politikas** nodrošināšana ir vērsta uz vēlamajām lietotāju grupām.</span><span class="sxs-lookup"><span data-stu-id="4c19b-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="4c19b-109">Tas var būt nepieciešams izveidot konkrētu lietotāju grupas pakalpojumā Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4c19b-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="4c19b-110">Lasīt vairāk:</span><span class="sxs-lookup"><span data-stu-id="4c19b-110">Read more:</span></span>
  
- [<span data-ttu-id="4c19b-111">Ierobežotas piekļuves paraugprakse</span><span class="sxs-lookup"><span data-stu-id="4c19b-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="4c19b-112">Darba sākšana ar ierobežotu piekļuvi</span><span class="sxs-lookup"><span data-stu-id="4c19b-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

