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
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030681"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="773e8-102">Vai Teams klients avarē?</span><span class="sxs-lookup"><span data-stu-id="773e8-102">Teams client crashing?</span></span>

<span data-ttu-id="773e8-103">Ja jūsu Teams klients avarē, mēģiniet veikt tālāk norādītās darbības:</span><span class="sxs-lookup"><span data-stu-id="773e8-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="773e8-104">Ja izmantojat Teams datora programmu, [pārliecinieties, vai programma ir pilnībā atjaunināta](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="773e8-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="773e8-105">Pārliecinieties, vai ir pieejami visi [Office 365 URL un adrešu diapazoni](https://docs.microsoft.com/microsoftteams/connectivity-issues).</span><span class="sxs-lookup"><span data-stu-id="773e8-105">Make sure all the [Office 365 URL's and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="773e8-106">Piesakieties ar savu administratora kontu un pārbaudiet [Pakalpojumu darbspējas informācijas panelis](https://docs.microsoft.com/office365/enterprise/view-service-health), vai nav dīkstāves vai pakalpojuma degradācijas.</span><span class="sxs-lookup"><span data-stu-id="773e8-106">Log in with your admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

 - <span data-ttu-id="773e8-107">Pēdējā darbības solī varat mēģināt iztīrīt savu Teams klienta kešatmiņu:</span><span class="sxs-lookup"><span data-stu-id="773e8-107">As a last step, you can attempt to clear your Teams client cache:</span></span>

    1.  <span data-ttu-id="773e8-108">Pilnībā aizveriet Microsoft Teams darbvirsmas klientu.</span><span class="sxs-lookup"><span data-stu-id="773e8-108">Fully exit the Microsoft Teams desktop client.</span></span> <span data-ttu-id="773e8-109">Varat ar peles labo pogu noklikšķināt **Teams** no ikonu teknes un noklikšķināt uz **Aizvērt**vai palaist uzdevumu pārvaldnieku un pilnībā apturēt procesu.</span><span class="sxs-lookup"><span data-stu-id="773e8-109">You can right-click **Teams** from the Icon Tray and click **Quit**, or run Task Manager and fully kill the process.</span></span>

    2.  <span data-ttu-id="773e8-110">Dodieties uz failu pārlūku un ierakstiet %appdata%\Microsoft\teams.</span><span class="sxs-lookup"><span data-stu-id="773e8-110">Go to File Explorer, and type in %appdata%\Microsoft\teams.</span></span>

    3.  <span data-ttu-id="773e8-111">Kad būsiet direktorijā, jūs redzēsiet dažas no tālāk norādītajām mapēm:</span><span class="sxs-lookup"><span data-stu-id="773e8-111">Once in the directory, you'll see a few of the following folders:</span></span>

         - <span data-ttu-id="773e8-112">Sadaļā **Programmas kešatmiņa**, atveriet kešatmiņu un izdzēsiet jebkurus no failiem kešatmiņas atrašanās vietā: %appdata%\Microsoft\teams\application cache\cache.</span><span class="sxs-lookup"><span data-stu-id="773e8-112">From within **Application Cache**, go to Cache and delete any of the files in the Cache location:  %appdata%\Microsoft\teams\application cache\cache.</span></span>

        - <span data-ttu-id="773e8-113">Sadaļā **Blob_storage**izdzēsiet visus failus: %appdata%\Microsoft\teams\ blob_storage.</span><span class="sxs-lookup"><span data-stu-id="773e8-113">From within **Blob_storage**, delete all files: %appdata%\Microsoft\teams\blob_storage.</span></span>

        - <span data-ttu-id="773e8-114">Sadaļā **Kešatmiņa**izdzēsiet visus failus: %appdata%\Microsoft\teams\Cache.</span><span class="sxs-lookup"><span data-stu-id="773e8-114">From within **Cache**, delete all files: %appdata%\Microsoft\teams\Cache.</span></span>

        - <span data-ttu-id="773e8-115">Sadaļā **datubāzes**izdzēsiet visus failus: %appdata%\Microsoft\teams\databases.</span><span class="sxs-lookup"><span data-stu-id="773e8-115">From within **databases**, delete all files: %appdata%\Microsoft\teams\databases.</span></span>

        - <span data-ttu-id="773e8-116">Sadaļā **GPU kešatmiņa**izdzēsiet visus failus: %appdata%\Microsoft\teams\GPUcache.</span><span class="sxs-lookup"><span data-stu-id="773e8-116">From within **GPUCache**, delete all files: %appdata%\Microsoft\teams\GPUcache.</span></span>

        - <span data-ttu-id="773e8-117">Sadaļā **IndexedDB**izdzēsiet .db failu: %appdata%\Microsoft\teams\IndexedDB.</span><span class="sxs-lookup"><span data-stu-id="773e8-117">From within **IndexedDB**, delete the .db file: %appdata%\Microsoft\teams\IndexedDB.</span></span>

        - <span data-ttu-id="773e8-118">Sadaļā **Lokālā krātuve**izdzēsiet visus failus: %appdata%\Microsoft\teams\Local Storage.</span><span class="sxs-lookup"><span data-stu-id="773e8-118">From within **Local Storage**, delete all files: %appdata%\Microsoft\teams\Local Storage.</span></span>

        - <span data-ttu-id="773e8-119">Visbeidzot **tmp**izdzēsiet jebkuru failu: %appdata%\Microsoft\teams\tmp.</span><span class="sxs-lookup"><span data-stu-id="773e8-119">Lastly, from within **tmp**, delete any file: %appdata%\Microsoft\teams\tmp.</span></span>

    4. <span data-ttu-id="773e8-120">Restartējiet Teams klientu.</span><span class="sxs-lookup"><span data-stu-id="773e8-120">Restart your Teams client.</span></span>
