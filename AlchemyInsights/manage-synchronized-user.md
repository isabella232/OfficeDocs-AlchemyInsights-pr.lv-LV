---
title: Sinhronizētā lietotāja pārvaldība
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
- "9000609"
- "2444"
ms.openlocfilehash: 7bf7d3f00308ff6bc973cd52e09ca51c5fd0f45b
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 10/13/2020
ms.locfileid: "48451407"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Nevar iestatīt primāro e-pasta adresi, mainīt lietotāja atribūtus vai noņemt/dzēst sinhronizētu lietotāju

Ja jūsu videi ir iespējota direktorija sinhronizēšana, dažus lietotāju vai objektu atribūtus nevar mainīt, izmantojot Microsoft 365 administrēšanas centru.

Lai pilnībā pārvaldītu sinhronizētos lietotājus un to atribūtus, izmantojiet lokālo Active Directory lietotāju un grupu pārvaldības konsoli (ADSIEDIT. msc).  

Varat arī mainīt atsevišķus lietotājus vai atribūtus sinhronizētiem lietotājiem, izmantojot PowerShell, piemēram, kā parādīts šajos vispārīgajos piemēros:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
