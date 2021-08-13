---
title: Paroles sinhronizācija
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 3cdde086e535d2397b4d1a8a66903121a5217015ca055fb9f8d025b0842f044b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960842"
---
# <a name="password-synchronization"></a>Paroles sinhronizācija

**Paroļu jaukšanas sinhronizācija vispār nedarbojas**

Dažas bieži sastopamās problēmas, kas rodas klientiem, kad paroļu jaukšanas sinhronizācija nedarbojas, ir:

- Active Directory kontam, ko Azure AD Savienošana izmanto saziņai ar lokālo  Active Directory,  nav piešķirta atļauja Replicēt direktorija izmaiņas un Replicēt direktorija izmaiņas visas atļaujas, kas ir nepieciešamas paroļu sinhronizēšanai. Tas ir jālabo, piešķirot šīs atļaujas Active Directory kontam.
- Paroļu jaukšanas sinhronizācija ir atspējota, kad  administrators ir mainījis lietotāja Sign-In metodi no paroļu sinhronizācijas uz citu opciju, piemēram,  federāciju ar **AD FS** Azure AD Savienošana vednī — to var novērst, atkārtoti iespējojot paroļu jaukšanas sinhronizācijas līdzekli Azure AD Savienošana vednī.
- Savienojamības problēma saistībā ar lokālo Active Directory. Piemēram, daži domēna kontrolleri nav pieejami pakalpojumam Azure AD [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) Savienošana vai nepieciešamos portus bloķē ugunsmūris — tas ir jālabo, nodrošinot, lai savienojums starp Azure AD Savienošana serveri un lokālo Active Directory darbotos pareizi.
- Azure AD Savienošana serveris pašlaik ir iztrūka iztrūkšanas režīmā, kā rezultātā serveris nevar piekļūt paroles jaukšanas metodei – Lai novērstu problēmu, izpildiet darbības, kas aprakstītas sadaļā Paroļu sinhronizēšanas ar Azure AD Savienošana sinhronizāciju problēmu novēršana — paroles netiek [sinhronizētas.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

**Paroļu jaukšanas sinhronizācija dažiem maniem lietotājiem nedarbojas**

1. Ja esat pamanījis, ka paroles jaukšanas vienums netiek sinhronizēts lietotājam, izmantojiet Azure AD Savienošana problēmu novēršanas uzdevumu, lai izpētītu un atrisinātu problēmu.  Veiciet šādus uzdevumus:

    a. [Problēmu novēršanas uzdevuma palaišana vednī](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Problēmu novēršanas cmdlet izmantošana, lai izpētītu paroļu jaukšanas sinhronizācijas problēmu konkrētam lietotājam](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Lokālais Active Directory lietotāja objekts ir iespējots **lietotājam, parole jāmaina pie nākamās pieteikšanās** opcijas. Kad šī opcija ir iespējota, lietotājam tiek piešķirta pagaidu parole, un nākamajā pieteikšanās reizē tiek prasīts mainīt paroli. Azure AD Savienošana nesinhronizē pagaidu paroles ar Azure AD.

Lai novērstu iepriekš minēto problēmu, veiciet kādu no tālāk minētajiem uzdevumiem.

- Palūdziet lietotājam pierakstīties lokālajā lietojumprogrammā (piemēram, Windows datorā) un mainīt paroli. Jaunā parole tiks sinhronizēta ar Azure AD.
- Lai administrators atjauninātu lietotāja paroli, neiespējojot opciju Nākamajā pieteikšanās reizē lietotājam ir jāmaina parole **un** jaunā parole jā koplietot ar lietotāju.

3. Lokālā Active Directory lietotāja objekts nav pareizi **konfigurēts objektu sinhronizācijai** vai paroļu sinhronizācijai. Lai novērstu šo problēmu, izpildiet darbības, kas aprakstītas rakstā Paroļu jaukšanas [sinhronizācijas problēmu novēršana ar Azure AD Savienošana sinhronizāciju.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)







