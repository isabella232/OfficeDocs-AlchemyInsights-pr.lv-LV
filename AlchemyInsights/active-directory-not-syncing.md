---
title: Active Directory nav sinhronizēšana
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265202"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="e0b5c-102">Active Directory nav sinhronizēšana</span><span class="sxs-lookup"><span data-stu-id="e0b5c-102">Active Directory not syncing</span></span>

<span data-ttu-id="e0b5c-103">Ja saņemat sinhronizācijas kļūdas, piemēram, "nav nesenās sinhronizācijas" vai paziņojumu direktorija sinhronizēšana statusu Office administrēšanas portāls saka "Pēdējoreiz sinhronizēts vairāk nekā 3 dienas pirms", iespējams, ka AADConnect ir nepareizi iestatījumi vai nepietiekams atļauju, lai veiktu sinhronizāciju.</span><span class="sxs-lookup"><span data-stu-id="e0b5c-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="e0b5c-104">Pārinstalēt AADConnect, izmantojot ekspresiestatījumus var atrisināt šo problēmu ātri:</span><span class="sxs-lookup"><span data-stu-id="e0b5c-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="e0b5c-105">[Lejupielādēt jaunāko AADConnect versiju](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="e0b5c-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="e0b5c-106">[Izpildiet tiešas instalēšanas instrukcijas](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="e0b5c-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="e0b5c-107">Lai iegūtu papildinformāciju par AADConnect pakalpojuma kontu, skatiet [AZURE ad Connect: konti un atļaujas](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="e0b5c-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
