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
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821454"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Piegādes problēmu (kļūdas kods 550 5.4.1 pārraide liegta) novēršana

Šī problēma rodas, [pārbaudot, vai](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) e-pasta adrese ir derīga, lai novērstu atlēcienu rādīšanu Microsoft tīklā. Veiciet tālāk norādītās darbības.

1. Nosakiet, vai problēma ir raksturīga visam domēnam vai vienai e-pasta adresei:
    - Viss domēns: dažreiz domēns ir jāsinhronizē; mēģiniet [iestatīt domēnu uz Iekšējs un pēc tam atpakaļ uz Autoritatīvs](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Viena e-pasta adrese: dažreiz adrese ir jāsinhronizē; smtp starpniekservera adreses maiņa un pēc tam atpakaļadreses maiņa var palīdzēt.
2. Nosakiet, vai problēma ir specifiska grupai vai publiskai mapei. Dažu objektu tipu gadījumā objektus var būt nepieciešams manuāli izveidot pakalpojumā Azure Active Directory.

Ja jums nepieciešama papildu palīdzība, lūdzu, atveriet atbalsta biļeti un norādiet problēmas tvērumu (tostarp tā objekta veidu, uz kuru nosūtāt), lai mēs varētu jums palīdzēt labāk.