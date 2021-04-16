---
title: Bluetooth problēmu novēršana operētājsistēmā Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001475"
- "3506"
ms.openlocfilehash: f20bf4a642e019c7901e988a027e0220f0f1b07b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812939"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="bc8c1-102">Bluetooth problēmu novēršana operētājsistēmā Windows 10</span><span class="sxs-lookup"><span data-stu-id="bc8c1-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="bc8c1-103">Ja trūkst Bluetooth ikonas vai Tehnoloģiju Bluetooth nevar ieslēgt vai izslēgt, varat palaist Bluetooth problēmu risinātāju.</span><span class="sxs-lookup"><span data-stu-id="bc8c1-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="bc8c1-104">[Sadaļā Atrast un novērst citas](ms-settings:troubleshoot)problēmas atveriet problēmu novēršanas **iestatījumus** un noklikšķiniet uz **Bluetooth** , noklikšķiniet uz Palaist **problēmu risinātāju**.</span><span class="sxs-lookup"><span data-stu-id="bc8c1-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="bc8c1-105">Ja neredzat Bluetooth ikonu, bet Bluetooth tiek rādīta ierīču pārvaldniekā:</span><span class="sxs-lookup"><span data-stu-id="bc8c1-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="bc8c1-106">Ierīču pārvaldniekā noklikšķiniet uz **Bluetooth**.</span><span class="sxs-lookup"><span data-stu-id="bc8c1-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="bc8c1-107">Nospiediet un turiet Bluetooth adaptera nosaukumu (vai noklikšķiniet uz tā ar peles labo pogu) un noklikšķiniet uz **Atinstalēt ierīci**.</span><span class="sxs-lookup"><span data-stu-id="bc8c1-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="bc8c1-108">Izslēdziet Windows ierīci, uzgaidiet dažas sekundes un pēc tam ieslēdziet to.</span><span class="sxs-lookup"><span data-stu-id="bc8c1-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="bc8c1-109">Windows mēģinās atkārtoti instalēt draiveri.</span><span class="sxs-lookup"><span data-stu-id="bc8c1-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="bc8c1-110">Ja nesen instalējāt Windows 10 atjauninājumus vai veicāt jaunināšanu uz operētājsistēmu Windows 10, iespējams, vēlēsities pārbaudīt, vai nav draivera atjauninājumu.</span><span class="sxs-lookup"><span data-stu-id="bc8c1-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="bc8c1-111">Sadaļā Ierīču pārvaldnieks noklikšķiniet uz **Bluetooth** un pēc tam noklikšķiniet uz Bluetooth adaptera nosaukuma (kas var ietvert vārdu "radio").</span><span class="sxs-lookup"><span data-stu-id="bc8c1-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="bc8c1-112">Nospiediet un turiet Bluetooth adapteri (vai noklikšķiniet uz tā ar peles labo pogu) un pēc tam noklikšķiniet uz Atjaunināt draivera  >  **meklēšanu automātiski, lai iegūtu atjauninātu draivera programmatūru.**</span><span class="sxs-lookup"><span data-stu-id="bc8c1-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="bc8c1-113">Izpildiet darbības un pēc tam noklikšķiniet uz **Aizvērt.**</span><span class="sxs-lookup"><span data-stu-id="bc8c1-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="bc8c1-114">Ja operētājsistēma Windows nevar atrast jaunu Bluetooth draiveri, apmeklējiet datora ražotāja tīmekļa vietni un lejupielādējiet jaunāko Bluetooth draiveri no šīs vietas.</span><span class="sxs-lookup"><span data-stu-id="bc8c1-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="bc8c1-115">Pēc lejupielādes noklikšķiniet uz Atjaunināt draiveri Meklēt datorā draivera programmatūru. Pārlūkojiet vietu, kur tiek glabāti draivera faili, un pēc tam > Labi Tālāk un izpildiet norādījumus, lai  >    >     >  instalētu.</span><span class="sxs-lookup"><span data-stu-id="bc8c1-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="bc8c1-116">Pēc atjauninātā draivera instalēšanas restartējiet datoru un pārbaudiet, vai tas novērš savienojuma problēmu.</span><span class="sxs-lookup"><span data-stu-id="bc8c1-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="bc8c1-117">Lai iegūtu papildinformāciju par to, kā novērst ar Bluetooth saistītas problēmas, skatiet pilnu rakstu [Bluetooth problēmu novēršana operētājsistēmā Windows 10.](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems)</span><span class="sxs-lookup"><span data-stu-id="bc8c1-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
