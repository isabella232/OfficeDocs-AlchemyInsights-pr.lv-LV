---
title: Funkcija WORKDAY uz AD lietotāju nodrošināšanu nonāk karantīnas stāvoklī
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
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481878"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Funkcija WORKDAY uz AD lietotāju nodrošināšanu nonāk karantīnas stāvoklī

**Funkcija WORKDAY uz AD lietotāju nodrošināšanu tiek pārveidota par karantīnas stāvokli, bet REKLĀMā netiek izveidots neviens lietotājs**

Darba sākšana ar reklāmas lietotāju nodrošināšanas darbu ir izdevusies karantīnas stāvoklī, un audita žurnālos tiek rādīts kļūdas ziņojuma **kļūdas ziņojums: OperationsError-SvcErr: radās darbības kļūda. Nav konfigurēta neviena vadītāja atsauce direktoriju pakalpojumam. Direktoriju pakalpojums tāpēc nevar sniegt norādes objektiem ārpus šī meža**. Šī kļūda parasti tiek rādīta, ja Active Directory konteiners OU nav iestatīts pareizi vai pastāv problēmas ar **ParentDistinguishedName** izteiksmju kartēšanu.

Pārbaudiet noklusējuma OU **jauniem lietotājiem** parametru typos. Pārliecinieties, vai jūsu REKLĀMā jau ir norādīta norādītā OU. Ja izmantojat **parentDistinguishedName** atribūtu kartē, pārliecinieties, vai tas vienmēr tiek novērtēts uz zināmo konteineru ad domēnā. Pārbaudiet eksportēšanas notikumu audita žurnālos, lai redzētu ģenerēto vērtību.

Lai iegūtu papildinformāciju par to, kā konfigurēt darba dienu automatizētai konfigurēšanai, skatiet rakstu [apmācība: darbdienas konfigurēšana automātiskai lietotāju nodrošināšanai](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).

