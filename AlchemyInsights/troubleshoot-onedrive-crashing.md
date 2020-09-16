---
title: OneDrive avāriju problēmu novēršana
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665005"
---
# <a name="troubleshoot-onedrive-crashes"></a>OneDrive avāriju problēmu novēršana

Ja OneDrive vairākkārt avarē, izmēģiniet šīs problēmu novēršanas darbības:

**Pārliecinieties, vai nav iestatītas reģistra atslēgas:**

1. Izmantojot reģistra redaktoru, pārejiet uz HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive
2. Ja DisableFileSyncNGSC ir klātesošs un iestatīts uz 1, atveriet atslēgu un mainiet vērtību uz 0.
3. Manuāli palaidiet OneDrive, dodoties uz sākumu ![Nospiediet Windows taustiņu](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), meklēšanas lodziņā ierakstiet OneDrive un pēc tam noklikšķiniet uz OneDrive datora lietojumprogrammas.

**OneDrive atiestatīšana:**

Piezīmes

- OneDrive atiestatīšana atveido visus esošos sinhronizācijas savienojumus (tostarp savu personisko OneDrive, ja tas ir iestatīts).
- Jūs nezaudēsit failus vai datus, atiestatot OneDrive savā datorā.

**Lai atiestatītu OneDrive:**

1. Atveriet palaišanas dialoglodziņu, nospiežot Windows taustiņu un R.
2. Ierakstiet% LOCALAPPDATA% \Microsoft\OneDrive\onedrive.exe/reset un nospiediet Labi. Var īslaicīgi parādīties komandu logs.
3. Manuāli palaidiet OneDrive, dodoties uz sākumu ![Nospiediet Windows taustiņu](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), meklēšanas lodziņā ierakstiet OneDrive un pēc tam noklikšķiniet uz OneDrive datora lietojumprogrammas.

Piezīmes

- Ja izvēlējāties sinhronizēt tikai dažas mapes pirms atiestates, jums tā būs jāveic atkārtoti, kad sinhronizācija ir pabeigta. Lai iegūtu papildinformāciju, izlasiet rakstu kā [izvēlēties, kuras OneDrive mapes sinhronizēt ar datoru](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   .
- Šī darbība ir jāveic jūsu personiskajai OneDrive un OneDrive darbam.