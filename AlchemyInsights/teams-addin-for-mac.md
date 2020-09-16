---
title: Teams pievienojumprogramma darbam ar Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 1e5f6d66386398ad8600f9383f9f7a1dcf0ce69f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670335"
---
# <a name="teams-add-in-for-mac"></a>Teams pievienojumprogramma darbam ar Mac

Lai novērstu problēmas saistībā ar trūkstošo grupu pievienojumprogrammu darbam ar Mac operētājsistēmu lietotājiem, veiciet tālāk norādītās darbības.

**1. darbība:** Ja jums ir hibrīda Exchange lokāli (2016 CU3 vai jaunāka versija), izmantojiet Test-HMA.ps1 rīku, lai apstiprinātu, ka hibrīdā modernā autentifikācija ir pareizi konfigurēta. Papildinformāciju skatiet rakstā [hibrīdās modernās autentifikācijas iestatīšana programmā Outlook darbam ar iOS un Android](https://aka.ms/AA980zq).  

**Piezīmes** Izmantojiet UPN adreses formātu (piemēram, [username@contoso.com](mailto:username@contoso.com)), not domēns \ lietotājvārds To var paveikt arī lietotājiem, kuriem ir Exchange Online pastkastes.

**2. darbība.** Vai lietotājam ir jāpāriet uz **rīku**  >  **konti**... programmā Outlook darbam ar Mac atrodiet un atlasiet kontu. Apstipriniet, ka sarakstā norādītais lietotājvārds ir UPN formātā (piemēram, [username@contoso.com](mailto:username@contoso.com)).

**3. darbība:** Apstipriniet, ka lietotājs ir licencēts Microsoft Teams lietotājs. Lietotājam ir jāizmanto Office 365 for Mac abonements, produkta versija 16,24 vai jaunāka versija.