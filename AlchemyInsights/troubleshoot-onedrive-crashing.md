---
title: OneDrive avāriju problēmu novēršana
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/15/2020
ms.locfileid: "44749161"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="8226c-102">OneDrive avāriju problēmu novēršana</span><span class="sxs-lookup"><span data-stu-id="8226c-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="8226c-103">Ja OneDrive atkārtoti avarē, veiciet tālāk norādītās problēmu novēršanas darbības.</span><span class="sxs-lookup"><span data-stu-id="8226c-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="8226c-104">**Pārliecinieties, vai reģistra atslēgas nav iestatītas:**</span><span class="sxs-lookup"><span data-stu-id="8226c-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="8226c-105">Izmantojot reģistra redaktoru, naviģējiet uz HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="8226c-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="8226c-106">Ja DisableFileSyncNGSC ir un iestatīts uz 1, atveriet atslēgu un mainiet vērtību uz 0.</span><span class="sxs-lookup"><span data-stu-id="8226c-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="8226c-107">Manuāli palaist OneDrive, dodoties uz sākuma ekrāna</span><span class="sxs-lookup"><span data-stu-id="8226c-107">Manually launch OneDrive by going to Start</span></span> ![Nospiediet Windows taustiņu](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="8226c-109">, meklēšanas lodziņā ierakstiet OneDrive un pēc tam noklikšķiniet uz OneDrive datora lietojumprogrammas.</span><span class="sxs-lookup"><span data-stu-id="8226c-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="8226c-110">**OneDrive atiestatīšana:**</span><span class="sxs-lookup"><span data-stu-id="8226c-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="8226c-111">Piezīmes:</span><span class="sxs-lookup"><span data-stu-id="8226c-111">Notes:</span></span>

- <span data-ttu-id="8226c-112">OneDrive atiestatīšana atvieno visus esošos sinhronizācijas savienojumus (tostarp personisko OneDrive, ja tas ir iestatīts).</span><span class="sxs-lookup"><span data-stu-id="8226c-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="8226c-113">Jūs nezaudēsit failus vai datus, atiestatot OneDrive datorā.</span><span class="sxs-lookup"><span data-stu-id="8226c-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="8226c-114">**Lai atiestatītu OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="8226c-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="8226c-115">Atveriet dialoglodziņu Izpildīt, nospiežot Windows taustiņu un R.</span><span class="sxs-lookup"><span data-stu-id="8226c-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="8226c-116">Ierakstiet %localappdata%\Microsoft\OneDrive\onedrive.exe /reset un nospiediet Labi.</span><span class="sxs-lookup"><span data-stu-id="8226c-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="8226c-117">Uz īsu brīdi var parādīties komandlogs.</span><span class="sxs-lookup"><span data-stu-id="8226c-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="8226c-118">Manuāli palaist OneDrive, dodoties uz sākuma ekrāna</span><span class="sxs-lookup"><span data-stu-id="8226c-118">Manually launch OneDrive by going to Start</span></span> ![Nospiediet Windows taustiņu](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="8226c-120">, meklēšanas lodziņā ierakstiet OneDrive un pēc tam noklikšķiniet uz OneDrive datora lietojumprogrammas.</span><span class="sxs-lookup"><span data-stu-id="8226c-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="8226c-121">Piezīmes:</span><span class="sxs-lookup"><span data-stu-id="8226c-121">Notes:</span></span>

- <span data-ttu-id="8226c-122">Ja pirms atiestatīšanas esat izvēlējies sinhronizēt tikai dažas mapes, pēc sinhronizācijas pabeigšanas tas būs jādara vēlreiz.</span><span class="sxs-lookup"><span data-stu-id="8226c-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="8226c-123">Lai [iegūtu papildinformāciju, izlasiet rakstu Izvēlieties, kuras OneDrive](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   mapes sinhronizēt ar datoru.</span><span class="sxs-lookup"><span data-stu-id="8226c-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="8226c-124">Tas ir jāaizpilda personiskajam OneDrive un OneDrive darbam.</span><span class="sxs-lookup"><span data-stu-id="8226c-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>