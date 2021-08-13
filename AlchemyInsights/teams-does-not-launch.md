---
title: Teams netiek palaista
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/4/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12673"
- "9007646"
ms.openlocfilehash: a37f980e700090da8199c703216af6f04f4aca464c21870beb3e907dd7b2d491
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813351"
---
# <a name="teams-doesnt-launch"></a>Teams netiek palaista

Ja mēģināt atvērt programmu Microsoft Teams taču tā nekad netiek palaista, izmēģiniet tālāk norādītās darbības.

1. Pārlūkojiet **līdz %appdata%\Microsoft\Teams.**
1. Dzēsiet mapes saturu.
1. Restartējiet datoru un mēģiniet palaist Teams.

Iespējams, būs atkārtoti jāinstalē Teams. Lai atkārtoti instalētu:

1. Atinstalējiet Teams, izmantojot vadības paneli.
1. Pārlūkojiet **līdz %appdata%\Microsoft\Teams\Application Cache.**
1. Dzēsiet mapes saturu.
1. Pārlūkojiet **līdz %appdata%\Microsoft\teams\Cache.**
1. Dzēsiet mapes saturu.
1. Restartējiet datoru un pēc tam lejupielādējiet un instalējiet Teams.

Ja nomniekam vēlaties veikt diagnostiku konkrētam lietotājam, kurš nevar pierakstīties, sāciet jaunu meklēšanu ar atslēgvārdu **TeamsUserUnableToSignIn** un izpildiet norādījumus.