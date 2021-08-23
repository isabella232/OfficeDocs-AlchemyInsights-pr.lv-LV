---
title: Netiek Outlook etiķetes noklusējuma iestatījums
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000181"
- "13259"
ms.openlocfilehash: 84284554151586ff0a22f983d9494f59b4675f92
ms.sourcegitcommit: 4b92c2648ddba3ad3bc61a22771c59ed5fc76303
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/17/2021
ms.locfileid: "58454751"
---
# <a name="default-outlook-label-setting-not-applied"></a>Netiek Outlook etiķetes noklusējuma iestatījums

Ja Outlook noklusējuma etiķetes iestatījumi netiek lietoti pareizi un tiek lietota cita etiķete vai etiķete netiek lietota, iespējams, ir radusies zināma problēma (MC277818) un ir jāizmanto kāda no šīm 2 opcijām, lai novērstu problēmu.

**1. iespēja.**

1. Dodieties uz Microsoft 365 atbilstības centru >   >  **Informācijas aizsardzība.**
1. Atlasiet **Uzlīmju politikas** un atlasiet jums rediģējamās uzlīmju politikas (**OutlookDefaultlabel** iestatījums nav pareizi iestatīts uz etiķetes politikas jautājumu. Lai **skatītu šo iestatījumu, palaidiet get-labelpolicy** un pēc tam atlasiet **Rediģēt politiku**.
1. Atlasiet **Tālāk,** līdz tiek parādīts **iestatījums** Lietot šo noklusējuma etiķeti e-pasta ziņojumiem, kas ir pieejams, ja dialoglodziņā Politikas iestatījumi atlasāt Pieprasīt lietotājiem lietot etiķeti heir e-pasta ziņojumiem un dokumentiem.  
1. Dialoglodziņā **Noklusējuma etiķetes pievienošana dokumentiem** nolaižamajā **sarakstā** izvēlieties Nav.
1. Atlasiet **Tālāk un** **Iesniegt,** lai saglabātu uzlīmes iestatījumus.

**2. iespēja.**

Drošības un atbilstības centra [Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell?view=exchange-ps)izmantojiet komandsīklietotni Set-LabelPolicy lai **mainītu OutlookDefaultlabel** uz **Nav** {OutlookDefaultLabel="None"}.

Palaišana: `Set-LabelPolicy -Identity [policy] -AdvancedSettings @{OutlookDefaultLabel="None"}`

Papildinformāciju par noklusējuma uzlīmēm Outlook skatiet [rakstā Citas noklusējuma etiķetes iestatīšana Outlook.](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide-customizations#set-a-different-default-label-for-outlook)