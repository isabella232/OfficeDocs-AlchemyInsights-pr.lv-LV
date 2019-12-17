---
title: 0x8004de40 kļūdas labošana pakalpojumā OneDrive
ms.author: pebaum
author: pebaum
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 48b29f57763ca22a71a23b2afddcac0e8e8a95db
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052044"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="e9620-102">0x8004de40 kļūdas labošana pakalpojumā OneDrive</span><span class="sxs-lookup"><span data-stu-id="e9620-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="e9620-103">Ja pakalpojumā OneDrive tiek parādīta kļūda 0x8004de40:</span><span class="sxs-lookup"><span data-stu-id="e9620-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="e9620-104">Atsāknējiet attiecīgajā datorā, kamēr izveidots savienojums ar Acitve direktorija domēns.</span><span class="sxs-lookup"><span data-stu-id="e9620-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="e9620-105">Ja atsāknēšana neatrisina problēmu, atpievienojieties un atkārtoti Pievienojieties ierīcei no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e9620-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="e9620-106">**Piezīme**: jums vajadzētu būt uzņēmuma tīklā, veicot šīs darbības.</span><span class="sxs-lookup"><span data-stu-id="e9620-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="e9620-107">Neveiciet šīs darbības, ja nevarat izveidot savienojumu ar uzņēmuma infrastruktūru (piemēram, ceļojot).</span><span class="sxs-lookup"><span data-stu-id="e9620-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="e9620-108">Atveriet privileģēto komandu uzvedni.</span><span class="sxs-lookup"><span data-stu-id="e9620-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="e9620-109">Lai atvērtu privileģēto komandu uzvedni, noklikšķiniet uz **Sākt**, ar peles labo pogu noklikšķiniet uz **komandu uzvedne**un pēc tam noklikšķiniet uz **Palaist kā administratoram**.</span><span class="sxs-lookup"><span data-stu-id="e9620-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="e9620-110">Ierakstiet *dsregcmd/Leave* un nospiediet taustiņu **Enter**.</span><span class="sxs-lookup"><span data-stu-id="e9620-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="e9620-111">Kad pabeigta, ierakstiet *dsregcmd/Join* un nospiediet taustiņu **Enter**.</span><span class="sxs-lookup"><span data-stu-id="e9620-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="e9620-112">Kad tas ir pabeigts, aizveriet komandu uzvedni.</span><span class="sxs-lookup"><span data-stu-id="e9620-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="e9620-113">Atsāknējiet datoru un piesakieties pakalpojumā OneDrive.</span><span class="sxs-lookup"><span data-stu-id="e9620-113">Reboot the computer, and log into OneDrive.</span></span>