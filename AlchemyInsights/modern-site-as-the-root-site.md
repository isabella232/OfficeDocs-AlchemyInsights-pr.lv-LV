---
title: Mūsdienu vietni kā saknes vietni
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: d5ea73c967013822854dbd408d4628d991c90378
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620766"
---
# <a name="modern-site-as-root-site"></a>Mūsdienu vietni kā saknes

Mēs esam sākuši izvēršana jauns līdzeklis, kas ļaus apmainīties ar klasisko vietnes saknes vietne, ar mūsdienu vietā. Izmantot [Izsaukums SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) swap atrašanās vietu ar citu vietā vienlaikus arhivē sākotnējā vietā. Pieejama gan darba grupas vietni (nav pievienots grupai) un saziņas vietne. 

>[!Important]
> Klasisks saknes vietne, lai izveidotu mūsdienīgu saziņas vietne nevar dzēst. Šī korporācija Microsoft to neatbalsta. Saknes vietnes dzēšana padarīs visas SharePoint vietnes organizācijā nepieejama visiem lietotājiem, kamēr vietā atjaunot vai izveidot jaunu vietni ar tādu pašu URL. Mums būs sazināties šo iespēju, izmantojot ziņu centru. Iespēja ieslēgt savu īrnieka drīzumā vajadzētu sagaidīt.

## <a name="known-issues-with-swapping-sites"></a>Zināmas problēmas ar apmainīšana vietām
- Mērķa vietnes var atgriezt "nav atrasts" kļūda (HTTP 404) uz neilgu laika periodu.
- Saturs būs nepieciešams recrawled atjaunināt meklēšanas indeksā. Tur ir bez manuālas darbības, kāda vajadzīga šeit, tas tiks veikts automātiski.
- Viss atkarīgs no "statisku" saites (piemēram, failu sinhronizēšana un OneNote failus) vajadzēs manuāli jālabo.
- Project Server vietņu, iespējams, tiks pārbaudīti, vai tie ir joprojām saistīts pareizi. 
