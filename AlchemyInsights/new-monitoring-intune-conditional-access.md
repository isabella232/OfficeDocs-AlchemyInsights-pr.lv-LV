---
title: Intune ierobežotas piekļuves pārraudzība
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
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427922"
---
# <a name="monitor-intune-conditional-access"></a>Intune ierobežotas piekļuves pārraudzība

Lietotāji, kuru mērķis ir ierobežotas piekļuves tiesības, saņem paziņojumu e-pasta ziņojumu, ja tie neatbilst jūsu organizācijas piekļuves prasībām. Lai atrisinātu šo problēmu, iesakām vienu vai vairākus no šiem risinājumiem:

1. Ja ierīce ir uzskatāma par piereģistrētu, informējiet lietotāju, ka esat pieteicies uzņēmuma portāla programmā, un pārbaudiet, vai tā ir redzama uzņēmuma portālā. Ja tā nav, lietotājam ir jāreģistrē ierīce.
1. Azure portālā dodieties uz **Intune**  >  **ierīces atbilstība**. 
1. Lai skatītu ierīces atbilstības atskaiti, lai pārliecinātos, vai lietotāja ierīce ir atzīmēta kā atbilstoša, sadaļā **monitors** noklikšķiniet uz **ierīces atbilstība**.
1. Azure portālā dodieties uz **Intune**  >  **ierīces atbilstība**. Sadaļā **pārvaldība** noklikšķiniet uz **politikas**. Atbilstības politiku sarakstā pārbaudiet, vai profils ir piešķirts jūsu lietotāja ierīcei. Ja nav piešķirts neviens profils, Intune nevarēs apstiprināt ierīces atbilstības statusu.
1. Rediģējiet lietotāja nosacījuma piekļuves uzdevumu.
1. Azure portālā pārejiet uz **Intune**  >  **nosacījuma piekļuves**  >  **politikām**, sarakstā atlasiet politiku un noklikšķiniet uz **lietotāji un grupas**.
1. Lai noteiktu konkrētu politiku, pievienojiet to **sarakstam iekļaut**. Lai nodrošinātu to, ka politika nav izlaista, pievienojiet tās **sarakstam neiekļaut**.

**Noderīgas saites:**

- [Ierīces atbilstības pārskats](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Problēmu novēršana CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Problēmu novēršanas politika](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Intune ierīces atbilstības pārraudzība](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> Šīs darbības ir noderīgas tikai pakalpojuma Azure Active Directory līdzekļu problēmu novēršanai. Varat arī karantīnā ievietot ierīci, lai bloķētu e-pasta piekļuvi ar Exchange politiku. Papildinformāciju par Exchange ierīču pārvaldību [**skatiet šeit**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).
