---
title: Noteikt 0x8004de40 error OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: d436184bdc0e283db217ea734fb2c8e05f85b4e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525066"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="bcdbf-102">Noteikt 0x8004de40 error OneDrive</span><span class="sxs-lookup"><span data-stu-id="bcdbf-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="bcdbf-103">Ja saņemat kļūdas 0x8004de40 ar OneDrive:</span><span class="sxs-lookup"><span data-stu-id="bcdbf-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="bcdbf-104">Atsāknēšana ietekmē datoru, savienojuma aktivs Directory domēns.</span><span class="sxs-lookup"><span data-stu-id="bcdbf-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="bcdbf-105">Ja reboot neatrisina problēmu, atvienoties un atkal pievienoties jūsu ierīci no debeszils reklāmu.</span><span class="sxs-lookup"><span data-stu-id="bcdbf-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="bcdbf-106">**Piezīme**: jums vajadzētu būt uzņēmuma tīklā, veicot šādas darbības.</span><span class="sxs-lookup"><span data-stu-id="bcdbf-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="bcdbf-107">Neveic šos pasākumus, ja jūs nespējat pieslēgties jūsu uzņēmuma infrastruktūra (piemēram, ceļojot).</span><span class="sxs-lookup"><span data-stu-id="bcdbf-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="bcdbf-108">Open paaugstināts komandu uzvednes.</span><span class="sxs-lookup"><span data-stu-id="bcdbf-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="bcdbf-109">Open paaugstināts komandu uzvednes, noklikšķiniet - **Sākt**, ar peles labo pogu noklikšķiniet uz **komandu uzvedne**un pēc tam noklikšķiniet uz **Palaist kā administratoram**.</span><span class="sxs-lookup"><span data-stu-id="bcdbf-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="bcdbf-110">*Dsregcmd /leave* tipu, un nospiediet taustiņu **Enter**.</span><span class="sxs-lookup"><span data-stu-id="bcdbf-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="bcdbf-111">Kad pabeigts, ierakstiet *dsregcmd /join* un nospiediet taustiņu **Enter**.</span><span class="sxs-lookup"><span data-stu-id="bcdbf-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="bcdbf-112">Kad pabeigta, aizveriet komandu uzvednes.</span><span class="sxs-lookup"><span data-stu-id="bcdbf-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="bcdbf-113">Atsāknējiet datoru un piesakieties savā OneDrive.</span><span class="sxs-lookup"><span data-stu-id="bcdbf-113">Reboot the computer, and log into OneDrive.</span></span>