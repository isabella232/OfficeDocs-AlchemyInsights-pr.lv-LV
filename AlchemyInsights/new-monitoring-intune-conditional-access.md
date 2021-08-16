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
ms.openlocfilehash: 7f30202ff0a5b9475393cf26c0506bd6bec24f3d378052f24ebf7f327cf84689
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54025509"
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

> [!NOTE]
> Šīs darbības ir noderīgas tikai, lai novērstu līdzekļa Azure Active Directory nosacījuma piekļuvi. Ir iespējams arī karantīnā ievietot ierīci, kas bloķē tās piekļuvi e-pastam, izmantojot Exchange politiku. Papildinformāciju par Exchange pārvaldību skatiet [**šeit.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))
