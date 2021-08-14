---
title: Kalendāra ikona netiek rādīta Teams klientā
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 7881d6837cb7d99180d2cc1b28d327ce12e4b836d33e4fca099569d4f72510fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989598"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>Kalendāra ikona netiek rādīta Teams klientā

Cilnei Kalendārs pakalpojumā Teams ir nepieciešama piekļuve Exchange pastkastei, izmantojot Exchange tīmekļa pakalpojumus. Exchange pastkaste var būt tiešsaistē vai lokāli. Tiešsaistes lietotājiem, kuri neredz cilni Kalendārs, jāpārliecinās, vai viņiem [ir Exchange Online pastkastes licence un vai pastkaste ir iespējota](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

Ja lietotājam ir derīga pastkaste pakalpojumā Exchange Online, bet viņš joprojām neredz cilni Kalendārs, iespējams, radušās tīkla problēmas. Izmantojiet [Microsoft attālās savienojamības analizētāju](https://testconnectivity.microsoft.com/) un palaidiet ietekmētajam lietotājam paredzētās **Microsoft Exchange tīmekļa pakalpojumu savienojamības pārbaudes**.

Visbeidzot pārbaudiet [Teams programmas — programmu iestatīšanas politikas](https://admin.teams.microsoft.com/policies/app-setup), lai nodrošinātu, ka programma Kalendārs nav noņemta no lietotājam piemērotās politikas (visdrīzāk **Globālā (organizācijas līmeņa noklusējums)**).

Ja jūsu lietotāji izmanto lokālo versiju, jums jāpārliecinās, vai hibrīdā konfigurācija ir darbspējīga. Izmantojiet [hibrīdās konfigurācijas vedni](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent), lai novērstu problēmas.

Ņemiet vērā, ka [pakalpojumam Teams nepieciešams Exchange 2016 CU3 vai jaunāka tā versija](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
