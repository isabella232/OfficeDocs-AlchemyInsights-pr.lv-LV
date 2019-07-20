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
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800458"
---
# <a name="no-results-from-content-searchexports"></a>Nekādi rezultāti no satura meklēšanas/eksports

Problēmas ar satura meklēšanas/eksports nav atgriežot datus var izraisīt noteiktu atbilstību drošības filtrs, kas bija setup īpašas Admin un nav to paziņot visiem Admins.

Lai atrisinātu šo problēmu, pārbaudiet, lai redzētu, vai pastāv atbilstība drošības filtrus, kas izraisa šo:
1. Drošības un atbilstības centrā Powershell savienojumu
2. Palaist šādu commandlets:
<br>$org = "yourdomain.com"
<br>Iegūt ComplianceSecurityFilter-organizācija $org