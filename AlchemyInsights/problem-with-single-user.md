---
title: Problēma ar vienu lietotāju
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
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430199"
---
# <a name="problem-with-single-user"></a>Problēma ar vienu lietotāju

- Lietotājs, iespējams, nav nodrošināts, jo pakalpojums vēl nav bijis izdevies novērtēt lietotāju. Pārskatiet norādījumus par to, kā ilgtermiņā tiek nodrošināts, kā arī norises josla lapā nodrošināšanas konfigurācija. Ja sadaļā Papildu dati norādītā stabilā stāvokļa vērtība ir pirms lietotāja izveides/atjaunināšanas/dzēšanas, tas nozīmē, ka vēl neesat izvērtējis lietotāju. Šajā scenārijā vislabākā darbība ir gaidīt, līdz tiek pabeigts nodrošināšanas pakalpojums.

  - Ņemiet vērā, ka mūsu pakalpojumi ir tikai informēti par izmaiņām lietotāja avota sistēmā (mākoņa stundā). Azure AD avota sistēmā ir jābūt derīgām izmaiņām, lai noteiktu izmaiņas un to ieplūstošu Active Directory.
- Nodrošināšanas pakalpojums novērtēja lietotāju un noteica, ka tas nav nodrošināts:
  - Ja esat iestatījis atribūtu, kura pamatā ir tvērums, pārliecinieties, vai lietotājs atbilst norādītajiem kritērijiem.
  - Ja lietotāji jau ir mērķa sistēmā un lietotāja stāvoklis avota un mērķa atbilstībā, mēs neveicam nekādas papildu darbības.
- Nodrošināšanas pakalpojums mēģināja nodrošināt lietotāju un tas neizdevās. Šos scenārijus skatiet nodrošināšanas žurnālu cilne problēmu novēršana un ieteikumi.
  - Lokālā Active Directory vai Azure AD, iespējams, trūkst nepieciešama lietotāja atribūta. Piemēram, userPrincipalName vai sAMAccountName ģenerēšanas kārtulas nerada pareizo vērtību.
  - Atbilstošais atribūts (parasti employeeId) nav atrisināts ar unikālu lietotāju lokālajā Active Directory vai Azure AD. Piemēram, ir divi lietotāji ar vienu un to pašu employeeId AD un pakalpojums atgriež kļūdas kodu, kas norāda tā paša avota ieraksta dublikātus.

Lai pārskatītu viena lietotāja un grupu žurnālus, skatiet rakstu [nodrošināšanas žurnālu pārskatīšana, lai iegūtu problēmu ar konkrētu lietotāju](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).
