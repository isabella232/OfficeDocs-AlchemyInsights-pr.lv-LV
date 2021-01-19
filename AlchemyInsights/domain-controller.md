---
title: Domēna kontrolleris
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901027"
---
# <a name="domain-controller"></a>Domēna kontrolleris

**Nevar iespējot AAD-DS vai izvietošanas kļūmi**

Lai atrisinātu Azure AD Domain Service (AAD-DS) problēmu, kas nav iespējota vai netiek izvietota, veiciet tālāk norādītās darbības.

1. Ja izmantojat jau esošu virtuālo tīklu, atzīmējiet savu NSG, lai iegūtu kārtulas, kas bloķē portus, kas nepieciešami, lai sinhronizētu ar AAD-DS portālā https://aka.ms/aadds-networking .
2. Pārbaudiet, vai jūsu kļūdas ziņojums ir atbildēts šajā rakstā pieejamā problēmu novēršanas rokasgrāmatā  https://aka.ms/aadds-troubleshoot-enable .
3. Izmēģiniet Azure AD Domain pakalpojumu izvietošanu jaunā virtuālajā tīklā.
4. Izpildiet darba sākšanas instrukciju par to, kā izvietot AAD-DS, kas ir pieejams [apmācība AZURE ad Domain pakalpojumu izveidei](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Ja rodas problēmas saistībā ar Azure AD domēna pakalpojumu izvietošanu, skatiet rakstu [AZURE ad Domain Services problēmu novēršana](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) , lai atrisinātu Biežākās kļūdas, kas palīdzēs paveikt darbu atkārtoti. 

**Nevar atspējot AAD-DS**

AAD-DS nevar pauzēt. Ja vēlaties pārtraukt pārvaldītā domēna izmantošanu, tas ir jādzēš.

Ja rodas problēmas, lai atrisinātu biežāk sastopamos kļūdu ziņojumus un saistītu problēmu novēršanas darbības, lai palīdzētu atkal sākt darbu, skatiet rakstu [Azure Active Directory domēna pakalpojumu problēmu novēršana](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).
