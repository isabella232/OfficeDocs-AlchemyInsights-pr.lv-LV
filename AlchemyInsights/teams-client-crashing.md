---
title: Vai Teams klients avarē?
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
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826278"
---
# <a name="teams-client-crashing"></a>Vai Teams klients avarē?

Ja jūsu Teams klients avarē, mēģiniet veikt tālāk norādītās darbības:

- Ja izmantojat Teams datora programmu, [pārliecinieties, vai programma ir pilnībā atjaunināta](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Pārliecinieties, vai [visi Microsoft 365 vietrāži URL un adrešu diapazoni](https://docs.microsoft.com/microsoftteams/connectivity-issues) ir pieejami.

- Piesakieties ar sava nomnieka administratora kontu un pārbaudiet pakalpojuma darbspējas informācijas [paneli,](https://docs.microsoft.com/office365/enterprise/view-service-health) lai pārliecinātos, vai nepastāv pārtraukums vai pakalpojuma degradācija.

- Atinstalējiet un atkārtoti instalējiet Teams programmu (saiti)
    - Pārlūkojiet līdz mapei %appdata%\Microsoft\teams\ savā datorā un izdzēsiet visus failus šajā direktorijā.
    - [Lejupielādējiet un instalējiet Teams lietotni](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)un, ja iespējams, instalējiet Teams kā administrators (ar peles labo pogu noklikšķiniet uz Teams instalēšanas programmas un atlasiet "Palaist kā administratoram", ja pieejams).

Ja jūsu Teams klients joprojām avarē, vai varat atveidot problēmu? Ja tā ir:

1. Izmantojiet darbību ierakstītāju, lai tvertu darbības.
    - Aizveriet VISAS nevajadzīgās vai konfidenciālās lietojumprogrammas.
    - Palaidiet darbību ierakstītāju un atveidot problēmu, kad esat pieteicies ar ietekmētā lietotāja kontu.
    - [Apkopojiet to grupu žurnālus, kas tver ierakstītās pārpro darbību veikšanas darbības.](https://docs.microsoft.com/microsoftteams/log-files) **Piezīme.** Noteikti tveriet ietekmētā lietotāja pierakstīšanās adresi.
    - Apkopojiet informācija par spaļu un/vai kļūmes intervālu (Windows). Datorā palaidiet Windows Powershell, kur notiek avārija, un izpildiet šādas komandas:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Pievienojiet failu savam atbalsta pieteikumam.
