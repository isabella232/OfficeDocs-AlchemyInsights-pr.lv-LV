---
title: GPO izvietošana
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: 6f9e164713ce36023de954d45031fd4414780e174bf5c7741c4aec274a65b32e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54067847"
---
# <a name="gpo-deployment"></a>GPO izvietošana

Iestatījumi un datoru objekti pakalpojumā Azure Active Directory (Azure AD DS) bieži tiek pārvaldīti, izmantojot grupas politikas objektus (GpOs). Azure AD DS ietver iebūvētu GPOS AADDC lietotājiem un AADDC computers konteineriem. Varat pielāgot šo iebūvēto GPOS, lai konfigurētu grupas politiku pēc nepieciešamības savā vidē. Azure AD DC administratoru grupas dalībniekiem ir grupas politikas administrēšanas privilēģijas Azure AD DS domēnā, un viņi var arī izveidot pielāgotas GPOS un organizācijas vienības (OU). Papildinformāciju par to, kas ir grupas politika un kā tā darbojas, skatiet rakstā [Grupas politikas pārskats.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

Hibrīdajā vidē grupas politikas, kas konfigurētas lokālajā AD DS vidē, netiek sinhronizētas ar Azure AD DS. Lai definētu konfigurācijas iestatījumus lietotājiem vai datoriem programmā Azure AD DS, rediģējiet kādu no noklusējuma GPOS vai izveidojiet pielāgotu GPO.

Šajā rakstā [Grupas politikas pārvaldība](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) parādīts, kā instalēt grupas politikas pārvaldības rīkus, kā rediģēt iebūvēto GPOS un kā izveidot pielāgotu GPOS.
