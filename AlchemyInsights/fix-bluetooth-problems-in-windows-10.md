---
title: Bluetooth problēmu novēršana operētājsistēmā Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001475"
- "3506"
ms.openlocfilehash: 94dda7a42632f57ce3aef5f467b87df1033b8d49
ms.sourcegitcommit: 9a35768444824cde9e192f1d9daafc9157437244
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/25/2020
ms.locfileid: "42268639"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="61ffe-102">Bluetooth problēmu novēršana operētājsistēmā Windows 10</span><span class="sxs-lookup"><span data-stu-id="61ffe-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="61ffe-103">Ja trūkst Bluetooth ikonas vai Bluetooth nevar ieslēgt vai izslēgt, iespējams, vēlēsities palaist Bluetooth problēmu risinātāju.</span><span class="sxs-lookup"><span data-stu-id="61ffe-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="61ffe-104">[Atveriet problēmu novēršanas iestatījumus](ms-settings:troubleshoot), noklikšķiniet uz **Bluetooth** sadaļā **atrast un novērst citas problēmas**noklikšķiniet uz **palaist problēmu risinātāju**.</span><span class="sxs-lookup"><span data-stu-id="61ffe-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="61ffe-105">Ja Bluetooth ikona nav redzama, tomēr ierīču pārvaldniekā tiek parādīts Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="61ffe-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="61ffe-106">Ierīču pārvaldniekā noklikšķiniet uz **Bluetooth**.</span><span class="sxs-lookup"><span data-stu-id="61ffe-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="61ffe-107">Nospiediet un turiet (vai noklikšķiniet ar peles labo pogu) Bluetooth adaptera nosaukumu un noklikšķiniet uz **atinstalēt ierīci**.</span><span class="sxs-lookup"><span data-stu-id="61ffe-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="61ffe-108">Izslēdziet Windows ierīci, pagaidiet dažas sekundes un pēc tam atkal ieslēdziet to.</span><span class="sxs-lookup"><span data-stu-id="61ffe-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="61ffe-109">Sistēma Windows mēģinās pārinstalēt draiveri.</span><span class="sxs-lookup"><span data-stu-id="61ffe-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="61ffe-110">Ja nesen instalējāt Windows 10 atjauninājumus vai veicāt jaunināšanu uz Windows 10, iespējams, vēlēsities pārbaudīt draiveru atjauninājumus:</span><span class="sxs-lookup"><span data-stu-id="61ffe-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="61ffe-111">Ierīču pārvaldniekā noklikšķiniet uz **Bluetooth**un pēc tam uz Bluetooth adaptera nosaukuma (kas var ietvert vārdu "radio").</span><span class="sxs-lookup"><span data-stu-id="61ffe-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="61ffe-112">Nospiediet un turiet Bluetooth adapteri (vai noklikšķiniet uz tā ar peles labo pogu) un pēc tam noklikšķiniet uz **Atjaunināt draivera** > **meklēšanu automātiski atjauninātai draivera programmatūrai**.</span><span class="sxs-lookup"><span data-stu-id="61ffe-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="61ffe-113">Izpildiet norādījumus un pēc tam noklikšķiniet uz **Aizvērt**.</span><span class="sxs-lookup"><span data-stu-id="61ffe-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="61ffe-114">Ja Windows nevar atrast jaunu Bluetooth draiveri, apmeklējiet datora ražotāja vietni un lejupielādējiet jaunāko Bluetooth draiveri no turienes.</span><span class="sxs-lookup"><span data-stu-id="61ffe-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="61ffe-115">Pēc tās lejupielādes noklikšķiniet uz **Atjaunināt draiveri** > **Meklēt datorā draivera programmatūru** > **atrodiet** atrašanās vietu, kur glabājas draivera faili > **Labi** > **blakus**, un veiciet norādītās darbības, lai to instalētu.</span><span class="sxs-lookup"><span data-stu-id="61ffe-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="61ffe-116">Pēc atjauninātā draivera instalēšanas restartējiet datoru un pēc tam pārbaudiet, vai savienojuma problēma tiek novērsta.</span><span class="sxs-lookup"><span data-stu-id="61ffe-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="61ffe-117">Lai iegūtu plašāku informāciju par to, kā novērst Bluetooth problēmas, lūdzu, skatiet pilnu rakstu, [novērst Bluetooth problēmas operētājsistēmā Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span><span class="sxs-lookup"><span data-stu-id="61ffe-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
