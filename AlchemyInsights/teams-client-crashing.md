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
ms.openlocfilehash: 7acb2f5f87a9cfbd67cd94efca696665fd80fc4a
ms.sourcegitcommit: 3cdfde87b7311c200431196031af92c640fd0d8d
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/29/2021
ms.locfileid: "53187728"
---
# <a name="teams-client-crashing"></a>Teams klienta avārija

Ja jūsu Teams klients avarē, mēģiniet veikt tālāk norādītās darbības:

- Ja izmantojat Teams datora programmu, [pārliecinieties, vai programma ir pilnībā atjaunināta](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Pārliecinieties, vai [visi Microsoft 365 vietrāžu URL un adrešu diapazoni](/microsoftteams/connectivity-issues) ir pieejami.

- Piesakieties ar sava nomnieka administratora kontu un pārbaudiet pakalpojuma darbspējas informācijas [paneli,](/office365/enterprise/view-service-health) lai pārliecinātos, vai nepastāv pārtraukums vai pakalpojuma degradācija.

- Atinstalējiet un atkārtoti instalējiet Teams programmu
    - Pārlūkojiet līdz mapei %appdata%\Microsoft\Teams\ savā datorā un izdzēsiet visus šajā direktorijā esošos failus.
    - [Lejupielādējiet un instalējiet lietojumprogrammu Teams](https://www.microsoft.com/microsoft-teams/download-app)un, ja iespējams, instalējiet Teams kā administrators (ar peles labo pogu noklikšķiniet uz Teams instalētāja un atlasiet Palaist kā administratoram, **ja** pieejams).

Ja jūsu Teams joprojām avarē, mēģiniet atveidot problēmu. Ja jūs varat:

1. Izmantojiet darbību ierakstītāju, lai tvertu darbības.
    - Aizveriet VISAS nevajadzīgās vai konfidenciālās lietojumprogrammas.
    - Palaidiet darbību ierakstītāju un atveidot problēmu, kad esat pieteicies ar ietekmētā lietotāja kontu.
    - [Apkopojiet to grupu žurnālus, kas tver ierakstītās pārpro darbību veikšanas darbības.](/microsoftteams/log-files) **Piezīme.** Noteikti tveriet ietekmētā lietotāja pierakstīšanās adresi.
    - Apkopojiet informācija par atmeti un/vai kļūmes intervālu (Windows). Datorā palaidiet Windows Powershell, kur notiek avārija, un izpildiet šādas komandas (pēc katras komandas nospiediet taustiņu Enter):

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. Kad teksta fails ir ģenerēts un parādīts ekrānā, saglabājiet failu un pievienojiet to pakalpojuma pieprasījumam. 
