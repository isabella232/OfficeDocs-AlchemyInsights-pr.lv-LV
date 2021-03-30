---
title: Palīdzība par nakts gaismas displeja iestatījumu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404665"
---
# <a name="help-with-the-night-light-display-setting"></a>Palīdzība par nakts gaismas displeja iestatījumu

Papildinformāciju par nakts laika displeja iestatījumiem skatiet [rakstā Displeja iestatīšana nakts laikam operētājsistēmā Windows 10.](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)

Ja nakts gaismas opcijas iestatījumos ir pelēkotas, skatiet displeja draiveri: 

1. Uzdevumjoslā noklikšķiniet uz meklēšanas lodziņa **un ierakstiet Ierīču** pārvaldnieks un pēc tam meklēšanas **rezultātos** atlasiet Ierīču pārvaldnieks.
1. Izvērsiet **displeja adapterus**. 

Diemžēl nakts gaismas līdzeklis nav pieejams, ja jūsu ierīce izmanto DisplayLink draiveri vai pamata displeja draiveri.

Nakts gaismas līdzeklis izmanto jaunākās grafikas tehnoloģijas, tāpēc, iespējams, būs jāatjaunina displeja draiveris:  

- Pārbaudiet, vai nav atjauninājumu, **dodoties uz Sākums**  >  **Iestatījumu**  >  **atjaunināšanas &** Windows  >  **Update**  >  **pārbaudīt, vai nav atjauninājumu.**  

VAI

- Apmeklējiet aparatūras ražotāja atbalsta tīmekļa vietni, lai manuāli lejupielādētu un instalētu jaunākos displeja draiverus.

## <a name="reset-night-light-in-the-registry"></a>Atiestatīt nakts gaismu reģistrā

Ja displeja draivera atjaunināšana nedarbojas, iespējams, būs jāatiestata nakts gaisma reģistrā.  

**Uzmanību!** Šī problēmu novēršanas darbība ir ieteicama tikai pieredzējušiem lietotājiem. Nepareizi modificējot reģistru, iespējamas nopietnas problēmas. Lai nodrošinātu papildu aizsardzību, dublējiet reģistru, pirms to modificējat, lai varētu to atjaunot, ja rodas problēmas.

1. Meklēšanas lodziņā ierakstiet **regedit un** pēc tam meklēšanas **rezultātos atlasiet** Reģistra redaktors.

1. Dodieties uz šo reģistra atslēgu: 

    HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount

1. Eksportējiet un pēc tam izdzēsiet šo apakšatslēgu:$$windows.data.bluelightreduction.bluelightreductionstate

1. Eksportējiet un pēc tam izdzēsiet šo apakšatslēgu:$$windows.data.bluelightreduction.settings

1. Restartējiet Windows un pārbaudiet, vai ir pieejamas nakts gaismas opcijas.


