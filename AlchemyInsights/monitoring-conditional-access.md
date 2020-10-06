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
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366435"
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

[Problēmu novēršanas politika](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[Intune ierīces atbilstības pārraudzība](https://docs.microsoft.com/intune/compliance-policy-monitor)

Piezīme: šīs darbības ir noderīgas tikai pakalpojuma Azure Active Directory līdzekļu problēmu novēršanai. Varat arī karantīnā ievietot ierīci, lai bloķētu e-pasta piekļuvi ar Exchange politiku. Papildinformāciju par Exchange ierīču pārvaldību [skatiet šeit](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).
