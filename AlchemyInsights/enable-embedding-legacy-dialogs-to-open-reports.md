---
title: Mantoto dialogu iegulšanas iespējošana, lai atvērtu atskaites
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814271"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Mantoto dialogu iegulšanas iespējošana, lai atvērtu atskaites

**Simptoms**

Lietotāji nevar atvērt atskaites. “Radās kāda kļūme. Lai iegūtu papildinformāciju, skatiet tehnisko detalizēto informāciju.”

**Iemesls**

Atskaites neizdodas ielādēt UCI, jo rodas kļūda “Veidlapas deskriptors ir Null vai nav definēts”. UCI atskaitēm joprojām ir nepieciešami mantoti dialogi, tāpēc klienta sistēmā ir jābūt iespējotai opcijai *legacydialogsembedding*.

**Risinājums**

1. Dodieties uz **Iestatījumi >Administrēšana > Sistēmas iestatījumi > cilne Vispārīgi**.

2. Iestatiet opcijas “Iespējot noteiktu mantoto dialogu iegulšanu vienotā interfeisa pārlūkprogrammas klientā” vērtību **Jā**.
