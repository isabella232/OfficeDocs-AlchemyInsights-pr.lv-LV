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
# <a name="teams-client-crashing"></a><span data-ttu-id="0d809-102">Vai Teams klients avarē?</span><span class="sxs-lookup"><span data-stu-id="0d809-102">Teams client crashing?</span></span>

<span data-ttu-id="0d809-103">Ja jūsu Teams klients avarē, mēģiniet veikt tālāk norādītās darbības:</span><span class="sxs-lookup"><span data-stu-id="0d809-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="0d809-104">Ja izmantojat Teams datora programmu, [pārliecinieties, vai programma ir pilnībā atjaunināta](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="0d809-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="0d809-105">Pārliecinieties, vai [visi Microsoft 365 vietrāži URL un adrešu diapazoni](https://docs.microsoft.com/microsoftteams/connectivity-issues) ir pieejami.</span><span class="sxs-lookup"><span data-stu-id="0d809-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="0d809-106">Piesakieties ar sava nomnieka administratora kontu un pārbaudiet pakalpojuma darbspējas informācijas [paneli,](https://docs.microsoft.com/office365/enterprise/view-service-health) lai pārliecinātos, vai nepastāv pārtraukums vai pakalpojuma degradācija.</span><span class="sxs-lookup"><span data-stu-id="0d809-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="0d809-107">Atinstalējiet un atkārtoti instalējiet Teams programmu (saiti)</span><span class="sxs-lookup"><span data-stu-id="0d809-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="0d809-108">Pārlūkojiet līdz mapei %appdata%\Microsoft\teams\ savā datorā un izdzēsiet visus failus šajā direktorijā.</span><span class="sxs-lookup"><span data-stu-id="0d809-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="0d809-109">[Lejupielādējiet un instalējiet Teams lietotni](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)un, ja iespējams, instalējiet Teams kā administrators (ar peles labo pogu noklikšķiniet uz Teams instalēšanas programmas un atlasiet "Palaist kā administratoram", ja pieejams).</span><span class="sxs-lookup"><span data-stu-id="0d809-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="0d809-110">Ja jūsu Teams klients joprojām avarē, vai varat atveidot problēmu?</span><span class="sxs-lookup"><span data-stu-id="0d809-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="0d809-111">Ja tā ir:</span><span class="sxs-lookup"><span data-stu-id="0d809-111">If so:</span></span>

1. <span data-ttu-id="0d809-112">Izmantojiet darbību ierakstītāju, lai tvertu darbības.</span><span class="sxs-lookup"><span data-stu-id="0d809-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="0d809-113">Aizveriet VISAS nevajadzīgās vai konfidenciālās lietojumprogrammas.</span><span class="sxs-lookup"><span data-stu-id="0d809-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="0d809-114">Palaidiet darbību ierakstītāju un atveidot problēmu, kad esat pieteicies ar ietekmētā lietotāja kontu.</span><span class="sxs-lookup"><span data-stu-id="0d809-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="0d809-115">[Apkopojiet to grupu žurnālus, kas tver ierakstītās pārpro darbību veikšanas darbības.](https://docs.microsoft.com/microsoftteams/log-files)</span><span class="sxs-lookup"><span data-stu-id="0d809-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="0d809-116">**Piezīme.** Noteikti tveriet ietekmētā lietotāja pierakstīšanās adresi.</span><span class="sxs-lookup"><span data-stu-id="0d809-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="0d809-117">Apkopojiet informācija par spaļu un/vai kļūmes intervālu (Windows).</span><span class="sxs-lookup"><span data-stu-id="0d809-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="0d809-118">Datorā palaidiet Windows Powershell, kur notiek avārija, un izpildiet šādas komandas:</span><span class="sxs-lookup"><span data-stu-id="0d809-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="0d809-119">Pievienojiet failu savam atbalsta pieteikumam.</span><span class="sxs-lookup"><span data-stu-id="0d809-119">Attach the file to your support case.</span></span>
