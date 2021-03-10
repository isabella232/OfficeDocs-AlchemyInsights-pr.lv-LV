---
title: MDATP instalēšanas problēmu novēršana Mac datorā
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694281"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a><span data-ttu-id="0f6c0-102">MDATP instalēšanas problēmu novēršana Mac datorā</span><span class="sxs-lookup"><span data-stu-id="0f6c0-102">Troubleshoot MDATP installation problems on a Mac</span></span>

<span data-ttu-id="0f6c0-103">Ja manuāla instalēšana neizdevās, instalēšanas vedņa **kopsavilkuma** lapā tiek rādīta šāda kļūda:</span><span class="sxs-lookup"><span data-stu-id="0f6c0-103">If manual installation fails, the **Summary** page of the installation wizard shows the following error:</span></span>

<span data-ttu-id="0f6c0-104">"Instalēšanas laikā radās kļūda.</span><span class="sxs-lookup"><span data-stu-id="0f6c0-104">"An error occurred during installation.</span></span> <span data-ttu-id="0f6c0-105">Instalēšanas programma atklāja kļūdu, kuras dēļ instalēšana neizdevās.</span><span class="sxs-lookup"><span data-stu-id="0f6c0-105">The Installer encountered an error that caused the installation to fail.</span></span> <span data-ttu-id="0f6c0-106">Lai saņemtu palīdzību, sazinieties ar programmatūras ražotāju.</span><span class="sxs-lookup"><span data-stu-id="0f6c0-106">Contact the software manufacturer for assistance."</span></span>

<span data-ttu-id="0f6c0-107">MDM izvietojumiem lapā tiek rādīta arī vispārīga instalēšanas kļūme.</span><span class="sxs-lookup"><span data-stu-id="0f6c0-107">For MDM deployments, the page shows a generic installation failure, too.</span></span>

<span data-ttu-id="0f6c0-108">Lai gan nerāda precīzas kļūdas lietotājiem, mēs pabeidzam reģistrēt failu ar instalēšanas norisi programmā **/Library/logs/Microsoft/mdatp/Install.log**.</span><span class="sxs-lookup"><span data-stu-id="0f6c0-108">Although we don't display exact errors to end users, we keep a log file with installation progress, in **/Library/Logs/Microsoft/mdatp/install.log**.</span></span> <span data-ttu-id="0f6c0-109">Katra instalācijas sesija pievieno šo žurnālfailu.</span><span class="sxs-lookup"><span data-stu-id="0f6c0-109">Each installation session appends to this log file.</span></span> <span data-ttu-id="0f6c0-110">Lai izvadītu tikai pēdējo instalēšanas sesiju, izmantojiet `sed` .</span><span class="sxs-lookup"><span data-stu-id="0f6c0-110">To output the last installation session only, use `sed`.</span></span>

<span data-ttu-id="0f6c0-111">Lai uzzinātu vairāk, skatiet rakstu [problēmu novēršana saistībā ar Microsoft Defender ATP darbam ar Mac instalēšanas problēmām](https://go.microsoft.com/fwlink/?linkid=2144615).</span><span class="sxs-lookup"><span data-stu-id="0f6c0-111">To learn more, see [Troubleshoot installation issues for Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span></span>
