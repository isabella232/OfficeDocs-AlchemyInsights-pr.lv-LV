---
title: Pārvaldīt sinhronizētu lietotāju
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
- "9000609"
- "2444"
ms.openlocfilehash: 0dc2ecfa0bb5703c619dc1b2d6b4d517f999da0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823974"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="f5245-102">Nevar iestatīt primāro e-pasta adresi, mainīt lietotāja atribūtus vai noņemt/dzēst sinhronizētu lietotāju</span><span class="sxs-lookup"><span data-stu-id="f5245-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="f5245-103">Ja jūsu vidē ir iespējota direktorija sinhronizēšana, dažus lietotāja vai objekta atribūtus nevar mainīt, izmantojot Microsoft 365 administrēšanas centru.</span><span class="sxs-lookup"><span data-stu-id="f5245-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="f5245-104">Lai pilnībā pārvaldītu sinhronizētos lietotājus un visus to atribūtus, izmantojiet lokālos Active Directory lietotājus un grupu pārvaldības konsoli (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="f5245-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="f5245-105">Varat mainīt arī atsevišķus lietotājus vai atribūtus sinhronizētiem lietotājiem, kuri izmanto powershell, kā parādīts šajos bieži izmantotajos piemēros:</span><span class="sxs-lookup"><span data-stu-id="f5245-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span>

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
