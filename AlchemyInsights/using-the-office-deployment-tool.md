---
title: Izmantojot rīku Office izvietošanai
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 874bb7883bca4f062e85963a6828a771cd2dad9b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/22/2019
ms.locfileid: "36531582"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="080bb-102">Izmantojot Office izvietošanas rīku (ODT)</span><span class="sxs-lookup"><span data-stu-id="080bb-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="080bb-103">Izmantojat Office izvietošanas rīku (ODT) izvietot Office 365 Office versijām.</span><span class="sxs-lookup"><span data-stu-id="080bb-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="080bb-104">Office ieviešanas rīks (setup.exe) tiek palaista no komandrindas un konfigurācijas XML failu izmanto, lai noteiktu, kādus iestatījumus lietot, izvietojot Office.</span><span class="sxs-lookup"><span data-stu-id="080bb-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="080bb-105">Lejupielādēt jaunāko versiju Office izvietošanas rīku no [Microsoft lejupielādes centra](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="080bb-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="080bb-106">Izmantojiet [Office pielāgošanas rīks (AZT)](https://config.office.com) atlasiet izvietošanas preferences un izveidot konfigurācijas XML failu.</span><span class="sxs-lookup"><span data-stu-id="080bb-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="080bb-107">Konfigurācijas faila eksportēšanas un lokāli novietot tajā pašā mapē, kur atrodas setup.exe.</span><span class="sxs-lookup"><span data-stu-id="080bb-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="080bb-108">**Piezīme:** Office instalācijas, bieži rodas problēmas sakarā ar misconfigured vai malformatted konfigurācijas failus.</span><span class="sxs-lookup"><span data-stu-id="080bb-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="080bb-109">Lai izvairītos no šādas problēmas, ieteicams izmantot Office pielāgošanas rīku, lai izveidotu konfigurācijas failu.</span><span class="sxs-lookup"><span data-stu-id="080bb-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="080bb-110">Esošās konfigurācijas failus var arī importēt Office pielāgošanas rīks.</span><span class="sxs-lookup"><span data-stu-id="080bb-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="080bb-111">Paaugstinātu komandu uzvednes, pāriet uz vietu, kur dzīvo setup.exe un palaist Office izvietošanas rīku lejupielādes režīmā un norādiet konfigurācijas failu, kuru tikko saglabājāt.</span><span class="sxs-lookup"><span data-stu-id="080bb-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="080bb-112">Šajā piemērā konfigurācijas fails tiek nosaukts Configuration:</span><span class="sxs-lookup"><span data-stu-id="080bb-112">In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="080bb-113">Palaidiet Office izvietošanas rīku konfigurēt režīmu un norādiet konfigurācijas failu.</span><span class="sxs-lookup"><span data-stu-id="080bb-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="080bb-114">**Piezīme:** Jāpalaiž šis solis no klienta datorā, kurā vēlaties instalēt Office un jums jābūt lokālā administratora atļaujām šajā datorā.</span><span class="sxs-lookup"><span data-stu-id="080bb-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="080bb-115">Lai uzzinātu vairāk par Office izvietošanas rīku izmantošana Office 365 ProPlus izvietošanas scenārijos, skatiet [Office izvietošanas rīku apskats](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="080bb-115">To learn more about using Office Deployment Tool for your Office 365 ProPlus deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span></span> <span data-ttu-id="080bb-116">Sīkāku informāciju par to, kā izmantot Office pielāgošanas rīku, skatiet [Office pielāgošanas rīku apskats](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="080bb-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
