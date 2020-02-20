---
title: Nevar iestatīt vai skatīt AllowSelfServicePurchase politiku
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158568"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Nevar iestatīt vai skatīt AllowSelfServicePurchase politiku

Mēģinot iestatīt vai skatīt AllowSelfServicePurchase politiku, tiek parādīts šāds kļūdas ziņojums:

*HandleError: neizdevās izgūt produktu politika ar PolicyId "AllowSelfServicePurchase" ErrorMessage-pamata savienojums tika aizvērts: radās neparedzēta kļūda nosūtīt.*

Tas var būt saistīts ar vecākas versijas transporta slāņa drošība (TLS). Lai savienotu MSCommerce pakalpojumu, ir jāizmanto TLS 1,2 vai jaunāka versija.  

Izmēģiniet tālāk aprakstītās darbības, lai iespējotu/iestatītu TLS protokolu 1,2, pārbaudiet un mēģiniet vēlreiz.
 1. PowerShell komandu uzvednē (PS C:\) ievadiet šādu komandu, lai iestatītu TLS protokola versija 1,2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Pārbaudiet, vai TLS protokolu (s) lietošanā, ar šādu komandu:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Ja nepieciešams, vēlreiz mēģiniet iegūt vai atjaunināt komandas.

