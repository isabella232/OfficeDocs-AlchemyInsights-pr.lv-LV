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
ms.openlocfilehash: e1ad34e8a5cefe168b86727ac3ca208d90f8d4478696cef58a7d0b04475fba56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003396"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Mantoto dialogu iegulšanas iespējošana, lai atvērtu atskaites

**Simptoms**

Lietotāji nevar atvērt atskaites. “Radās kāda kļūme. Lai iegūtu papildinformāciju, skatiet tehnisko detalizēto informāciju.”

**Iemesls**

Atskaites neizdodas ielādēt UCI, jo rodas kļūda “Veidlapas deskriptors ir Null vai nav definēts”. UCI atskaitēm joprojām ir nepieciešami mantoti dialogi, tāpēc klienta sistēmā ir jābūt iespējotai opcijai *legacydialogsembedding*.

**Risinājums**

1. Dodieties uz **Iestatījumi >Administrēšana > Sistēmas iestatījumi > cilne Vispārīgi**.

2. Iestatiet opcijas “Iespējot noteiktu mantoto dialogu iegulšanu vienotā interfeisa pārlūkprogrammas klientā” vērtību **Jā**.
