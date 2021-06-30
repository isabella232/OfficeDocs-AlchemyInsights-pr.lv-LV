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
# <a name="teams-client-crashing"></a><span data-ttu-id="f7ac7-102">Teams klienta avārija</span><span class="sxs-lookup"><span data-stu-id="f7ac7-102">Teams client crashing</span></span>

<span data-ttu-id="f7ac7-103">Ja jūsu Teams klients avarē, mēģiniet veikt tālāk norādītās darbības:</span><span class="sxs-lookup"><span data-stu-id="f7ac7-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="f7ac7-104">Ja izmantojat Teams datora programmu, [pārliecinieties, vai programma ir pilnībā atjaunināta](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="f7ac7-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="f7ac7-105">Pārliecinieties, vai [visi Microsoft 365 vietrāžu URL un adrešu diapazoni](/microsoftteams/connectivity-issues) ir pieejami.</span><span class="sxs-lookup"><span data-stu-id="f7ac7-105">Make sure all the [Microsoft 365 URLs and address ranges](/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="f7ac7-106">Piesakieties ar sava nomnieka administratora kontu un pārbaudiet pakalpojuma darbspējas informācijas [paneli,](/office365/enterprise/view-service-health) lai pārliecinātos, vai nepastāv pārtraukums vai pakalpojuma degradācija.</span><span class="sxs-lookup"><span data-stu-id="f7ac7-106">Log in with your tenant admin account and check your [Service Health Dashboard](/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="f7ac7-107">Atinstalējiet un atkārtoti instalējiet Teams programmu</span><span class="sxs-lookup"><span data-stu-id="f7ac7-107">Uninstall and reinstall the Teams Application</span></span>
    - <span data-ttu-id="f7ac7-108">Pārlūkojiet līdz mapei %appdata%\Microsoft\Teams\ savā datorā un izdzēsiet visus šajā direktorijā esošos failus.</span><span class="sxs-lookup"><span data-stu-id="f7ac7-108">Browse to the %appdata%\Microsoft\Teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="f7ac7-109">[Lejupielādējiet un instalējiet lietojumprogrammu Teams](https://www.microsoft.com/microsoft-teams/download-app)un, ja iespējams, instalējiet Teams kā administrators (ar peles labo pogu noklikšķiniet uz Teams instalētāja un atlasiet Palaist kā administratoram, **ja** pieejams).</span><span class="sxs-lookup"><span data-stu-id="f7ac7-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-teams/download-app), and if possible, install Teams as an administrator (right-click the Teams installer, and select **Run as administrator** if available).</span></span>

<span data-ttu-id="f7ac7-110">Ja jūsu Teams joprojām avarē, mēģiniet atveidot problēmu.</span><span class="sxs-lookup"><span data-stu-id="f7ac7-110">If your Teams client is still crashing, try to reproduce the issue.</span></span> <span data-ttu-id="f7ac7-111">Ja jūs varat:</span><span class="sxs-lookup"><span data-stu-id="f7ac7-111">If you can:</span></span>

1. <span data-ttu-id="f7ac7-112">Izmantojiet darbību ierakstītāju, lai tvertu darbības.</span><span class="sxs-lookup"><span data-stu-id="f7ac7-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="f7ac7-113">Aizveriet VISAS nevajadzīgās vai konfidenciālās lietojumprogrammas.</span><span class="sxs-lookup"><span data-stu-id="f7ac7-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="f7ac7-114">Palaidiet darbību ierakstītāju un atveidot problēmu, kad esat pieteicies ar ietekmētā lietotāja kontu.</span><span class="sxs-lookup"><span data-stu-id="f7ac7-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="f7ac7-115">[Apkopojiet to grupu žurnālus, kas tver ierakstītās pārpro darbību veikšanas darbības.](/microsoftteams/log-files)</span><span class="sxs-lookup"><span data-stu-id="f7ac7-115">[Collect the teams logs that capture the recorded repro steps](/microsoftteams/log-files).</span></span> <span data-ttu-id="f7ac7-116">**Piezīme.** Noteikti tveriet ietekmētā lietotāja pierakstīšanās adresi.</span><span class="sxs-lookup"><span data-stu-id="f7ac7-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="f7ac7-117">Apkopojiet informācija par atmeti un/vai kļūmes intervālu (Windows).</span><span class="sxs-lookup"><span data-stu-id="f7ac7-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="f7ac7-118">Datorā palaidiet Windows Powershell, kur notiek avārija, un izpildiet šādas komandas (pēc katras komandas nospiediet taustiņu Enter):</span><span class="sxs-lookup"><span data-stu-id="f7ac7-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands (after each command, press Enter):</span></span>

    <span data-ttu-id="f7ac7-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span><span class="sxs-lookup"><span data-stu-id="f7ac7-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span></span>
    `notepad .\FaultBuckets.txt`
    
2. <span data-ttu-id="f7ac7-120">Kad teksta fails ir ģenerēts un parādīts ekrānā, saglabājiet failu un pievienojiet to pakalpojuma pieprasījumam.</span><span class="sxs-lookup"><span data-stu-id="f7ac7-120">After the text file is generated and appears on your screen, save the file and attach it to the service request.</span></span> 
