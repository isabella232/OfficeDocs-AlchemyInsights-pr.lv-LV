---
title: OneDrive avāriju problēmu novēršana
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665005"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="86b2c-102">OneDrive avāriju problēmu novēršana</span><span class="sxs-lookup"><span data-stu-id="86b2c-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="86b2c-103">Ja OneDrive vairākkārt avarē, izmēģiniet šīs problēmu novēršanas darbības:</span><span class="sxs-lookup"><span data-stu-id="86b2c-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="86b2c-104">**Pārliecinieties, vai nav iestatītas reģistra atslēgas:**</span><span class="sxs-lookup"><span data-stu-id="86b2c-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="86b2c-105">Izmantojot reģistra redaktoru, pārejiet uz HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="86b2c-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="86b2c-106">Ja DisableFileSyncNGSC ir klātesošs un iestatīts uz 1, atveriet atslēgu un mainiet vērtību uz 0.</span><span class="sxs-lookup"><span data-stu-id="86b2c-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="86b2c-107">Manuāli palaidiet OneDrive, dodoties uz sākumu</span><span class="sxs-lookup"><span data-stu-id="86b2c-107">Manually launch OneDrive by going to Start</span></span> ![Nospiediet Windows taustiņu](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="86b2c-109">, meklēšanas lodziņā ierakstiet OneDrive un pēc tam noklikšķiniet uz OneDrive datora lietojumprogrammas.</span><span class="sxs-lookup"><span data-stu-id="86b2c-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="86b2c-110">**OneDrive atiestatīšana:**</span><span class="sxs-lookup"><span data-stu-id="86b2c-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="86b2c-111">Piezīmes</span><span class="sxs-lookup"><span data-stu-id="86b2c-111">Notes:</span></span>

- <span data-ttu-id="86b2c-112">OneDrive atiestatīšana atveido visus esošos sinhronizācijas savienojumus (tostarp savu personisko OneDrive, ja tas ir iestatīts).</span><span class="sxs-lookup"><span data-stu-id="86b2c-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="86b2c-113">Jūs nezaudēsit failus vai datus, atiestatot OneDrive savā datorā.</span><span class="sxs-lookup"><span data-stu-id="86b2c-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="86b2c-114">**Lai atiestatītu OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="86b2c-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="86b2c-115">Atveriet palaišanas dialoglodziņu, nospiežot Windows taustiņu un R.</span><span class="sxs-lookup"><span data-stu-id="86b2c-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="86b2c-116">Ierakstiet% LOCALAPPDATA% \Microsoft\OneDrive\onedrive.exe/reset un nospiediet Labi.</span><span class="sxs-lookup"><span data-stu-id="86b2c-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="86b2c-117">Var īslaicīgi parādīties komandu logs.</span><span class="sxs-lookup"><span data-stu-id="86b2c-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="86b2c-118">Manuāli palaidiet OneDrive, dodoties uz sākumu</span><span class="sxs-lookup"><span data-stu-id="86b2c-118">Manually launch OneDrive by going to Start</span></span> ![Nospiediet Windows taustiņu](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="86b2c-120">, meklēšanas lodziņā ierakstiet OneDrive un pēc tam noklikšķiniet uz OneDrive datora lietojumprogrammas.</span><span class="sxs-lookup"><span data-stu-id="86b2c-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="86b2c-121">Piezīmes</span><span class="sxs-lookup"><span data-stu-id="86b2c-121">Notes:</span></span>

- <span data-ttu-id="86b2c-122">Ja izvēlējāties sinhronizēt tikai dažas mapes pirms atiestates, jums tā būs jāveic atkārtoti, kad sinhronizācija ir pabeigta.</span><span class="sxs-lookup"><span data-stu-id="86b2c-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="86b2c-123">Lai iegūtu papildinformāciju, izlasiet rakstu kā [izvēlēties, kuras OneDrive mapes sinhronizēt ar datoru](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   .</span><span class="sxs-lookup"><span data-stu-id="86b2c-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="86b2c-124">Šī darbība ir jāveic jūsu personiskajai OneDrive un OneDrive darbam.</span><span class="sxs-lookup"><span data-stu-id="86b2c-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>