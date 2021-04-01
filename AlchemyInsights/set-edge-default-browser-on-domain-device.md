---
title: Microsoft Edge iestatīšana par noklusējuma pārlūkprogrammu domēnā savienotā ierīcē
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491582"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a><span data-ttu-id="7b41c-102">Microsoft Edge iestatīšana par noklusējuma pārlūkprogrammu domēnā savienotā ierīcē</span><span class="sxs-lookup"><span data-stu-id="7b41c-102">Set Microsoft Edge as the default browser on a domain-joined device</span></span>

<span data-ttu-id="7b41c-103">Iestatiet Microsoft Edge kā noklusējuma pārlūkprogrammu.</span><span class="sxs-lookup"><span data-stu-id="7b41c-103">Set Microsoft Edge as the default browser:</span></span> 

1. <span data-ttu-id="7b41c-104">[Izveidojiet noklusējuma saistību konfigurācijas failu](https://go.microsoft.com/fwlink/?linkid=2132437) un saglabājiet to lokāli vai tīkla koplietojumā.</span><span class="sxs-lookup"><span data-stu-id="7b41c-104">[Create a default associations configuration file](https://go.microsoft.com/fwlink/?linkid=2132437) and store it locally or on a network share.</span></span>

1. <span data-ttu-id="7b41c-105">Atveriet grupas politikas redaktoru un pēc tam dodieties uz sadaļu **Datora konfigurācijas**  >  **administratīvās veidnes** Windows  >  **komponentu**  >  **failu pārlūks.**</span><span class="sxs-lookup"><span data-stu-id="7b41c-105">Open the Group Policy editor, and then go to **Computer Configuration** > **Administrative Templates** > **Windows Components** > **File Explorer**.</span></span>

1. <span data-ttu-id="7b41c-106">Atlasiet **Noklusējuma saistību konfigurācijas faila iestatīšana**.</span><span class="sxs-lookup"><span data-stu-id="7b41c-106">Select **Set a default associations configuration file**.</span></span>

1. <span data-ttu-id="7b41c-107">Atlasiet **Politikas iestatījums** un pēc tam atlasiet **Iespējots**.</span><span class="sxs-lookup"><span data-stu-id="7b41c-107">Select **Policy setting**, and then select **Enabled**.</span></span>

1. <span data-ttu-id="7b41c-108">Sadaļā **Opcijas** ievadiet noklusējuma saistību konfigurācijas faila atrašanās vietu un pēc tam atlasiet **Labi**.</span><span class="sxs-lookup"><span data-stu-id="7b41c-108">Under **Options**, enter the location of your default associations configuration file, and then select **OK**.</span></span>
