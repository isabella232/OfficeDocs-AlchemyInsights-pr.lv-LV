---
title: Dublikātu kopa
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
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714250"
---
# <a name="replica-set"></a>Dublikātu kopa

AADDS tiek dēvēts arī par pārvaldīto domēnu. Faktiski tie ir divi domēnu kontrolleri, kurus vada un ko uztur backend. Divi DCs ietilpst viens galvenais DC un viens replicēšanas KONTROLLERis. Dublējumkopijas pakalpojumā AADDS (Managed Domain) ir automatizēts process, ko pārvalda Azure Platform. Ja rodas problēmas ar jūsu pārvaldīto domēnu, Azure atbalsts var palīdzēt veikt atjaunošanu no dublējuma.

Jūs izveidojat katru dublikātu kopu virtuālajā tīklā. Katrs virtuālais tīkls ir jāvienādranga visos citos virtuālajos tīklos, kas vieso pārvaldītā domēna dublikātu kopu. Šī konfigurācija izveido Mesh tīkla topoloģiju, kas atbalsta direktorija replicēšanu. Virtuālais tīkls var atbalstīt vairākas dublikātu kopas, ja katra dublikātu kopa ir citā virtuālajā apakštīklā.

Detalizētu informāciju par dublikātu kopu skatiet rakstā [jēdzienu dublikātu kopas](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).
