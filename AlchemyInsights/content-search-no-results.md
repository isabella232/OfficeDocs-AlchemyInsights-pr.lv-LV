---
title: Satura meklēšana nav rezultātu
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
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816855"
---
# <a name="no-results-from-content-searchexports"></a>Nav rezultātu no satura meklēšanas/eksportēšanas

Problēmas ar satura meklēšanu/eksportēšanu neatgriež nekādus datus, iespējams, izraisa konkrēts administrators iestatīts atbilstības drošības filtrs, kas netika darīts zināmu visiem administratoriem.

Lai novērstu šo problēmu, pārbaudiet, vai ir kāds atbilstības drošības filtrs, kas varētu izraisīt šo problēmu:
1. Savienojuma izveide ar drošības un atbilstības centra Powershell
2. Palaidiet šādus komandsīklietotņus:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter organizācijas $org