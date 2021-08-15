---
title: Dažādu portu piekļuves problēmu diagnostika
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 07c108d5292965d20340da039b67744d93c0a4fc61edb8115796671f2f7f1552
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030909"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Dažādu portu piekļuves problēmu diagnostika

Lai novērstu dažādas ar piekļuvi portiem saistītas problēmas, veiciet tālāk norādītās darbības.

1. Apturiet/nodaliet virtuālo mašīnu (VM) no portāla, restartējiet virtuālo mašīnu un pārbaudiet vēlreiz. 
2. Pārbaudiet sava VM tīkla iestatījumus, lai noteiktu, vai jums ir tīkla drošības grupas (NSG) trafika bloķēšana. Varat arī [](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) izmantot tīkla skatīšanās IP plūsmas pārbaudes rīku, lai pārbaudītu, vai NSG bloķē trafiku, User-Defined Maršruti (UDR) pāradresē jūsu trafiku atpakaļ uz lokālo ("Noklusējuma maršruts" 0.0.0.0/0) vai uz tīkla iekārtu.
Ja pēc iepriekš minēto darbību izmēģinīšanas joprojām rodas problēmas, lūdzu, norādiet VM nosaukumu un TCP portu, kurā mēģināt nosūtīt e-pastu, lai uz to papildinformāciju piedāvātu.

**Ieteiktie dokumenti**

[Ierobežojumi un ieteikumi izejošā e-pasta sūtīšanai pa portu 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)