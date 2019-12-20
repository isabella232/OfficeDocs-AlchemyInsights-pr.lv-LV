---
title: Teams 4C 7 kļūda
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796232"
---
# <a name="4c7-error-in-microsoft-teams"></a>4C 7 kļūda Microsoft Teams

Šī kļūda rodas tāpēc, ka Microsoft Teams nepieciešama veidlapu autentifikācija. Ieviešot Active Directory Federācijas pakalpojums (AD FS), veidlapu autentifikācija nav iekštīkla pēc noklusējuma nav iespējots. Ja Windows integrētā autentifikācija neizdodas, tiek piedāvāts pierakstīties, izmantojot veidlapu autentifikācija.

Lai novērstu šo problēmu, iespējojiet veidlapu autentifikācija, izmantojot AD FS Microsoft pārvaldības konsoles (MMC) papildprogrammu datorā, kurā ir Active Directory lokālo kopiju. Lai to izdarītu, veiciet tālāk norādītās darbības. 

1. Navigācijas rūtī atrodiet **autentifikācijas politikas**.
2. Detalizētās informācijas rūts sadaļā **darbības** atlasiet **Rediģēt globālo primāro autentifikāciju**.
3. Cilnē **iekštīkla** atlasiet **veidlapu autentifikācija**.
4. Atlasiet **Labi** (vai **lietot**).