---
title: Teams 4c7 kļūda
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: ea3e8f23c07103e604fc6b264047582b9c3e26b6b73237adc30eba574e06cfd3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049315"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c7 kļūda Microsoft Teams

Šī kļūda rodas tāpēc, Microsoft Teams nepieciešama Forms Authentication. Kad izvietojat Active Directory federācijas pakalpojumu (AD FS), veidlapu autentifikācija pēc noklusējuma nav iespējota iekštīklam. Ja Windows autentifikācija neizdodas, jums tiek piedāvāts pierakstīties, izmantojot veidlapu autentifikāciju.

Lai novērstu šo problēmu, iespējojiet Forms Authentication, izmantojot AD FS Microsoft Management Console (MMC) papildprogrammu datorā, kurā ir lokālā Active Directory kopija. Lai to izdarītu, veiciet tālāk norādītās darbības. 

1. Navigācijas rūtī pārlūkojiet līdz **Autentifikācijas politikas**.
2. Sadaļas Darbības detalizētas informācijas rūtī atlasiet **Rediģēt globālo primāro autentifikāciju**. 
3. Cilnē **Iekštīkls** atlasiet Forms **Authentication**.
4. Atlasiet **Labi** (vai **Lietot**).