---
title: 'Windows 10 trūkst enerģijas vai akumulatora ikonas '
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
- "9002953"
- "5655"
ms.openlocfilehash: 95b68cee58f88d04f02e29477b139f7f583dc0b1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790555"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a><span data-ttu-id="21624-102">Windows 10 trūkst enerģijas vai akumulatora ikonas </span><span class="sxs-lookup"><span data-stu-id="21624-102">Power or battery icon missing in Windows 10</span></span>

<span data-ttu-id="21624-103">Ja jūsu Windows 10 ierīce ir aprīkota ar akumulatoru (piem., klēpjdators vai planšetdators, vai dators, kas ar USB pieslēgts pie UPS ierīces), tad parasti enerģijas/akumulatora ikona ir redzama uzdevumjoslā, blakus pulkstenim, piemēram:</span><span class="sxs-lookup"><span data-stu-id="21624-103">If your Windows 10 device has a battery (e.g., laptop or tablet, or a PC connected via USB to a UPS), normally a power/battery icon is shown in the taskbar near the clock, for example:</span></span>

![Akumulatora ikona](media/battery-icon.png)

<span data-ttu-id="21624-105">Ja neredzat šo ikonu, tā var būt slēpta:</span><span class="sxs-lookup"><span data-stu-id="21624-105">If you don't see this icon, it may be hidden:</span></span>

1. <span data-ttu-id="21624-106">Dodieties uz **[Iestatījumi > Personalizēšana > Uzdevumjosla](ms-settings:taskbar?activationSource=GetHelp)**.</span><span class="sxs-lookup"><span data-stu-id="21624-106">Go to **[Settings > Personalization > Taskbar](ms-settings:taskbar?activationSource=GetHelp)**.</span></span>

2. <span data-ttu-id="21624-107">Paziņojumu apgabalā noklikšķiniet uz **Atlasīt ikonas, kas parādās uzdevumjoslā**.</span><span class="sxs-lookup"><span data-stu-id="21624-107">In the Notification area, click **Select which icons appear on the taskbar**.</span></span>

3. <span data-ttu-id="21624-108">Pēc tam sarakstā atrodiet vienumu **Enerģija** un pārslēdziet tā iestatījumu uz **Ieslēgts**.</span><span class="sxs-lookup"><span data-stu-id="21624-108">Then find the **Power** item in the list and toggle its setting to **On**.</span></span>

    ![Rādīt enerģijas ikonu uzdevumjoslā](media/power-icon-on.png)

<span data-ttu-id="21624-110">**Problēmu novēršana**</span><span class="sxs-lookup"><span data-stu-id="21624-110">**Troubleshooting**</span></span>

<span data-ttu-id="21624-111">Ja sekojāt norādījumiem augstāk un **Enerģijas** pārslēgšanas poga ir pelēkota vai nav redzama, meklēšanas joslā ierakstiet **ierīču pārvaldnieks** un rezultātu sarakstā atlasiet **Ierīču pārvaldnieks**.</span><span class="sxs-lookup"><span data-stu-id="21624-111">If you followed the above instructions and the **Power** toggle is greyed out or not visible, in the search box on the taskbar, type **device manager**, and then select **Device Manager** in the list of results.</span></span> <span data-ttu-id="21624-112">Sadaļā **Akumulatori** ar labo peles pogu noklikšķiniet uz jūsu ierīces akumulatora, pēc tam noklikšķiniet uz **Atspējot** un noklikšķiniet uz **Jā**.</span><span class="sxs-lookup"><span data-stu-id="21624-112">Under **Batteries**, right-click the battery for your device, click **Disable**, and click **Yes**.</span></span> <span data-ttu-id="21624-113">Uzgaidiet pāris sekundes, pēc tam ar labo peles pogu noklikšķiniet uz akumulatora un noklikšķiniet uz **Iespējot**.</span><span class="sxs-lookup"><span data-stu-id="21624-113">Wait a few seconds, and then right-click the battery and click **Enable**.</span></span> <span data-ttu-id="21624-114">Pēc tam restartējiet savu ierīci.</span><span class="sxs-lookup"><span data-stu-id="21624-114">Then restart your device.</span></span>

<span data-ttu-id="21624-115">Ja sekojāt norādījumiem augstāk, bet akumulatora ikona joprojām neparādās uzdevumjoslā, tad uzdevumjoslas meklēšanas laukā ierakstiet **uzdevumu pārvaldnieks** un pēc tam rezultātu sarakstā noklikšķiniet uz **Uzdevumu pārvaldnieks**.</span><span class="sxs-lookup"><span data-stu-id="21624-115">If you followed the above instructions, but the battery icon does not appear on the taskbar, in the search box on the taskbar, type **task manager**, and then click **Task Manager** in the list of results.</span></span> <span data-ttu-id="21624-116">Cilnē **Procesi**, sadaļā **Nosaukums**, ar labo peles pogu noklikšķiniet uz **Pārlūks** un pēc tam noklikšķiniet uz **Restartēt**.</span><span class="sxs-lookup"><span data-stu-id="21624-116">On the **Processes** tab, under **Name**, right-click **Explorer**, and then click **Restart**.</span></span>
