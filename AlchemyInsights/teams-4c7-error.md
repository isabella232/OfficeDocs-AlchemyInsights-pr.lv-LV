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
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786676"
---
# <a name="4c7-error-in-microsoft-teams"></a>Kļūda 4c7 lietojumprogrammā Microsoft Teams

Šī kļūda rodas tāpēc, ka Microsoft Teams pieprasa veidlapu autentifikāciju. Kad izvietojat Active Directory federācijas pakalpojumu (AD FS), veidlapu autentifikācija pēc noklusējuma nav iespējota iekštīklam. Ja Windows integrētā autentifikācija neizdodas, jums tiek piedāvāts pierakstīties, izmantojot veidlapu autentifikāciju.

Lai novērstu šo problēmu, iespējojiet Forms Authentication, izmantojot AD FS Microsoft Management Console (MMC) papildprogrammu datorā, kurā ir lokālā Active Directory kopija. Lai to izdarītu, veiciet tālāk norādītās darbības. 

1. Navigācijas rūtī pārlūkojiet līdz **Autentifikācijas politikas**.
2. Sadaļas Darbības detalizētas informācijas rūtī atlasiet **Rediģēt globālo primāro autentifikāciju**. 
3. Cilnē **Iekštīkls** atlasiet Forms **Authentication**.
4. Atlasiet **Labi** (vai **Lietot**).