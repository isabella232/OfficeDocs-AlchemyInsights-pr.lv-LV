---
title: Ierobežotas piekļuves pārraudzība
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708681"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Ierobežotas piekļuves Exchange pārraudzība

Lietotāji, kuru mērķis ir ierobežotas piekļuves tiesības, saņem paziņojumu e-pasta ziņojumu, ja tie neatbilst jūsu organizācijas piekļuves prasībām. Lai atrisinātu šo problēmu, iesakām vienu vai vairākus no šiem risinājumiem:

- Ja ierīce ir uzskatāma par piereģistrētu, informējiet lietotāju, ka esat pieteicies uzņēmuma portāla programmā, un pārbaudiet, vai tā ir redzama uzņēmuma portālā. Ja tā nav, lietotājam ir jāreģistrē ierīce.
- Azure portālā dodieties uz Intune > ierīces atbilstība. Sadaļā Monitora noklikšķiniet uz ierīces atbilstība. Skatīt ierīces atbilstības atskaiti, lai pārliecinātos, vai lietotāja ierīce ir atzīmēta kā atbilstoša.
- Azure portālā dodieties uz Intune > ierīces atbilstība. Sadaļā pārvaldība noklikšķiniet uz politikas. Atbilstības politiku sarakstā pārbaudiet, vai profils ir piešķirts jūsu lietotāja ierīcei. Ja nav piešķirts neviens profils, Intune nevarēs apstiprināt ierīces atbilstības statusu.
- Rediģējiet lietotāja nosacījuma piekļuves uzdevumu.

1. Azure portālā dodieties uz **Intune**  >  **ierobežotas piekļuves**  >  **politikām**.
2. Sarakstā atlasiet politiku.
3. Noklikšķiniet uz lietotāji un grupas.
4. Lai noteiktu konkrētu politiku, pievienojiet to sarakstam iekļaut. Lai nodrošinātu to, ka politika nav izlaista, pievienojiet tās sarakstam neiekļaut.

Noderīgas saites:

[Ierīces atbilstības pārskats](https://docs.microsoft.com/intune/device-compliance-get-started)

[Problēmu novēršana CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Problēmu novēršanas politika](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Intune ierīces atbilstības pārraudzība](https://docs.microsoft.com/intune/compliance-policy-monitor)

Piezīme: šīs darbības ir noderīgas tikai pakalpojuma Azure Active Directory līdzekļu problēmu novēršanai. Varat arī karantīnā ievietot ierīci, lai bloķētu e-pasta piekļuvi ar Exchange politiku. Plašāku informāciju par Exchange ierīču pārvaldību var atrast [šeit] ( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
