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
ms.openlocfilehash: 8d8821cda94b2af244fa317707421f9d197b6052fb316789cd286ea8b4adf19e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960158"
---
# <a name="problem-with-single-user"></a>Problēma ar vienu lietotāju

- Lietotājs, iespējams, nav nodrošināts, jo pakalpojumam vēl nav bijusi iespēja novērtēt lietotāju. Pārskatiet norādījumus par to, cik ilgi notiek nodrošināšana, kā arī nodrošināšanas konfigurācijas lapas norises joslu. Ja nemainīgais stāvoklis, kas norādīts papildinformācijas sadaļā, ir pirms lietotāja izveides/atjaunināšanas/dzēšanas datuma, tas nozīmē, ka lietotājs vēl nav novērtēts. Šajā scenārijā vislabāk ir gaidīt, līdz tiek pabeigts nodrošināšanas pakalpojums.

  - Ņemiet vērā, ka mūsu pakalpojums ir informēts tikai par izmaiņām, kas veiktas lietotājam avota sistēmā (Cloud HR). Ir jāveic derīgas izmaiņas avota sistēmā, lai Azure AD noteiktu izmaiņas un to plūsmu pakalpojumā Active Directory.
- Nodrošināšanas pakalpojums novērtēja lietotāju un nolēma, ka tas nav jānodrošina:
  - Ja esat iestatījis atribūtu tvēruma noteikšanai, pārliecinieties, vai lietotājs atbilst jūsu norādītajiem kritērijiem.
  - Ja lietotāji jau pastāv mērķa sistēmā un lietotāja stāvokli avotā un mērķa atbilstības līmenī, mēs tālāk nesācām veikt nekādas darbības.
- Nodrošināšanas pakalpojums mēģināja nodrošināt lietotāju, un tas neizdevās. Šādā gadījumā skatiet problēmu novēršanas un ieteikumu cilni nodrošināšanas žurnālos:
  - Iespējams, lokālajā Active Directory vai Azure AD lietotājam trūkst nepieciešamā atribūta. Piemēram, userPrincipalName vai sAMAccountName ģenerēšanas kārtulas neveido pareizo vērtību.
  - Atbilstošais atribūts (parasti employeeId) nav atrisināms unikālam lietotājam lokālajā Active Directory vai Azure AD. Piemēram, ad ir divi lietotāji ar vienādu employeeId un pakalpojums atgriež kļūdas kodu, kas norāda mērķa ierakstu dublikātus tam pašam avota ierakstam.

Lai pārskatītu žurnālus atsevišķam lietotājam un grupām, skatiet rakstu Konkrēta lietotāja [problēmas nodrošināšanas žurnālu pārskatīšana.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)
