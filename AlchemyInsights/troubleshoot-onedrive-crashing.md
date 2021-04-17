---
title: OneDrive avarēšanu novēršana
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
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826206"
---
# <a name="troubleshoot-onedrive-crashes"></a>OneDrive avarēšanu novēršana

Ja OneDrive atkārtoti avarē, izmēģiniet šīs problēmu novēršanas darbības:

**Pārliecinieties, vai reģistra atslēgas nav iestatītas:**

1. Izmantojot reģistra redaktoru, naviģējiet uz HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Ja parametra DisableFileSyncNGSC vērtība ir 1, atveriet atslēgu un mainiet vērtību uz 0.
3. Manuāla OneDrive palaišana, dodoties uz sākumu ![Nospiediet Windows taustiņu](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), meklēšanas lodziņā ierakstiet OneDrive un pēc tam noklikšķiniet uz OneDrive datora programmas.

**OneDrive atiestatīšana:**

Piezīmes.

- OneDrive atiestatīšana atvieno visus esošos sinhronizācijas savienojumus (ieskaitot OneDrive individuālai lietošanai, ja tas ir iestatīts).
- Datorā atiestatot OneDrive, jūs nezaudēsit failus vai datus.

**Lai atiestatītu OneDrive:**

1. Atveriet izpildes dialoglodziņu, nospiežot Windows taustiņu un R.
2. Ierakstiet %localappdata%\Microsoft\OneDrive\onedrive.exe /reset un nospiediet Labi. Var īslaicīgi parādīties komandu logs.
3. Manuāla OneDrive palaišana, dodoties uz sākumu ![Nospiediet Windows taustiņu](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), meklēšanas lodziņā ierakstiet OneDrive un pēc tam noklikšķiniet uz OneDrive datora programmas.

Piezīmes.

- Ja pirms atiestatīšanas izvēlējāties sinhronizēt tikai dažas mapes, to vajadzēs izdarīt vēlreiz (pēc tam, kad būs pabeigta sinhronizācija).  [Papildinformāciju skatiet rakstu Ar datoru sinhronizējamo OneDrive](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)mapju   izvēlēšana.
- Šīs darbības būs jāveic personiskajam OneDrive un OneDrive darbam.