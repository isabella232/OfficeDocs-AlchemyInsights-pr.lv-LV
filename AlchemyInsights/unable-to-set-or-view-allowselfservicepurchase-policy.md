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
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091730"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Nevar iestatīt vai skatīt AllowSelfServicePurchase politiku

Mēģinot iestatīt vai skatīt AllowSelfServicePurchase politiku, tiek parādīts šāds kļūdas ziņojums:

*HandleError: neizdevās izgūt produktu politika ar PolicyId "AllowSelfServicePurchase" ErrorMessage-pamata savienojums tika aizvērts: radās neparedzēta kļūda nosūtīt.*

Tas var būt saistīts ar vecākas versijas transporta slāņa drošība (TLS). Lai savienotu MSCommerce pakalpojumu, ir jāizmanto TLS 1,2 vai jaunāka versija.  

Izmēģiniet tālāk aprakstītās darbības, lai iespējotu/iestatītu TLS protokolu 1,2, pārbaudiet un mēģiniet vēlreiz.
 1. PowerShell komandu uzvednē (PS C:\) ievadiet šādu komandu, lai iestatītu TLS protokola versija 1,2:

    \[NET. ServicePointManager]:: SecurityProtocol = \[net. SecurityProtocolType]:: Tls12

2. Pārbaudiet, vai TLS protokolu (s) lietošanā, ar šādu komandu:

    \[NET. ServicePointManager]:: SecurityProtocol 

3. Ja nepieciešams, vēlreiz mēģiniet iegūt vai atjaunināt komandas.

