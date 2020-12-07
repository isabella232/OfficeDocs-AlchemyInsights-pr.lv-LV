---
title: Microsoft Edge politikas iestatījumu konfigurēšana operētājsistēmā Windows
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003845"
- "6894"
ms.openlocfilehash: 7f626152c3833638436dfe05e8dcd13fc86ef594
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583445"
---
# <a name="configure-microsoft-edge-policy-settings-on-windows"></a><span data-ttu-id="d2dd7-102">Microsoft Edge politikas iestatījumu konfigurēšana operētājsistēmā Windows</span><span class="sxs-lookup"><span data-stu-id="d2dd7-102">Configure Microsoft Edge policy settings on Windows</span></span>

<span data-ttu-id="d2dd7-103">Lai konfigurētu politikas iestatījumus un Microsoft Edge pārvaldītos atjauninājumus, izmantojiet grupas politikas objektus (GPO).</span><span class="sxs-lookup"><span data-stu-id="d2dd7-103">To configure policy settings and managed updates for Microsoft Edge, use Group Policy Objects (GPOs).</span></span> <span data-ttu-id="d2dd7-104">Varat arī nodrošināt politiku, izmantojot reģistru. tas būtu piemērots (1) Windows ierīces, kas pievienotas Microsoft Active Directory domēnam, un (2) Windows 10 Pro un Enterprise instances, kuras ir piereģistrētas ierīču pārvaldībai pakalpojumā Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="d2dd7-104">You can also provision policy through the registry; this would be appropriate for (1) Windows devices joined to a Microsoft Active Directory domain and for (2) Windows 10 Pro and Enterprise instances enrolled for device management in Microsoft Intune.</span></span>

<span data-ttu-id="d2dd7-105">Lai konfigurētu Microsoft Edge, izmantojot GPO, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="d2dd7-105">To configure Microsoft Edge by using GPOs, do the following:</span></span>

1. <span data-ttu-id="d2dd7-106">Grupas politikas centrālā krātuve savā Active Directory domēnā vai politikas definēšanas veidnes mapē atsevišķos datoros, instalējiet visas administratīvās veidnes, kas pievieno kārtulu un Microsoft Edge iestatījumus.</span><span class="sxs-lookup"><span data-stu-id="d2dd7-106">To the Group Policy Central Store in your Active Directory domain, or to the Policy Definition template folder on individual computers, install all administrative templates that add rules and settings for Microsoft Edge.</span></span>
2. <span data-ttu-id="d2dd7-107">Konfigurējiet konkrētās politikas, ko vēlaties iestatīt.</span><span class="sxs-lookup"><span data-stu-id="d2dd7-107">Configure the specific policies you want to set.</span></span>

<span data-ttu-id="d2dd7-108">Papildinformāciju skatiet rakstā [Microsoft Edge politikas iestatījumu konfigurēšana](https://go.microsoft.com/fwlink/?linkid=2135024)operētājsistēmā Windows.</span><span class="sxs-lookup"><span data-stu-id="d2dd7-108">To learn more, see [Configure Microsoft Edge policy settings on Windows](https://go.microsoft.com/fwlink/?linkid=2135024).</span></span>
