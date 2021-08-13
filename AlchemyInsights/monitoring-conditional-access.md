---
title: Nosacījum piekļuves pārraudzība
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
ms.openlocfilehash: 80e8cc72db8ae32445d48e5c8a411d5ccd538626653260b3dbd28a247561e888
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975108"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Nosacījum piekļuves pārraudzība Exchange

Lietotāji, kas tiek paredzēti nosacījum piekļuves saņemšanai, saņem paziņojuma e-pasta ziņojumu, ja tie neatbilst jūsu organizācijas piekļuves prasībām. Lai novērstu šo problēmu, iesakām vienu vai vairākus no šiem risinājumiem:

- Ja tiek pieņemts, ka ierīce ir reģistrēta, iesakiet lietotājam doties uz Company Portal un pārbaudīt, vai tā ir redzama Company Portal. Ja tā nav, lietotājam ierīce ir jāreģistrē.
- Azure portālā dodieties uz Intune un > atbilstību. Sadaļā Pārraugs noklikšķiniet uz Ierīces atbilstība. Skatiet savu ierīču atbilstības atskaiti, lai pārbaudītu, vai lietotāja ierīce ir atzīmēta kā atbilstošs.
- Azure portālā dodieties uz Intune un > atbilstību. Sadaļā Pārvaldība noklikšķiniet uz Politikas. Atbilstības politiku sarakstā pārliecinieties, vai lietotāja ierīcei ir piešķirts profils. Ja neviens profils nav piešķirts, Tad Intune nevar apstiprināt ierīces atbilstības statusu.
- Rediģējiet lietotāja nosacījumiekļuves piešķiri.

1. Azure portālā dodieties uz **Intune nosacījum**  >  **piekļuves**  >  **politikas**.
2. Sarakstā atlasiet politiku.
3. Noklikšķiniet uz Lietotāji un grupas.
4. Lai noteiktu politiku rādīšanu uz kādu lietotāju, pievienojiet to sarakstā Iekļaut. Lai nodrošinātu, ka persona netiek iekļauts politikā, pievienojiet to izslēgšanas sarakstam.

Noderīgas saites:

[Ierīces atbilstības pārskats](https://docs.microsoft.com/intune/device-compliance-get-started)

[Problēmu novēršana CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Problēmu novēršanas politika](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Intune ierīču atbilstības pārraudzība](https://docs.microsoft.com/intune/compliance-policy-monitor)

Piezīme. Šīs darbības ir noderīgas tikai, lai novērstu līdzekļa Azure Active Directory nosacījuma piekļuvi. Ir iespējams arī karantīnā ievietot ierīci, kas bloķē tās piekļuvi e-pastam, izmantojot Exchange politiku. Papildinformāciju par Exchange pārvaldību skatiet [šeit]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
