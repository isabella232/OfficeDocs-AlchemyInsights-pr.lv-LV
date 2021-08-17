---
title: Replicēt kopu
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 45cf530c3258fa3c7008c3e8251fdb7b74be6911d0487f58c5ce2530e25ca282
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54110687"
---
# <a name="replica-set"></a>Replicēt kopu

AADDS tiek dēvēts arī par pārvaldīto domēnu. Faktiski aizmugurguri tiek palaisti un uzturēti divi domēna kontrolleri. Divos DC ir viena galvenā DC un viena replicēšana DC. Dublējumi AADDS (pārvaldītais domēns) ir automatizēts process, ko pārvalda Azure platforma. Ja rodas problēma ar jūsu pārvaldīto domēnu, Azure atbalsts var palīdzēt atjaunot no dublējuma.

Katra dublikāta kopa tiek izveidota virtuālajā tīklā. Katram virtuālajam tīklam ir jābūt vienādranga katram virtuālajam tīklam, kas vieso pārvaldītā domēna dublikāta kopu. Šī konfigurācija izveido režģa tīkla topoloģiju, kas atbalsta direktorija replicēšanu. Virtuālais tīkls var atbalstīt vairākas dublikātu kopas, ja katra dublikāta kopa atrodas citā virtuālajā apakštīklā.

Papildinformāciju par replicēto kopu skatiet [rakstā Koncepcijas replicēt kopas.](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)
