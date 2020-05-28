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
# <a name="teams-client-crashing"></a><span data-ttu-id="97b69-102">Vai Teams klients avarē?</span><span class="sxs-lookup"><span data-stu-id="97b69-102">Teams client crashing?</span></span>

<span data-ttu-id="97b69-103">Ja jūsu Teams klients avarē, mēģiniet veikt tālāk norādītās darbības:</span><span class="sxs-lookup"><span data-stu-id="97b69-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="97b69-104">Ja izmantojat Teams datora programmu, [pārliecinieties, vai programma ir pilnībā atjaunināta](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="97b69-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="97b69-105">Pārliecinieties, vai ir pieejami visi [Microsoft 365 vietrāži URL un adrešu diapazoni](https://docs.microsoft.com/microsoftteams/connectivity-issues) .</span><span class="sxs-lookup"><span data-stu-id="97b69-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="97b69-106">Piesakieties ar savu nomnieka administratora kontu un pārbaudiet [pakalpojumu darbspējas informācijas paneli](https://docs.microsoft.com/office365/enterprise/view-service-health) , lai pārbaudītu, vai pastāv pārtraukums vai pakalpojumu degradācija.</span><span class="sxs-lookup"><span data-stu-id="97b69-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="97b69-107">Programmu Teams atinstalēšana un atkārtota instalēšana (saite)</span><span class="sxs-lookup"><span data-stu-id="97b69-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="97b69-108">Atrodiet datorā%appdata%\Microsoft\teams\ mapi un dzēsiet visus failus šajā direktorijā.</span><span class="sxs-lookup"><span data-stu-id="97b69-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="97b69-109">[Lejupielādējiet un instalējiet programmu Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), un, ja iespējams, instalējiet komandas kā administratoram (ar peles labo pogu noklikšķiniet uz komandu Installer un atlasiet "palaist kā administratoram", ja pieejams).</span><span class="sxs-lookup"><span data-stu-id="97b69-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="97b69-110">Ja jūsu komandas klients joprojām avarē, jūs varat reproducēt problēmu?</span><span class="sxs-lookup"><span data-stu-id="97b69-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="97b69-111">Ja tā:</span><span class="sxs-lookup"><span data-stu-id="97b69-111">If so:</span></span>

1. <span data-ttu-id="97b69-112">Lai tvertu soļus, izmantojiet darbību reģistrētāju.</span><span class="sxs-lookup"><span data-stu-id="97b69-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="97b69-113">Aizveriet visas nevajadzīgās vai konfidenciālās lietojumprogrammas.</span><span class="sxs-lookup"><span data-stu-id="97b69-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="97b69-114">Palaidiet darbību reģistrētājs un atveidot problēmu, kamēr pieteicies ar attiecīgā lietotāja kontu.</span><span class="sxs-lookup"><span data-stu-id="97b69-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="97b69-115">[Savāc komandu žurnālus, kas tver ierakstītās REPRO darbības](https://docs.microsoft.com/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="97b69-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="97b69-116">**Piezīme**: pārliecinieties, vai tverat skartā lietotāja pierakstīšanās adresi.</span><span class="sxs-lookup"><span data-stu-id="97b69-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="97b69-117">Savāc dump un/vai vaina Bucket info (Windows).</span><span class="sxs-lookup"><span data-stu-id="97b69-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="97b69-118">Palaidiet Windows PowerShell datorā, kur notiek avārija, un palaidiet tālāk norādītās komandas.</span><span class="sxs-lookup"><span data-stu-id="97b69-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="97b69-119">Pievienojiet failu savam atbalsta gadījumam.</span><span class="sxs-lookup"><span data-stu-id="97b69-119">Attach the file to your support case.</span></span>
