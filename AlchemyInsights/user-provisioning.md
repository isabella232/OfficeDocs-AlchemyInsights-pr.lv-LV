---
title: Lietotāju nodrošinājums
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004348"
- "8428"
ms.openlocfilehash: bd415b2d44bccf0c2b3eccb4e38452498b748b3a
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481887"
---
# <a name="user-provisioning"></a>Lietotāju nodrošinājums

- Izmantojiet pēc [pieprasījuma nodrošināšanas](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) iespējas, lai nodrošinātu lietotājam un iegūtu detalizētu diagnostiku par veiktajām darbībām.
- Lai novērstu problēmas, kas rodas, [nodrošinot lietotāju un](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned)grupu nodrošināšanu, skatiet problēmu novēršanas norādījumus.
- Ja ievērojat, ka lietotāji netiek nodrošināti, skatiet rakstu pakalpojuma Azure Active Directory (AD) [nodrošināšanas žurnāli (priekšskatījums)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) . Meklējiet reģistrācijas ierakstus, kas attiecas uz noteiktu lietotāju.
- Periodiski atsāciet nodrošināšanu, lai noķertu lietotājus, kuru iepriekšējais nodrošināšanas cikls ir nokavēts.
- Lietotājs/grupa, iespējams, nav nodrošināta, jo mūsu pakalpojumam vēl nav bijusi iespēja šo lietotāju novērtēt. Pārskatiet norādījumus par to, kā ilgtermiņā tiek nodrošināts, kā arī norises josla lapā nodrošināšanas konfigurācija. Ja sadaļā Papildu dati norādītā stabilā stāvokļa vērtība ir pirms lietotāja izveides/atjaunināšanas/dzēšanas, tas nozīmē, ka vēl neesat izvērtējis lietotāju. Šajā scenārijā vislabākā darbība ir gaidīt, līdz tiek pabeigts nodrošināšanas pakalpojums. Ja vienmērīgā stāvoklī ir sasniegts, iesakām veikt restartēšanu no lietotāja interfeisa Azure portālā.
  - Ņemiet vērā, ka mūsu pakalpojums ir tikai informēts par izmaiņām lietotāja/grupas avota sistēmā (Azure Active Directory). Ja lietotājs/grupa tiek noņemta tieši lietojumprogrammā (piemēram, ServiceNow), mēs neesam informēti par šīm izmaiņām un neveicu atgriešanos, pamatojoties uz lietotāja stāvokli avota sistēmā. Šajā scenārijā ieteicams veikt izmaiņas tieši atritināt vajadzīgajā lietojumprogrammā.
- Mūsu pakalpojums novērtēja lietotāju/grupu un noteica, ka tā nav nodrošināta.
  - Ja esat iestatījis tvērumu Piešķirtie lietotāji un grupas, pārbaudiet, vai lietotājam/grupai ir piešķirta programma.
  - Ja lietojumprogrammai ir piešķirta lietotājam/grupai, pārliecinieties, vai tie nav piešķirti noklusējuma piekļuves lomai. Šo lomu nevar izmantot nodrošinājuma nodrošināšanai.
  - Ja esat iestatījis atribūtu, kura pamatā ir tvērums, pārliecinieties, vai lietotājs atbilst norādītajiem kritērijiem.
  - Ja lietotāji jau ir mērķa sistēmā un lietotāja stāvoklis avota un mērķa atbilstībā, mēs neveicam nekādas papildu darbības.
- Mūsu pakalpojums mēģināja nodrošināt lietotāju un tas neizdevās. Šos scenārijus skatiet nodrošināšanas žurnālu cilne problēmu novēršana un ieteikumi.
  - Pakalpojumā Azure Active Directory var trūkt obligāts lietotāja atribūts vai tas neatbilst formātam, ko pieprasa trešās puses lietojumprogramma. Piemēram, valsts atribūts lietotājam var būt iestatīts uz United States, ja tas ir mums.
  - Atribūts ir atsauces atribūts, kas vēl nepastāv Target lietojumprogrammā. Attiecinošais atribūts ir atribūts, kas norāda uz citu objektu, piemēram, lietotājs, kas ir grupas dalībnieks. Lietotāja ID būtu grupas dalībnieka atribūtā, bet to var apstrādāt tikai tad, ja lietotāja objekts norāda uz jau esošu.
