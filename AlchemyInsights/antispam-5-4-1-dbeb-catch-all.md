---
title: Pretsurogātpasta 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717368"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Piegādes problēmu novēršana kļūdas kodam 550 5.4.1 relay piekļuvei

Šī problēma rodas, [pārbaudot, vai e-pasta adrese ir derīga, lai neļautu bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) , kad ievadāt Microsoft tīklu. Izmēģiniet kādu no tālāk norādītajām darbībām.

1. Noteikt, vai problēma ir saistīta ar visu domēnu vai vienu e-pasta adresi:
    - Viss domēns: dažreiz domēns ir jāsinhronizē. mēģiniet [Iestatīt domēnu uz iekšējs un pēc tam atpakaļ uz autoritatīvo](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Viena e-pasta adrese: dažreiz adrese ir jāsinhronizē. var palīdzēt mainīt SMTP starpniekservera adresi un pēc tam to mainīt atpakaļ.
2. Noteikt, vai problēma ir specifiska grupai vai publiskai mapei. Dažiem objektu veidiem objekti, iespējams, ir manuāli jāveido Azure Active Directory.

Ja jums ir vajadzīgas papildu palīdzība, lūdzu, atveriet atbalsta biļeti un norādiet problēmas apjomu (ieskaitot tā objekta tipu, ko sūtāt), lai mēs varētu jums palīdzēt labāk.