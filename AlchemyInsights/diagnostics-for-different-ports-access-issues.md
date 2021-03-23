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
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035780"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Dažādu portu piekļuves problēmu diagnostika

Lai atrisinātu dažādas portu piekļuves problēmas, veiciet tālāk norādītās darbības.

1. Apturēt/depiešķirt virtuālo mašīnu (VM) no portāla, restartējiet VM un testējiet vēlreiz. 
2. Pārbaudiet sava VM tīkla iestatījumus, lai noteiktu, vai jums ir tīkla drošības grupu (NSGs) bloķēšanas trafiks. Varat arī izmantot [tīkla uzrauga IP plūsmas pārbaudes rīku](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) , lai meklētu NSGs bloķēšanas trafiku, User-Defined maršrutus (UDRs) atkārtoti maršrutējiet savu trafiku atpakaļ uz lokālo ("noklusējuma maršruts" 0.0.0.0/0) vai uz tīkla ierīci.
Ja pēc šo darbību veikšanas joprojām rodas problēmas, lūdzu, norādiet VM nosaukumu un TCP portu, no kura mēģināt nosūtīt e-pasta ziņojumu, lai saņemtu turpmāku diagnozi.

**Ieteiktie dokumenti**

[Ierobežojumi un ieteikumi par izejošā e-pasta nosūtīšanu, salīdzinot ar portu 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)