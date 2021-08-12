---
title: Problēmu OneDrive avarēšanu
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
ms.openlocfilehash: d5982bafbb8aaa1d240a34c071efe37e92c2ec5c5170dc59337df9a5435e22e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53921014"
---
# <a name="troubleshoot-onedrive-crashes"></a>Problēmu OneDrive avarēšanu

Ja OneDrive atkārtoti avarē, izmēģiniet šīs problēmu novēršanas darbības:

**Pārliecinieties, vai reģistra atslēgas nav iestatītas:**

1. Izmantojot reģistra redaktoru, naviģējiet uz HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Ja parametra DisableFileSyncNGSC vērtība ir 1, atveriet atslēgu un mainiet vērtību uz 0.
3. Manuāli OneDrive, dodoties uz sākumu ![Nospiediet Windows taustiņu](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), ierakstiet OneDrive lodziņā un pēc tam noklikšķiniet uz darbvirsmas OneDrive lietojumprogrammas.

**Atiestatīt OneDrive:**

Piezīmes.

- Atiestatot OneDrive tiek pārtraukti visi jūsu esošie sinhronizācijas savienojumi (ieskaitot personiskos savienojumus OneDrive ja tādi ir iestatīti).
- Datorā atiestatot datus, jūs nezaudēsit OneDrive datus.

**Lai atiestatītu OneDrive:**

1. Atveriet izpildes dialoglodziņu, nospiežot taustiņu Windows un R.
2. Ierakstiet %localappdata%\Microsoft\OneDrive\onedrive.exe /reset un nospiediet Labi. Var īslaicīgi parādīties komandu logs.
3. Manuāli OneDrive, dodoties uz sākumu ![Nospiediet Windows taustiņu](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), ierakstiet OneDrive lodziņā un pēc tam noklikšķiniet uz darbvirsmas OneDrive lietojumprogrammas.

Piezīmes.

- Ja pirms atiestatīšanas izvēlējāties sinhronizēt tikai dažas mapes, to vajadzēs izdarīt vēlreiz (pēc tam, kad būs pabeigta sinhronizācija).  [Papildinformāciju skatiet OneDrive, kuras mapes sinhronizēt ar](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   datoru.
- Šīs darbības būs jāveic personiskajām OneDrive OneDrive darbam.