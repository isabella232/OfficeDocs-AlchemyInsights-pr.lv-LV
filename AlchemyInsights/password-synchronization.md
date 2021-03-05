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
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482038"
---
# <a name="password-synchronization"></a>Paroles sinhronizācija

**Paroļu jaukšanas sinhronizācija vispār nedarbojas**

Biežāk sastopamās problēmas, kas rodas klientiem, ja nedarbojas paroļu jaukšanas sinhronizācija, ir šādas:

- Active Directory konts, ko izmanto Azure AD Connect, lai sazinātos ar lokālo pakalpojumu Active Directory, nepiešķir **replicēšanas direktorija izmaiņas** un **replicē direktorija izmaiņas** , kas nepieciešamas paroļu sinhronizēšanai, un jums tas ir jānovērš, piešķirot šīs atļaujas Active Directory kontam.
- Paroļu jaukšanas sinhronizācija ir atspējota pēc tam, kad administrators ir mainījis lietotāja Sign-In metodi no **paroļu sinhronizēšanas** uz citu opciju, piemēram, **FEDERĀCIJU ar AD FS** Azure AD Connect vednī — to var izlabot, atkārtoti iespējojot **paroļu jaukšanas sinhronizācijas** līdzekli Azure AD Connect vednī.
- Savienojamības problēma ar lokālo Active Directory. Piemēram, dažiem domēnu kontrolleriem nevar piekļūt, izmantojot Azure AD Connect, vai [nepieciešamos portus](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) ir bloķējis ugunsmūris — tas ir jānovērš, nodrošinot, ka savienojamība starp Azure AD Connect serveri un lokālo Active Directory darbojas pareizi.
- Azure AD Connect serveris pašlaik tiek atvērts sagatavošanas režīmā, un tas rezultātā serveris nevarēs izmantot paroļu jaukšanas iespējas — lai novērstu šo problēmu, izpildiet rakstā norādītās darbības: [paroļu sinhronizēšana ar AZURE ad Connect sinhronizāciju — nav paroļu](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).

**Dažu lietotāju paroļu jaukšanas sinhronizācija nedarbojas**

1. Ja esat pamanījis, ka parole hash netiek sinhronizēta lietotājam, izmantojiet **problēmu novēršanas** uzdevumu Azure AD Connect, lai izpētītu un atrisinātu problēmu. Veiciet tālāk norādītās darbības.

    izveide. [Vedņa problēmu novēršana](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Problēmu novēršanas cmdlet izmantošana, lai izpētītu paroļu jaukšanas problēmu saistībā ar konkrētu lietošanu](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Lokālā Active Directory lietotāja objekts ir iespējots **lietotājam ir jāmaina parole blakus pieteikšanās** opcijai. Ja šī opcija ir iespējota, lietotājam tiek piešķirta pagaidu parole, un tiks prasīts mainīt paroli nākamajā pieteikšanās reizē. Azure AD Connect nesinhronizē pagaidu paroles pakalpojumam Azure AD.

Lai atrisinātu šo problēmu, veiciet kādu no tālāk norādītajiem uzdevumiem.

- Lūdziet lietotājam pierakstīties lokālajā lietojumprogrammā (piemēram, Windows datorā) un mainīt paroli. Jaunā parole tiks sinhronizēta ar Azure AD.
- Administratoram ir jāatjaunina lietotāja parole, neiespējojot opciju **lietotājam nākamajā pieteikšanās reizē ir jāmaina parole** un jākopīgo jaunā parole ar lietotāju.

3. Lokālā Active Directory lietotāja objekts nav **pareizi konfigurēts** objektu sinhronizācijai vai paroļu sinhronizēšanai. Lai novērstu šo problēmu, izpildiet darbības, kas aprakstītas rakstā [paroļu jaukšanas sinhronizācijas problēmu novēršana, izmantojot AZURE ad Connect sinhronizāciju](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).







