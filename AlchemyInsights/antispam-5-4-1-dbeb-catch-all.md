---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: e0e9b4fec0615943227f40043aeed842e8ee556c5916a59f65e79ce121ec9547
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932284"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Piegādes problēmu (kļūdas kods 550 5.4.1 pārraide liegta) novēršana

Šī problēma rodas, [pārbaudot, vai](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) e-pasta adrese ir derīga, lai novērstu atlēcienu rādīšanu Microsoft tīklā. Veiciet tālāk norādītās darbības.

1. Nosakiet, vai problēma ir raksturīga visam domēnam vai vienai e-pasta adresei:
    - Viss domēns: dažreiz domēns ir jāsinhronizē; mēģiniet [iestatīt domēnu uz Iekšējs un pēc tam atpakaļ uz Autoritatīvs](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Viena e-pasta adrese: dažreiz adrese ir jāsinhronizē; smtp starpniekservera adreses maiņa un pēc tam atpakaļadreses maiņa var palīdzēt.
2. Nosakiet, vai problēma ir specifiska grupai vai publiskai mapei. Dažiem objektu tipiem objektus var būt nepieciešams manuāli izveidot Azure Active Directory.

Ja jums nepieciešama papildu palīdzība, lūdzu, atveriet atbalsta biļeti un norādiet problēmas tvērumu (tostarp tā objekta veidu, uz kuru nosūtāt), lai mēs varētu jums palīdzēt labāk.