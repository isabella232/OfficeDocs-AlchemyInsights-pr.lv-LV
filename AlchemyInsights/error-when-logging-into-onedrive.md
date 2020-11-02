---
title: 0x8004de40 kļūda, palaižot OneDrive
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
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823052"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="b9fed-102">0x8004de40 kļūda, palaižot OneDrive</span><span class="sxs-lookup"><span data-stu-id="b9fed-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="b9fed-103">Ja, pierakstoties pakalpojumā OneDrive, saņemat kļūdas ziņojumu **0x8004de40** , restartējiet datoru, kamēr ir izveidots savienojums ar darba vai mācību iestādes domēnu.</span><span class="sxs-lookup"><span data-stu-id="b9fed-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="b9fed-104">Ja pēc atsāknēšanas saņemat šo kļūdu, izmēģiniet to, kamēr ir izveidots savienojums ar darba vai mācību iestādes domēnu:</span><span class="sxs-lookup"><span data-stu-id="b9fed-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="b9fed-105">Noklikšķiniet uz Sākt un meklēšanas lodziņā ierakstiet **cmd** vai **komandu uzvedne**  , ar peles labo pogu noklikšķiniet uz komandu uzvednes lietojumprogrammas un atlasiet  **Palaist kā administratoram** .</span><span class="sxs-lookup"><span data-stu-id="b9fed-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator** .</span></span> <span data-ttu-id="b9fed-106">Ja tiek parādīta uzvedne ar aicinājumu ievadīt administratora paroli vai apstiprinājumu, ierakstiet paroli vai noklikšķiniet uz **Atļaut** .</span><span class="sxs-lookup"><span data-stu-id="b9fed-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow** .</span></span>  

2. <span data-ttu-id="b9fed-107">Komandu uzvednes logā ierakstiet **dsregcmd/Leave**  un uzgaidiet, līdz tiek pabeigta komanda.</span><span class="sxs-lookup"><span data-stu-id="b9fed-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="b9fed-108">Pēc tam ierakstiet **dsregcmd/Join** un uzgaidiet, līdz tiek pabeigta komanda.</span><span class="sxs-lookup"><span data-stu-id="b9fed-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="b9fed-109">Restartējiet datoru.</span><span class="sxs-lookup"><span data-stu-id="b9fed-109">Reboot your computer.</span></span>
