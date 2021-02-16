---
title: Grupas politika
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256780"
---
# <a name="group-policy"></a><span data-ttu-id="c3b41-102">Grupas politika</span><span class="sxs-lookup"><span data-stu-id="c3b41-102">Group policy</span></span>

<span data-ttu-id="c3b41-103">Lietotāja un datora objektu iestatījumi Azure Active Directory domēna pakalpojumos (Azure AD DS) bieži tiek pārvaldīti, izmantojot grupas politikas objektus (GPO).</span><span class="sxs-lookup"><span data-stu-id="c3b41-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="c3b41-104">Azure AD DS ir iebūvēts GPO AADDC lietotājiem un AADDC datoru konteineriem.</span><span class="sxs-lookup"><span data-stu-id="c3b41-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="c3b41-105">Šos iebūvētos GPO varat pielāgot, lai pēc vajadzības konfigurētu grupas politiku.</span><span class="sxs-lookup"><span data-stu-id="c3b41-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="c3b41-106">Azure AD DC administratoru grupas dalībniekiem ir grupas politikas administrēšanas privilēģijas Azure AD DS domēnā, kā arī var izveidot pielāgotus GPO un organizācijas vienības (OU).</span><span class="sxs-lookup"><span data-stu-id="c3b41-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="c3b41-107">Papildinformāciju par grupas politiku un to, kā tas darbojas, skatiet sadaļā [grupas politikas pārskats](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span><span class="sxs-lookup"><span data-stu-id="c3b41-107">For more information on what group policy is and how it works, see [Group Policy overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="c3b41-108">Hibrīdajā vidē grupu politikas, kas konfigurētas lokālajā AD DS vidē, netiek sinhronizētas ar Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="c3b41-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="c3b41-109">Lai definētu konfigurācijas iestatījumus lietotājiem vai datoriem Azure AD DS, rediģējiet kādu no noklusējuma GPO vai izveidojiet pielāgotu GPO.</span><span class="sxs-lookup"><span data-stu-id="c3b41-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="c3b41-110">Šajā rakstā [grupas politikas pārvaldība](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) ir parādīts, kā instalēt grupas politikas pārvaldības rīkus, kā ton rediģēt iebūvētos GPO un kā izveidot pielāgotus GPO.</span><span class="sxs-lookup"><span data-stu-id="c3b41-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>



