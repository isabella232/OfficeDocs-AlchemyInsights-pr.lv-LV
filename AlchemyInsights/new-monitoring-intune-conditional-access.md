---
title: Intune nosacījum piekļuves pārraudzība
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: 2c3a382671ac95ecbaec1b374bd8c474cf9690a2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327564"
---
# <a name="monitor-intune-conditional-access"></a>Intune nosacījum piekļuves pārraudzība

Lietotāji, kas tiek paredzēti nosacījum piekļuves saņemšanai, saņem paziņojuma e-pasta ziņojumu, ja tie neatbilst jūsu organizācijas piekļuves prasībām. Lai novērstu šo problēmu, iesakām vienu vai vairākus no šiem risinājumiem:

1. Ja tiek pieņemts, ka ierīce ir reģistrēta, iesakiet lietotājam doties uz Company Portal un pārbaudīt, vai tā ir redzama Company Portal. Ja tā nav, lietotājam ierīce ir jāreģistrē.
1. Azure portālā dodieties uz **Intune**  >  **ierīču atbilstība**. 
1. Lai skatītu savu ierīču atbilstības atskaiti un pārbaudītu, vai lietotāja ierīce ir atzīmēta kā atbilstošs, sadaļā **Pārraugs** noklikšķiniet uz **Ierīces atbilstība**.
1. Azure portālā dodieties uz **Intune**  >  **ierīču atbilstība**. Sadaļā **Pārvaldība noklikšķiniet** uz **Politikas.** Atbilstības politiku sarakstā pārliecinieties, vai lietotāja ierīcei ir piešķirts profils. Ja neviens profils nav piešķirts, Tad Intune nevar apstiprināt ierīces atbilstības statusu.
1. Rediģējiet lietotāja nosacījumiekļuves piešķiri.
1. Azure portālā naviģējiet uz **Intune nosacījum** piekļuves politikas , sarakstā atlasiet politiku un  >    >  noklikšķiniet uz **Lietotāji un grupas**.
1. Lai noteiktu politiku rādīšanu uz kādu lietotāju, pievienojiet to **sarakstā Iekļaut.** Lai nodrošinātu, ka persona netiek iekļauts politikā, pievienojiet to **izslēgšanas sarakstam.**

**Noderīgas saites:**

- [Ierīces atbilstības pārskats](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Problēmu novēršana CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Problēmu novēršanas politika](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Intune ierīču atbilstības pārraudzība](https://docs.microsoft.com/intune/compliance-policy-monitor)

**Piezīme.** Šīs darbības ir noderīgas tikai, lai novērstu līdzekļa Azure Active Directory nosacījuma piekļuvi. Ir iespējams arī karantīnā ievietot ierīci, kas bloķē tās piekļuvi e-pastam, Exchange politiku. Papildinformāciju par Exchange pārvaldību skatiet [**šeit.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))
