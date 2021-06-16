---
title: Active Directory netiek sinhronizēts
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930982"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="f1c88-102">Active Directory netiek sinhronizēts</span><span class="sxs-lookup"><span data-stu-id="f1c88-102">Active Directory not syncing</span></span>

<span data-ttu-id="f1c88-103">Ja saņemat sinhronizācijas kļūdas, piemēram, "nav nesenas sinhronizācijas" vai saņemat paziņojumu par direktorija sinhronizēšanas statusu Office administrēšanas portālā, tiek parādīts ziņojums "Pēdējoreiz sinhronizēts pirms vairāk nekā 3 dienām", iespējams, AADConnect ir nepareizi iestatījumi vai nepietiekamas atļaujas sinhronizācijas veikšanai.</span><span class="sxs-lookup"><span data-stu-id="f1c88-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="f1c88-104">AADConnect atkārtota instalēšana, izmantojot ekspresiestatādes iestatījumus, var ātri atrisināt problēmu:</span><span class="sxs-lookup"><span data-stu-id="f1c88-104">Reinstalling AADConnect by using express settings might resolve the issue quickly:</span></span>

1. <span data-ttu-id="f1c88-105">[Lejupielādējiet AADConnect jaunāko versiju.](https://go.microsoft.com/fwlink/?LinkId=615771)</span><span class="sxs-lookup"><span data-stu-id="f1c88-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="f1c88-106">[Izpildiet norādījumus par ekspresinstalēšanu.](/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="f1c88-106">[Follow the instructions for express installation](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="f1c88-107">Azure AD Connect ir jāinstalē Windows Server 2012 vai jaunākā versijā.</span><span class="sxs-lookup"><span data-stu-id="f1c88-107">Azure AD Connect must be installed on Windows Server 2012 or later.</span></span> <span data-ttu-id="f1c88-108">Šim serverim ir jābūt pievienotam domēnam, un tas var būt domēna kontrolleris vai dalībnieku serveris.</span><span class="sxs-lookup"><span data-stu-id="f1c88-108">This server must be domain joined and may be a domain controller or a member server.</span></span> <span data-ttu-id="f1c88-109">Lai iegūtu pilnu Azure AD ad Savienošana prasības un priekšnosacījumus, pārskatiet [Azure AD](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)Savienošana .</span><span class="sxs-lookup"><span data-stu-id="f1c88-109">For a full list of Azure AD Connect requirements and pre-requisites, review [Prerequisites for Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span></span>

<span data-ttu-id="f1c88-110">Papildinformāciju par AADConnect pakalpojumu kontiem skatiet rakstā [Azure AD Savienošana: Konti un atļaujas.](/azure/active-directory/hybrid/reference-connect-accounts-permissions)</span><span class="sxs-lookup"><span data-stu-id="f1c88-110">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
