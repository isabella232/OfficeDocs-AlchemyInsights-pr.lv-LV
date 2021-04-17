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
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822858"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="67880-102">Active Directory netiek sinhronizēts</span><span class="sxs-lookup"><span data-stu-id="67880-102">Active Directory not syncing</span></span>

<span data-ttu-id="67880-103">Ja saņemat sinhronizācijas kļūdas, piemēram, "nav nesenas sinhronizācijas", vai saņemat paziņojumu par direktorija sinhronizēšanas statusu Office administrēšanas portālā:"Pēdējoreiz sinhronizēts pirms vairāk nekā 3 dienām", iespējams, AADConnect ir nepareizi iestatījumi vai nepietiekamas atļaujas sinhronizācijas veikšanai.</span><span class="sxs-lookup"><span data-stu-id="67880-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="67880-104">AADConnect atkārtota instalēšana, izmantojot ekspresiestatādes iestatījumus, var ātri atrisināt problēmu:</span><span class="sxs-lookup"><span data-stu-id="67880-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="67880-105">[Lejupielādējiet AADConnect jaunāko versiju.](https://go.microsoft.com/fwlink/?LinkId=615771)</span><span class="sxs-lookup"><span data-stu-id="67880-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="67880-106">[Izpildiet norādījumus par ekspresinstalēšanu.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="67880-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="67880-107">Papildinformāciju par AADConnect pakalpojumu kontiem skatiet rakstā [Azure AD Connect: konti un atļaujas.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)</span><span class="sxs-lookup"><span data-stu-id="67880-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
