---
title: Satura meklēšana rezultāti
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516786"
---
# <a name="no-results-from-content-searchexports"></a>Nekādi rezultāti no satura meklēšanas/eksports

Problēmas ar satura meklēšanas/eksports nav atgriežot datus var izraisīt noteiktu atbilstību drošības filtrs, kas bija setup īpašas Admin un nav to paziņot visiem Admins.

Lai atrisinātu šo problēmu, pārbaudiet, lai redzētu, vai pastāv atbilstība drošības filtrus, kas izraisa šo:
1. Drošības un atbilstības centrā Powershell savienojumu
2. Palaist šādu commandlets:
<br>$org = "yourdomain.com"
<br>Iegūt ComplianceSecurityFilter-organizācija $org