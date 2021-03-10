---
title: Nomnieka politikas labošana (darbības ignorēšana)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694060"
---
# <a name="fix-tenant-policy-action-override"></a>Nomnieka politikas labošana (darbības ignorēšana)

Šis ziņojums ietekmēja jūsu nomnieka pretsurogātpasta politiku. Lai pārskatītu politiku, veiciet tālāk norādītās darbības.

1. Dodieties uz [Office 365 drošības & atbilstības centru](https://go.microsoft.com/fwlink/p/?linkid=2077143)un pēc tam dodieties uz **Threat Management**  >  **Policy**  >  [anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Pārbaudiet, vai **politikas avots** norāda šādu informāciju:  **Add-Xheader/ModifySubject/redirect/DELETE/bez darbības/diskrētās kopijas ziņojums**

    Ja tā ir, cilnē **pielāgot** atzīmējiet tās politikas iestatījumus, kas ietekmēja šo ziņojumu. Iespējams, ka **standarta iestatījumi** ir lietoti visiem Exchange Online aizsardzības klientiem, kas ietekmējuši šo ziņojumu.

Papildinformāciju par surogātpasta filtrēšanas politiku konfigurēšanu skatiet rakstā [surogātpasta filtrēšanas politiku konfigurēšana](https://go.microsoft.com/fwlink/?linkid=2101431).
