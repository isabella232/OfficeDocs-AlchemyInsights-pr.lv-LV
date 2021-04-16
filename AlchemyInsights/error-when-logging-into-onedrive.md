---
title: 0x8004de40 kļūda, palaižot OneDrive
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
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813659"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="0db2e-102">0x8004de40 kļūda, palaižot OneDrive</span><span class="sxs-lookup"><span data-stu-id="0db2e-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="0db2e-103">Ja, piesakoties **pakalpojumā** OneDrive, 0x8004de40 kļūda, restartējiet datoru, kamēr ir izveidots savienojums ar darba vai mācību domēnu.</span><span class="sxs-lookup"><span data-stu-id="0db2e-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="0db2e-104">Ja pēc atkārtotas palaišanas tiek parādīta šāda kļūda, mēģiniet to veikt, kamēr ir izveidots savienojums ar darba vai mācību domēnu.</span><span class="sxs-lookup"><span data-stu-id="0db2e-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="0db2e-105">Noklikšķiniet uz Sākt un  meklēšanas **lodziņā ierakstiet cmd** vai komandu uzvedne, ar peles labo pogu noklikšķiniet uz komandu uzvednes lietojumprogrammas un atlasiet Palaist **kā administratoram.**</span><span class="sxs-lookup"><span data-stu-id="0db2e-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator**.</span></span> <span data-ttu-id="0db2e-106">Ja saņemat aicinājumu ierakstīt administratora paroli vai apstiprinājumu, ierakstiet paroli vai noklikšķiniet uz **Atļaut**.</span><span class="sxs-lookup"><span data-stu-id="0db2e-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow**.</span></span>  

2. <span data-ttu-id="0db2e-107">Komandu uzvednes logā ierakstiet **dsregcmd /leave un**  gaidiet, līdz komanda tiek pabeigta.</span><span class="sxs-lookup"><span data-stu-id="0db2e-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="0db2e-108">Pēc tam **ierakstiet dsregcmd /join un** gaidiet, līdz komanda tiek pabeigta.</span><span class="sxs-lookup"><span data-stu-id="0db2e-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="0db2e-109">Restartējiet datoru.</span><span class="sxs-lookup"><span data-stu-id="0db2e-109">Reboot your computer.</span></span>
