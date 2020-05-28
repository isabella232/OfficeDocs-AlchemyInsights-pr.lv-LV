---
title: Vai Teams klients avarē?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ac1cc05adfa33626ff34d30dca6c77f1bb96477a
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354059"
---
# <a name="teams-client-crashing"></a>Vai Teams klients avarē?

Ja jūsu Teams klients avarē, mēģiniet veikt tālāk norādītās darbības:

- Ja izmantojat Teams datora programmu, [pārliecinieties, vai programma ir pilnībā atjaunināta](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Pārliecinieties, vai ir pieejami visi [Microsoft 365 vietrāži URL un adrešu diapazoni](https://docs.microsoft.com/microsoftteams/connectivity-issues) .

- Piesakieties ar savu nomnieka administratora kontu un pārbaudiet [pakalpojumu darbspējas informācijas paneli](https://docs.microsoft.com/office365/enterprise/view-service-health) , lai pārbaudītu, vai pastāv pārtraukums vai pakalpojumu degradācija.

- Programmu Teams atinstalēšana un atkārtota instalēšana (saite)
    - Atrodiet datorā%appdata%\Microsoft\teams\ mapi un dzēsiet visus failus šajā direktorijā.
    - [Lejupielādējiet un instalējiet programmu Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), un, ja iespējams, instalējiet komandas kā administratoram (ar peles labo pogu noklikšķiniet uz komandu Installer un atlasiet "palaist kā administratoram", ja pieejams).

Ja jūsu komandas klients joprojām avarē, jūs varat reproducēt problēmu? Ja tā:

1. Lai tvertu soļus, izmantojiet darbību reģistrētāju.
    - Aizveriet visas nevajadzīgās vai konfidenciālās lietojumprogrammas.
    - Palaidiet darbību reģistrētājs un atveidot problēmu, kamēr pieteicies ar attiecīgā lietotāja kontu.
    - [Savāc komandu žurnālus, kas tver ierakstītās REPRO darbības](https://docs.microsoft.com/microsoftteams/log-files). **Piezīme**: pārliecinieties, vai tverat skartā lietotāja pierakstīšanās adresi.
    - Savāc dump un/vai vaina Bucket info (Windows). Palaidiet Windows PowerShell datorā, kur notiek avārija, un palaidiet tālāk norādītās komandas.

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Pievienojiet failu savam atbalsta gadījumam.
