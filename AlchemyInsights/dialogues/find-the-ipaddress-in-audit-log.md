---
title: IP adreses atrašana audita žurnālfailā
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429783"
---
# <a name="find-the-ip-address-in-audit-log"></a>IP adreses atrašana audita žurnālfailā

1. Audita žurnālos tiek parādīta tā IP adrese, kas atbilst lietotāja vai administratora veiktajai darbībai. Tiek reģistrēta arī klienta informācija. Lai noteiktu IP adresi, rīkojieties šādi:

1. Dodieties uz [Office 365 drošības & atbilstības centru](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Atlasiet **meklēšanas**  >  **[audita žurnālu meklēšana](https://go.microsoft.com/fwlink/?linkid=2103759)**.
    > [!NOTE]
    > Ja redzat paziņojumu par to, ka ir jāieslēdz auditēšana, pārejiet uz priekšu un ieslēdziet to tūlīt. Ja šis līdzeklis nav iespējots, meklēšanas rezultātos nevarēs paņemt datus no iepriekšējiem datumiem.
1. Ja esat ieinteresēts noteiktā aktivitātē, atlasiet to sarakstā **aktivitātes** . Pretējā gadījumā pēc noklusējuma visi darbi tiks atgriezti atlasītajam lietotājam. Ņemiet vērā, ka noteiktas darbības, iespējams, nav pieejamas atlases veikšanai izvēlnē **darbības** . taču šie audita vienumi tiek atgriezti, ja ir atlasīts **Rādīt rezultātus visām darbībām** (noklusējuma iestatījums).
1. Norādiet datumu diapazonu un laukā **lietotāji** atlasiet tā lietotāja lietotājvārdu, kuru vēlaties izpētīt.
1. Atlasiet **Meklēt**. Darbības būs redzamas sadaļā **rezultāti**. Katrai darbībai varat redzēt IP adresi.
1. Lai skatītu detalizētu informāciju, atlasiet aktivitāti un pēc tam atlasiet **Papildinformācija**.

Lai uzzinātu vairāk, skatiet rakstu meklēšana [Office 365 audita žurnālu, lai novērstu raksturīgākos scenārijus](https://go.microsoft.com/fwlink/?linkid=2103944).