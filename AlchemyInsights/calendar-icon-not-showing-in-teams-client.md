---
title: Kalendāra ikona netiek rādīta Teams klientā
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 21692639fb746b2e5aab3dfc8894293d5dc890ac
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932202"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>Kalendāra ikona netiek rādīta Teams klientā

Cilnei Kalendārs pakalpojumā Teams ir nepieciešama piekļuve Exchange pastkastei, izmantojot Exchange tīmekļa pakalpojumus. Exchange pastkaste var būt tiešsaistē vai lokāli. Tiešsaistes lietotājiem, kuri neredz cilni Kalendārs, jāpārliecinās, vai viņiem [ir licence Exchange Online pastkastei un vai pastkaste ir iespējota](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

Ja lietotājam ir derīga pastkaste pakalpojumā Exchange Online, bet viņš joprojām neredz cilni Kalendārs, iespējams, radušās tīkla problēmas. Izmantojiet [Microsoft attālā savienojuma analizētāju](https://testconnectivity.microsoft.com/) un palaidiet ietekmētajam lietotājam paredzētās **Microsoft Exchange tīmekļa pakalpojumu savienojuma pārbaudes**.

Visbeidzot pārbaudiet [Teams programmas — programmu iestatīšanas politikas](https://admin.teams.microsoft.com/policies/app-setup), lai nodrošinātu, ka lietojumprogramma Kalendārs nav noņemta no lietotājam piemērotās politikas (visdrīzāk **Globālā (organizācijas līmeņa noklusējums)**.

Ja jūsu lietotāji izmanto lokālo versiju, jums jāpārliecinās, vai hibrīdā konfigurācija ir darbspējīga. Izmantojiet [hibrīdās konfigurācijas vedni](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent), lai novērstu problēmas.

Ņemiet vērā, ka [pakalpojumam Teams nepieciešams Exchange 2016 CU3 vai jaunāka tā versija](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
