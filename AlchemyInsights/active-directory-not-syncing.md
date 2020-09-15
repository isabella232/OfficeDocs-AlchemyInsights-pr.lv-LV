---
title: Active Directory netiek sinhronizēts
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697636"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="8ca8b-102">Active Directory netiek sinhronizēts</span><span class="sxs-lookup"><span data-stu-id="8ca8b-102">Active Directory not syncing</span></span>

<span data-ttu-id="8ca8b-103">Ja saņemat sinhronizācijas kļūdas, piemēram, "nav pēdējās sinhronizācijas" vai paziņojums par direktorija sinhronizēšanas statusu Office administrēšanas portālā, tiek rādīts ziņojums "Pēdējoreiz sinhronizēts vairāk nekā pirms 3 dienām", iespējams, ka AADConnect ir nepareizi iestatījumi vai nepietiekamas atļaujas, lai veiktu sinhronizēšanu.</span><span class="sxs-lookup"><span data-stu-id="8ca8b-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="8ca8b-104">AADConnect atkārtota instalēšana, izmantojot ekspresiestatījumus, var ātri atrisināt šo problēmu:</span><span class="sxs-lookup"><span data-stu-id="8ca8b-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="8ca8b-105">[Lejupielādējiet jaunāko AADConnect versiju](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="8ca8b-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="8ca8b-106">[Izpildiet norādījumus saistībā ar izteiktu instalēšanu](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="8ca8b-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="8ca8b-107">Papildinformāciju par AADConnect pakalpojumu kontiem skatiet rakstā [AZURE ad Connect: konti un atļaujas](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="8ca8b-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
