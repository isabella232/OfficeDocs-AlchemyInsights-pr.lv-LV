---
title: OneDrive avarēšanu novēršana
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
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826206"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="7ca4e-102">OneDrive avarēšanu novēršana</span><span class="sxs-lookup"><span data-stu-id="7ca4e-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="7ca4e-103">Ja OneDrive atkārtoti avarē, izmēģiniet šīs problēmu novēršanas darbības:</span><span class="sxs-lookup"><span data-stu-id="7ca4e-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="7ca4e-104">**Pārliecinieties, vai reģistra atslēgas nav iestatītas:**</span><span class="sxs-lookup"><span data-stu-id="7ca4e-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="7ca4e-105">Izmantojot reģistra redaktoru, naviģējiet uz HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="7ca4e-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="7ca4e-106">Ja parametra DisableFileSyncNGSC vērtība ir 1, atveriet atslēgu un mainiet vērtību uz 0.</span><span class="sxs-lookup"><span data-stu-id="7ca4e-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="7ca4e-107">Manuāla OneDrive palaišana, dodoties uz sākumu</span><span class="sxs-lookup"><span data-stu-id="7ca4e-107">Manually launch OneDrive by going to Start</span></span> ![Nospiediet Windows taustiņu](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="7ca4e-109">, meklēšanas lodziņā ierakstiet OneDrive un pēc tam noklikšķiniet uz OneDrive datora programmas.</span><span class="sxs-lookup"><span data-stu-id="7ca4e-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="7ca4e-110">**OneDrive atiestatīšana:**</span><span class="sxs-lookup"><span data-stu-id="7ca4e-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="7ca4e-111">Piezīmes.</span><span class="sxs-lookup"><span data-stu-id="7ca4e-111">Notes:</span></span>

- <span data-ttu-id="7ca4e-112">OneDrive atiestatīšana atvieno visus esošos sinhronizācijas savienojumus (ieskaitot OneDrive individuālai lietošanai, ja tas ir iestatīts).</span><span class="sxs-lookup"><span data-stu-id="7ca4e-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="7ca4e-113">Datorā atiestatot OneDrive, jūs nezaudēsit failus vai datus.</span><span class="sxs-lookup"><span data-stu-id="7ca4e-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="7ca4e-114">**Lai atiestatītu OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="7ca4e-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="7ca4e-115">Atveriet izpildes dialoglodziņu, nospiežot Windows taustiņu un R.</span><span class="sxs-lookup"><span data-stu-id="7ca4e-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="7ca4e-116">Ierakstiet %localappdata%\Microsoft\OneDrive\onedrive.exe /reset un nospiediet Labi.</span><span class="sxs-lookup"><span data-stu-id="7ca4e-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="7ca4e-117">Var īslaicīgi parādīties komandu logs.</span><span class="sxs-lookup"><span data-stu-id="7ca4e-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="7ca4e-118">Manuāla OneDrive palaišana, dodoties uz sākumu</span><span class="sxs-lookup"><span data-stu-id="7ca4e-118">Manually launch OneDrive by going to Start</span></span> ![Nospiediet Windows taustiņu](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="7ca4e-120">, meklēšanas lodziņā ierakstiet OneDrive un pēc tam noklikšķiniet uz OneDrive datora programmas.</span><span class="sxs-lookup"><span data-stu-id="7ca4e-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="7ca4e-121">Piezīmes.</span><span class="sxs-lookup"><span data-stu-id="7ca4e-121">Notes:</span></span>

- <span data-ttu-id="7ca4e-122">Ja pirms atiestatīšanas izvēlējāties sinhronizēt tikai dažas mapes, to vajadzēs izdarīt vēlreiz (pēc tam, kad būs pabeigta sinhronizācija).</span><span class="sxs-lookup"><span data-stu-id="7ca4e-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="7ca4e-123"> [Papildinformāciju skatiet rakstu Ar datoru sinhronizējamo OneDrive](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)mapju   izvēlēšana.</span><span class="sxs-lookup"><span data-stu-id="7ca4e-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="7ca4e-124">Šīs darbības būs jāveic personiskajam OneDrive un OneDrive darbam.</span><span class="sxs-lookup"><span data-stu-id="7ca4e-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>