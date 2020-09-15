---
title: Teams 4c7 kļūda
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
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700210"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c7 kļūda pakalpojumā Microsoft Teams

Šī kļūda rodas tādēļ, ka programmai Microsoft Teams ir nepieciešama veidlapu autentifikācija. Kad izvietojat Active Directory Federācijas pakalpojumu (AD FS), pēc noklusējuma iekštīklam nav iespējota veidlapu autentifikācija. Ja Windows integrētā autentifikācija rodas nesekmīga, saņemsit aicinājumu pierakstīties, izmantojot veidlapu autentifikāciju.

Lai atrisinātu šo problēmu, iespējojiet veidlapu autentifikāciju, izmantojot AD FS Microsoft pārvaldības konsoles (MMC) papildprogramma datorā, kurā ir lokālā Active Directory kopija. Lai to izdarītu, veiciet tālāk norādītās darbības. 

1. Navigācijas rūtī pārlūkojiet līdz **autentificēšanas politikas**.
2. Detalizētās informācijas rūts sadaļā **darbības** atlasiet **Rediģēt globālo primāro autentifikāciju**.
3. Cilnē **iekštīkls** atlasiet **veidlapu autentifikācija**.
4. Atlasiet **Labi** (vai **lietot**).