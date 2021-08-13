---
title: Lietotāju nodrošināšana
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
ms.openlocfilehash: 12490df735ca8c524058404df92db79c6c5682fe2ecafe2b42baed70fa3ab142
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971346"
---
# <a name="user-provisioning"></a>Lietotāju nodrošināšana

- Izmantojiet pēc [pieprasījuma nodrošināšanas iespēju, lai](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) nodrošinātu lietotāju un iegūtu detalizētu diagnostiku par veiktajiem soļiem.
- Lai novērstu problēmas, ar kurām sastopaties, norādot lietotājus un grupas, skatiet problēmu novēršanas [rokasgrāmatu.](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned)
- Ja novērots, ka lietotāji netiek nodrošināti, skatiet rakstu Nodrošināšanas [žurnāli (priekšskatījums)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) programmā Azure Active Directory (AD). Meklējiet žurnāla ierakstus, kas attiecas uz konkrētu lietotāju.
- Periodiski restartējiet nodrošināšanu, lai apskatītu lietotājus, kas netika palaisti iepriekšējā nodrošināšanas ciklā.
- Lietotājs/grupa var nebūt nodrošināta, jo mūsu pakalpojumam vēl nav bijusi iespēja novērtēt lietotāju. Pārskatiet norādījumus par to, cik ilgi notiek nodrošināšana, kā arī nodrošināšanas konfigurācijas lapas norises joslu. Ja nemainīgais stāvoklis, kas norādīts papildinformācijas sadaļā, ir pirms lietotāja izveides/atjaunināšanas/dzēšanas datuma, tas nozīmē, ka lietotājs vēl nav novērtēts. Šajā scenārijā vislabāk ir gaidīt, līdz tiek pabeigts nodrošināšanas pakalpojums. Ja stabilais stāvoklis ir sasniegts, iesakām veikt restartēšanu no Lietotāja interfeisa Azure portālā.
  - Ņemiet vērā, ka mūsu pakalpojums ir informēts tikai par lietotāja/grupas izmaiņām avota sistēmā (Azure Active Directory). Ja lietotājs/grupa tiek noņemts tieši lietojumprogrammā (piemēram, ServiceNow), mēs zinām par šīm izmaiņām un to neatritinām, ņemot vērā lietotāja stāvokli avota sistēmā. Šajā scenārijā vislabāk atritiniet izmaiņas tieši mērķa lietojumprogrammā.
- Mūsu pakalpojums izvērtēja lietotāju/grupu un nolēma, ka tas nav jānodrošina:
  - Ja esat iestatījis tvērumu kā piešķirtos lietotājus un grupas, pārbaudiet, vai lietojumprogrammai ir piešķirts lietotājs/grupa.
  - Ja lietojumprogrammai ir piešķirts lietotājs/grupa, pārliecinieties, vai tam nav piešķirta noklusējuma piekļuves loma. Šo lomu nevar izmantot nodrošināšana.
  - Ja esat iestatījis atribūtu tvēruma noteikšanai, pārliecinieties, vai lietotājs atbilst jūsu norādītajiem kritērijiem.
  - Ja lietotāji jau pastāv mērķa sistēmā un lietotāja stāvokli avotā un mērķa atbilstības līmenī, mēs tālāk nesācām veikt nekādas darbības.
- Mūsu pakalpojums mēģināja nodrošināt lietotāju, un tas neizdevās. Šādā gadījumā skatiet problēmu novēršanas un ieteikumu cilni nodrošināšanas žurnālos:
  - Iespējams, trūkst nepieciešamā atribūta lietotāja lietojumprogrammā Azure Active Directory vai tas neatbilst trešās puses lietojumprogrammas pieprasītam formātam. Piemēram, atribūts Valsts/valstij lietotājam var būt iestatīts uz Amerikas Savienotajām Valstīm, ja tam ir jābūt ASV.
  - Atribūts ir attiecinošs atribūts, kas mērķa lietojumprogrammā vēl nepastāv. Attiecinošā atribūts ir atribūts, kas norāda uz citu objektu, piemēram, lietotāju, kurš ir grupas dalībnieks. Lietotāja ID būs grupas dalībnieka atribūtā, bet to var apstrādāt tikai tad, ja lietotāja objekts, uz kuru tas norāda, jau pastāv.
