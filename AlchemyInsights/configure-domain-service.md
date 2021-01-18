---
title: Domēna pakalpojuma konfigurēšana
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885682"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a>Nevar iespējot AAD-DS vai izvietošanas kļūmi

Lai atrisinātu Azure AD Domain Service (AAD-DS) problēmu, kas nav iespējota vai netiek izvietota, veiciet tālāk norādītās darbības.

1. Ja izmantojat jau esošu virtuālo tīklu, atzīmējiet savu NSG, lai iegūtu kārtulas, kas bloķē portus, kas nepieciešami, lai sinhronizētu ar AAD-DS portālā https://aka.ms/aadds-networking .
2. Pārbaudiet, vai jūsu kļūdas ziņojums ir atbildēts šajā rakstā pieejamā problēmu novēršanas rokasgrāmatā  https://aka.ms/aadds-troubleshoot-enable .
3. Izmēģiniet Azure AD Domain pakalpojumu izvietošanu jaunā virtuālajā tīklā.
4. Izpildiet darba sākšanas rokasgrāmatu par to, kā izvietot AAD-DS: [izveidot un konfigurēt AAD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Ja rodas problēmas saistībā ar Azure AD domēna pakalpojumu izvietošanu, skatiet rakstu [AZURE ad Domain Services problēmu novēršana](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) , lai atrisinātu Biežākās kļūdas, kas palīdzēs paveikt darbu atkārtoti. 

**Nevar atspējot AAD-DS**

AAD-DS nevar pauzēt. Ja vēlaties pārtraukt pārvaldītā domēna izmantošanu, tas ir jādzēš.
Lai dzēstu pārvaldīto domēnu, skatiet rakstu [AAD Domain Service DELETE](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).



