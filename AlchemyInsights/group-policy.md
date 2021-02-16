---
title: Grupas politika
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256780"
---
# <a name="group-policy"></a>Grupas politika

Lietotāja un datora objektu iestatījumi Azure Active Directory domēna pakalpojumos (Azure AD DS) bieži tiek pārvaldīti, izmantojot grupas politikas objektus (GPO). Azure AD DS ir iebūvēts GPO AADDC lietotājiem un AADDC datoru konteineriem. Šos iebūvētos GPO varat pielāgot, lai pēc vajadzības konfigurētu grupas politiku. Azure AD DC administratoru grupas dalībniekiem ir grupas politikas administrēšanas privilēģijas Azure AD DS domēnā, kā arī var izveidot pielāgotus GPO un organizācijas vienības (OU). Papildinformāciju par grupas politiku un to, kā tas darbojas, skatiet sadaļā [grupas politikas pārskats](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

Hibrīdajā vidē grupu politikas, kas konfigurētas lokālajā AD DS vidē, netiek sinhronizētas ar Azure AD DS. Lai definētu konfigurācijas iestatījumus lietotājiem vai datoriem Azure AD DS, rediģējiet kādu no noklusējuma GPO vai izveidojiet pielāgotu GPO.

Šajā rakstā [grupas politikas pārvaldība](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) ir parādīts, kā instalēt grupas politikas pārvaldības rīkus, kā ton rediģēt iebūvētos GPO un kā izveidot pielāgotus GPO.



