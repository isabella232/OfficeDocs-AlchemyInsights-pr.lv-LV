---
title: Workday līdz AD user Provisioning pāriet karantīnā
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 32a5d010b95b9587e121ca1526def743fd8f371b13d1d73d3578c692839edf19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036499"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Workday līdz AD user Provisioning pāriet karantīnā

**AD lietotāju nodrošināšanas darba diena tiek ievietots karantīnā un lietotāji netiek veidoti AD**

Ad lietotāju nodrošināšanas darba diena ir pāriet karantīnā, un audita žurnālos tiek rādīti eksportēšanas kļūmju notikumi ar kļūdas ziņojumu **Kļūda: OperationsError-SvcErr: Radās operācijas kļūda. Direktorija pakalpojumam nav konfigurēta neviena izcila atsauce. Tādējādi direktorija pakalpojums nevar sniegt atsauces uz objektiem ārpus šī meža.** Šī kļūda parasti tiek parādīta, ja Active Directory konteinera ou nav pareizi iestatīts vai ja pastāv problēmas ar izteiksmju kartējumu, kas izmantots **parentDistinguishedName**.

Pārbaudiet, vai parametrā Noklusējuma OU **jauniem lietotājiem** nav kļūdu. Pārliecinieties, vai norādītais OU jau pastāv jūsu AD. Ja izmantojat **parentDistinguishedName** atribūtu kartēšanā, pārliecinieties, vai tas vienmēr tiek novērtēts kā zināms konteiners AD domēnā. Pārbaudiet eksportēšanas notikumu audita žurnālos, lai skatītu ģenerēto vērtību.

Papildinformāciju par automātiskās nodrošināšanas darba dienas konfigurēšanu skatiet rakstā Apmācība: darba [dienas konfigurēšana automātiskai lietotāju nodrošināšana.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)

