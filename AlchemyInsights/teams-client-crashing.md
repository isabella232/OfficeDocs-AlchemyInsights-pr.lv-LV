---
title: Teams klienta avārija
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
- "9002323"
- "4512"
ms.openlocfilehash: a292e160abcfc26ffebc454d32ee489a319a23f4bb81e70fe5dbe72bfd0b8b81
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890345"
---
# <a name="teams-client-crashing"></a>Teams klienta avārija

Ja jūsu Teams klients avarē, mēģiniet veikt tālāk norādītās darbības:

- Ja izmantojat Teams datora programmu, [pārliecinieties, vai programma ir pilnībā atjaunināta](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Pārliecinieties, vai [visi Microsoft 365 visi vietrāži URL un adrešu diapazoni](https://docs.microsoft.com/microsoftteams/connectivity-issues) ir pieejami.

- Piesakieties ar sava nomnieka administratora kontu un pārbaudiet pakalpojuma darbspējas informācijas [paneli,](https://docs.microsoft.com/office365/enterprise/view-service-health) lai pārliecinātos, vai nepastāv pārtraukums vai pakalpojuma degradācija.

- Atinstalējiet un atkārtoti instalējiet Teams programmu
    - Pārlūkojiet līdz mapei %appdata%\Microsoft\Teams\ savā datorā un izdzēsiet visus šajā direktorijā esošos failus.
    - [Lejupielādējiet un instalējiet Teams programmu](https://www.microsoft.com/microsoft-teams/download-app)un, ja iespējams, instalējiet Teams kā administrators (ar peles labo  pogu noklikšķiniet uz Teams instalētāja un atlasiet Palaist kā administratoram, ja pieejams).

Ja jūsu Teams joprojām avarē, mēģiniet atveidot problēmu. Ja jūs varat:

1. Izmantojiet darbību ierakstītāju, lai tvertu darbības.
    - Aizveriet VISAS nevajadzīgās vai konfidenciālās lietojumprogrammas.
    - Palaidiet darbību ierakstītāju un atveidot problēmu, kad esat pieteicies ar ietekmētā lietotāja kontu.
    - [Apkopojiet to grupu žurnālus, kas tver ierakstītās pārpro darbību veikšanas darbības.](https://docs.microsoft.com/microsoftteams/log-files) **Piezīme.** Noteikti tveriet ietekmētā lietotāja pierakstīšanās adresi.
    - Apkopojiet informācija par atmeti un/vai kļūmes intervālu (Windows). Datorā palaidiet Windows Powershell, kur notiek avārija, un izpildiet šādas komandas (pēc katras komandas nospiediet taustiņu Enter):

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. Kad teksta fails ir ģenerēts un parādīts ekrānā, saglabājiet failu un pievienojiet to pakalpojuma pieprasījumam. 
