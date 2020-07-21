---
title: Dzēst bāreņlietotāju no lokālā servera
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198181"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="54d8f-102">Dzēst bāreņlietotāju no lokālā servera</span><span class="sxs-lookup"><span data-stu-id="54d8f-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="54d8f-103">Lai noņemtu savrupās lietotājs, rīkojieties šādi:</span><span class="sxs-lookup"><span data-stu-id="54d8f-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="54d8f-104">Vaibst direktorija sinhronizāciju, izpildot [norādījumus kas ir hibrīds identitāti ar Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span><span class="sxs-lookup"><span data-stu-id="54d8f-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="54d8f-105">Lai pārbaudītu direktoriju sinhronizāciju, skatiet [rakstu Kas ir hibrīda identitāte ar Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span><span class="sxs-lookup"><span data-stu-id="54d8f-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="54d8f-106">Ja sinhronizācija darbojas pareizi, bet Active Directory objektu dzēšana nav izplatīt Azure AD, manuāli noņemt savrupās objektu, izmantojot kādu no šīm Azure Active Directory modulis Windows PowerShell cmdlet:</span><span class="sxs-lookup"><span data-stu-id="54d8f-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="54d8f-107">Noņemt MsolContact</span><span class="sxs-lookup"><span data-stu-id="54d8f-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="54d8f-108">Noņemt MsolGroup</span><span class="sxs-lookup"><span data-stu-id="54d8f-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="54d8f-109">Noņemt MsolUser</span><span class="sxs-lookup"><span data-stu-id="54d8f-109">Remove-MsolUser</span></span>

    <span data-ttu-id="54d8f-110">Piemēram, lai noņemtu savrupās lietotāja ID john.smith@contoso.com, kas sākotnēji izveidots, izmantojot direktoriju sinhronizāciju, palaidiet cmdlet:</span><span class="sxs-lookup"><span data-stu-id="54d8f-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="54d8f-111">Remove-MsolUser -UserPrincipal John.Smith@Contoso.comName Remove-MsolUser-UserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="54d8f-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>