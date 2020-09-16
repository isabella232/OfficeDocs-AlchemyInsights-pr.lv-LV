---
title: Bluetooth problēmu novēršana operētājsistēmā Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001475"
- "3506"
ms.openlocfilehash: 7e7a397a1f6777972a81bcbb6bffa1c98d8370a4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730166"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="e57a6-102">Bluetooth problēmu novēršana operētājsistēmā Windows 10</span><span class="sxs-lookup"><span data-stu-id="e57a6-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="e57a6-103">Ja trūkst Bluetooth ikonas vai Bluetooth nevar ieslēgt vai izslēgt, iespējams, vēlēsities palaist Bluetooth problēmu risinātāju.</span><span class="sxs-lookup"><span data-stu-id="e57a6-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="e57a6-104">[Atveriet problēmu novēršanas iestatījumus](ms-settings:troubleshoot), noklikšķiniet uz **Bluetooth** sadaļā **atrast un labot citas problēmas**, noklikšķiniet uz **palaist problēmu risinātāju**.</span><span class="sxs-lookup"><span data-stu-id="e57a6-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="e57a6-105">Ja netiek rādīta Bluetooth ikona, bet Bluetooth funkcija ir redzama ierīču pārvaldniekā:</span><span class="sxs-lookup"><span data-stu-id="e57a6-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="e57a6-106">Ierīču pārvaldniekā noklikšķiniet uz **Bluetooth**.</span><span class="sxs-lookup"><span data-stu-id="e57a6-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="e57a6-107">Nospiediet un turiet nospiestu (vai noklikšķiniet ar peles labo pogu) uz Bluetooth adaptera nosaukuma un noklikšķiniet uz **atinstalēt ierīci**.</span><span class="sxs-lookup"><span data-stu-id="e57a6-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="e57a6-108">Beidzējiet Windows ierīci, uzgaidiet dažas sekundes un pēc tam atkal ieslēdziet to.</span><span class="sxs-lookup"><span data-stu-id="e57a6-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="e57a6-109">Windows mēģinās atkārtoti instalēt draiveri.</span><span class="sxs-lookup"><span data-stu-id="e57a6-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="e57a6-110">Ja nesen instalējāt Windows 10 atjauninājumus vai jauninājāt uz Windows 10, iespējams, vēlēsities meklēt draiveru atjauninājumus.</span><span class="sxs-lookup"><span data-stu-id="e57a6-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="e57a6-111">Ierīču pārvaldniekā noklikšķiniet uz **Bluetooth**un pēc tam noklikšķiniet uz Bluetooth adaptera nosaukuma (tas var ietvert vārdu "radio").</span><span class="sxs-lookup"><span data-stu-id="e57a6-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="e57a6-112">Nospiediet un turiet Bluetooth adapteri (vai noklikšķiniet ar peles labo pogu) un pēc tam noklikšķiniet uz **atjaunināt draiveru**  >  **meklēšanu automātiski, lai atjauninātu draivera programmatūru**.</span><span class="sxs-lookup"><span data-stu-id="e57a6-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="e57a6-113">Izpildiet norādītās darbības un pēc tam noklikšķiniet uz **izslēgt**.</span><span class="sxs-lookup"><span data-stu-id="e57a6-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="e57a6-114">Ja operētājsistēma Windows neatrod jaunu Bluetooth draiveri, apmeklējiet datora ražotāja tīmekļa vietni un lejupielādējiet jaunāko Bluetooth draiveri no šīs vietas.</span><span class="sxs-lookup"><span data-stu-id="e57a6-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="e57a6-115">Pēc lejupielādes noklikšķiniet uz **Atjaunināt draiveri**  >  **datorā, lai atrastu draivera programmatūru**  >  **pārlūkojiet** vietu, kur ir saglabāti draiveru faili > **Labi**  >  **Next**, un izpildiet instalēšanas darbības.</span><span class="sxs-lookup"><span data-stu-id="e57a6-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="e57a6-116">Pēc atjauninātā draivera instalēšanas restartējiet datoru un pārbaudiet, vai tas novērš savienojuma problēmu.</span><span class="sxs-lookup"><span data-stu-id="e57a6-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="e57a6-117">Papildinformāciju par to, kā novērst Bluetooth problēmas, skatiet rakstā Viss raksts, [ar Bluetooth saistītu problēmu](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems)novēršana operētājsistēmā Windows 10.</span><span class="sxs-lookup"><span data-stu-id="e57a6-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
