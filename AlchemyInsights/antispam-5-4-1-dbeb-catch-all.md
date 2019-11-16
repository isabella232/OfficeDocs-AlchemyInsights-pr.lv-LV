---
title: AntiSpam 5.4.1 DBEB catch-visi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: 4f531a063d63aff239ef7dead869bb526e17fb35
ms.sourcegitcommit: 2591e1f56e8943bddb9d3b77ba5b494ac49d4f30
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 11/15/2019
ms.locfileid: "38672440"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Izlabojiet kļūdas kods piegādes problēmas 550 5.4.1 relay piekļuve liegta

Šī problēma rodas, [pārbaudot, lai redzētu, vai e-pasta adrese ir derīga, lai novērstu atgriešanu](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) , ievadot Office 365 tīklā. Mēģiniet veikt šādas darbības:

1. Nosakiet, vai problēma ir specifiska visam domēnam vai vienai e-pasta adresei:
    - Viss domēns: dažreiz domēns ir jāsinhronizē; mēģiniet [Iestatīt domēnu uz iekšējo un pēc tam atpakaļ uz autoritatīvu](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Viena e-pasta adrese: dažreiz adrese ir jāsinhronizē; mainot SMTP starpniekservera adrese un pēc tam mainot to atpakaļ var palīdzēt.
2. Nosakiet, vai problēma ir saistīta ar grupu vai publisko mapi. Dažiem objektu tipiem objekti, iespējams, ir jāizveido manuāli pakalpojumā Azure Active Directory.

Ja jums nepieciešama papildu palīdzība, lūdzu, atveriet atbalsta biļeti un norādiet problēmas tvērumu (includidng objekta veidu, uz kuru sūtāt ziņojumu), lai mēs varētu jums palīdzēt labāk.