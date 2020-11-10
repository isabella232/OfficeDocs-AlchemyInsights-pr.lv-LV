---
title: OneDrive pieteikšanās kļūdas AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982482"
---
# <a name="onedrive-login-error-aadsts50011"></a>OneDrive pieteikšanās kļūdas AADSTS50011

Ja saņemat kļūdas ziņojumu "AADSTS50011: pieprasījumā norādītais atbildes vietrādis URL neatbilst atbildei", kad pierakstāties lietojumprogrammā OneDrive, pārbaudiet, vai:

Jūsu OneDrive versijai ir jābūt vienādai vai lielākai par versiju 20.052. XXXX. XXXX. Lai pārbaudītu savu versiju, paziņojumu apgabalā noklikšķiniet uz zilās OneDrive ikonas, atlasiet **palīdzības & iestatījumi > iestatījumi > par**.

Jūsu tīkls var bloķēt trafiku uz **g.Live.com** un **oneclient.SFX.MS**. Ja šī satiksme ir bloķēta, OneDrive nevar veikt atjaunināšanu. Strādājiet ar tīkla administratoru, lai nodrošinātu piekļuvi šiem vietrāžiem URL. [Šiem galapunktiem](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) jāsasniedz klienti, kas izmanto Microsoft 365 plānus.

Ja jums ir manuāli jāiegūst pašreizējā OneDrive versija, apmeklējiet vietni [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
