---
title: Grupu piešķiršana Azure AD lomai
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
- "7898"
- "9003230"
ms.openlocfilehash: 563b1a7c93c9ca64fdea51c57b70fd2132750c4ad8ee15de0c65c9668c9c3c56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036247"
---
# <a name="assigning-groups-to-azure-ad-role"></a>Grupu piešķiršana Azure AD lomai

Lai Azure AD lomai piešķirtu Azure AD grupu ar azure AD avotu, veiciet šādas darbības:

1. Izveidot jaunu grupu — lai izveidotu jaunu grupu:

    a. Pierakstieties Azure AD administrēšanas centrā ar **priviliģētas lomas administratora** vai **globālā administratora atļaujām.**
    b. Atlasiet **Azure Active Directory > Grupas > Visas grupas > Jauna grupa**.
    c. Izveidojiet grupu.

2. Piešķiriet lomu grupai grupas izveides laikā vai pēc grupas izveides.

    a. Lai piešķirtu lomu grupai grupas izveides laikā, ieslēdziet slēdzi **Azure AD** lomu var piešķirt grupai un izveidot grupu.
    b. Lai piešķirtu lomu grupai pēc tās izveides, naviģējiet uz jaunizveidotās grupas cilni **Piešķirtās lomas** un piešķiriet lomu grupai.  

**Pārvaldīt dalību grupā, kas ir piešķirta Azure AD lomai**

Lai nepieļautu privilēģiju pacēlumu, pēc noklusējuma tikai priviliģētie lomu administratori un globālie administratori var modificēt lomu grupai, kam ir piešķirta šī loma. Tomēr viņi var izvēlēties piešķirt šādas grupas īpašniekam un deleģēt šo uzdevumu.

Papildinformāciju par mākoņu grupu piešķiršanu Azure AD lomām skatiet rakstā [AD lomu piešķiršana mākoņa grupai.](https://docs.microsoft.com/azure/active-directory/roles/groups-concept) Papildinformāciju par mākoņa grupām piešķirtajām problēmu novēršanas lomām skatiet rakstā Mākoņa grupām [piešķirto lomu problēmu novēršana.](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)





