---
title: Problēma, kas savieno VMs
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
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885656"
---
# <a name="issue-joining-vms"></a>Problēma, kas savieno VMs

Lai atrisinātu problēmas, kas rodas, mēģinot pievienoties VMs, veiciet tālāk norādītās darbības.

1. Mēģiniet pierakstīties, izmantojot **UPN** formātu (piemēram, "joeuser@contoso.com"), nevis **SAMAccountName** formātu (' CONTOSO\joeuser ').
2. Pārliecinieties, vai esat iespējojis paroļu sinhronizāciju atbilstoši *darba sākšanas* rokasgrāmatā izklāstītajām darbībām.
3. Nodrošiniet, lai attiecīgais lietotāja konts nav ārējs konts Azure AD nomniekā. Ārējie lietotāji nevar pierakstīties pārvaldītajā domēnā, jo Azure AD domēna pakalpojumos nav šādu lietotāju kontu akreditācijas datu.
4. Ja attiecīgais lietotāja konts ir tikai Cloud lietotāja konts, pārliecinieties, vai lietotāji ir mainījuši savu paroli pēc Azure AD Domain Services iespējošanas. Veicot šo darbību, tiek izraisīti, lai varētu ģenerēt Azure AD domēna pakalpojumu vajadzībām nepieciešamos akreditācijas datus.
5. Ja ietekmētie lietotāju konti tiek sinhronizēti no lokālā direktorija, pārbaudiet, vai Azure AD Connect ieteicamais laidiens ir konfigurēts, lai veiktu pilnu sinhronizāciju.
6. Ja pēc 4. darbības apstiprināšanas problēma ir novērsta, izpildiet tālāk minētās komandas no sinhronizācijas datora.
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     `"net start 'Microsoft Azure AD Sync'"`.