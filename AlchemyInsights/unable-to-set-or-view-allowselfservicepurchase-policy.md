---
title: Nevar iestatīt vai skatīt AllowSelfServicePurchase politiku
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
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735206"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Nevar iestatīt vai skatīt AllowSelfServicePurchase politiku

Mēģinot iestatīt vai skatīt AllowSelfServicePurchase politiku, tiek parādīts šāds kļūdas ziņojums:

*HandleError: neizdevās izgūt produkta politiku ar PolicyId ' AllowSelfServicePurchase ', ErrorMessage-galvenais savienojums ir aizvērts: sūtot radās neparedzēta kļūda.*

Iespējams, tas skaidrojams ar vecāku transporta slāņa drošības (TLS) versiju. Lai izveidotu savienojumu ar MSCommerce pakalpojumu, ir jāizmanto TLS 1,2 vai jaunāka versija.  

Izmēģiniet tālāk norādītās darbības, lai iespējotu/iestatītu TLS protokolu 1,2, pārbaudiet un mēģiniet vēlreiz.
 1. PowerShell komandu uzvedne (PS C: ievadiet šo \) komandu, lai IESTATĪTU TLS protokolu versijai 1,2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Pārbaudiet lietotos TLS protokolus ar šādu komandu:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Pēc nepieciešamības atkārtoti mēģiniet iegūt vai atjaunināt komandas.

