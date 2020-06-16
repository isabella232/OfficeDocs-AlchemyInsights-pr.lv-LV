---
title: OneDrive avāriju problēmu novēršana
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/15/2020
ms.locfileid: "44749161"
---
# <a name="troubleshoot-onedrive-crashes"></a>OneDrive avāriju problēmu novēršana

Ja OneDrive atkārtoti avarē, veiciet tālāk norādītās problēmu novēršanas darbības.

**Pārliecinieties, vai reģistra atslēgas nav iestatītas:**

1. Izmantojot reģistra redaktoru, naviģējiet uz HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Ja DisableFileSyncNGSC ir un iestatīts uz 1, atveriet atslēgu un mainiet vērtību uz 0.
3. Manuāli palaist OneDrive, dodoties uz sākuma ekrāna ![Nospiediet Windows taustiņu](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), meklēšanas lodziņā ierakstiet OneDrive un pēc tam noklikšķiniet uz OneDrive datora lietojumprogrammas.

**OneDrive atiestatīšana:**

Piezīmes:

- OneDrive atiestatīšana atvieno visus esošos sinhronizācijas savienojumus (tostarp personisko OneDrive, ja tas ir iestatīts).
- Jūs nezaudēsit failus vai datus, atiestatot OneDrive datorā.

**Lai atiestatītu OneDrive:**

1. Atveriet dialoglodziņu Izpildīt, nospiežot Windows taustiņu un R.
2. Ierakstiet %localappdata%\Microsoft\OneDrive\onedrive.exe /reset un nospiediet Labi. Uz īsu brīdi var parādīties komandlogs.
3. Manuāli palaist OneDrive, dodoties uz sākuma ekrāna ![Nospiediet Windows taustiņu](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), meklēšanas lodziņā ierakstiet OneDrive un pēc tam noklikšķiniet uz OneDrive datora lietojumprogrammas.

Piezīmes:

- Ja pirms atiestatīšanas esat izvēlējies sinhronizēt tikai dažas mapes, pēc sinhronizācijas pabeigšanas tas būs jādara vēlreiz. Lai [iegūtu papildinformāciju, izlasiet rakstu Izvēlieties, kuras OneDrive](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   mapes sinhronizēt ar datoru.
- Tas ir jāaizpilda personiskajam OneDrive un OneDrive darbam.