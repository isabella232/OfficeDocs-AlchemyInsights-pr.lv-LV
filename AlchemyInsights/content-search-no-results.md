---
title: Satura meklēšana bez rezultātiem
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
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680654"
---
# <a name="no-results-from-content-searchexports"></a>Nav rezultātu no satura meklēšanas/eksportēšanas

Problēmas saistībā ar satura meklēšanu/eksportēšanu, kas neatgriež datus, var būt saistīti ar noteiktu atbilstības drošības filtru, ko iestatīja konkrēts administrators un kas to nedara visiem administratoriem.

Lai atrisinātu šo problēmu, pārbaudiet, vai pastāv atbilstības drošības filtri, kas var izraisīt šādu situāciju:
1. Savienojuma izveide ar drošības un atbilstības centra PowerShell
2. Palaidiet šādu commandlets:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-Organization $org