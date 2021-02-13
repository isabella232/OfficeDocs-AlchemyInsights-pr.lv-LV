---
title: Microsoft Edge pievienošana Microsoft Intune
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8240"
- "9004604"
ms.openlocfilehash: d56c65910d1c2170d3e0ce9676e913663701db96
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194512"
---
# <a name="add-microsoft-edge-to-microsoft-intune"></a><span data-ttu-id="e4355-102">Microsoft Edge pievienošana Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="e4355-102">Add Microsoft Edge to Microsoft Intune</span></span>

<span data-ttu-id="e4355-103">Lai varētu izvietot, konfigurēt, pārraudzīt un aizsargāt Microsoft Edge operētājsistēmā Windows 10, jums tā vispirms ir jāpievieno Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="e4355-103">To be able to deploy, configure, monitor, and protect Microsoft Edge for Windows 10, you must first add it to Microsoft Intune.</span></span>

> [!IMPORTANT]
- <span data-ttu-id="e4355-104">Intune atbalsta Microsoft Edge 77 un jaunākas versijas.</span><span class="sxs-lookup"><span data-stu-id="e4355-104">Intune supports Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="e4355-105">Intune noteiks visas iepriekš pastāvējušās Microsoft Edge instalācijas.</span><span class="sxs-lookup"><span data-stu-id="e4355-105">Intune will detect any pre-existing installations of Microsoft Edge.</span></span>
- <span data-ttu-id="e4355-106">Ja Microsoft Edge ir instalēta lietotāja kontekstā, sistēmas instalācija pārrakstīs instalāciju lietotāja kontekstā.</span><span class="sxs-lookup"><span data-stu-id="e4355-106">If Microsoft Edge is installed in user context, a system installation will overwrite the installation in user context.</span></span>
- <span data-ttu-id="e4355-107">Ja sistēmas konteksta datorā ir instalēta programma Microsoft Edge, tiks ziņots par instalēšanas panākumiem.</span><span class="sxs-lookup"><span data-stu-id="e4355-107">If Microsoft Edge is installed in system context, the installation success will be reported.</span></span>
- <span data-ttu-id="e4355-108">Iepriekš instalētas Microsoft Edge 77 un jaunākas versijas visiem kanāliem lietotāja kontekstā tiks pārrakstītas ar Microsoft Edge, kas instalēta sistēmas kontekstā.</span><span class="sxs-lookup"><span data-stu-id="e4355-108">Pre-installed Microsoft Edge 77 and later versions, for all channels in user context, will be overwritten with Microsoft Edge installed in system context.</span></span>

<span data-ttu-id="e4355-109">**Priekšnosacījuma**</span><span class="sxs-lookup"><span data-stu-id="e4355-109">**Prerequisite**</span></span>

<span data-ttu-id="e4355-110">Windows 10 versija 1709 vai jaunākas versijas</span><span class="sxs-lookup"><span data-stu-id="e4355-110">Windows 10 version 1709 or later versions</span></span>

<span data-ttu-id="e4355-111">**Darbības, kas jāveic, lai pievienotu Windows Intune malu**</span><span class="sxs-lookup"><span data-stu-id="e4355-111">**Steps to add Edge to Intune**</span></span>

1. <span data-ttu-id="e4355-112">[Konfigurējiet lietojumprogrammu Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="e4355-112">[Configure the app in Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
2. <span data-ttu-id="e4355-113">[Konfigurējiet lietojumprogrammu informāciju](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="e4355-113">[Configure the app information](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
3. <span data-ttu-id="e4355-114">[Konfigurējiet programmas iestatījumus](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="e4355-114">[Configure the app settings](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
4. <span data-ttu-id="e4355-115">[Atlasiet tvēruma atzīmes (neobligāti)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="e4355-115">[Select the scope tags (optional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
5. <span data-ttu-id="e4355-116">[Pievienojiet programmu](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="e4355-116">[Add the app](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>

<span data-ttu-id="e4355-117">Papildu palīdzību skatiet rakstā [problēmu novēršana](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="e4355-117">For more help, see [Troubleshooting](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>




