---
title: Office izvietošanas rīka izmantošana
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: f3a5dbfc6b64ccd4f0b19a5f86236336e78838d4
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085839"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="80a65-102">Izmantojot Office izvietošanas rīku (ODT)</span><span class="sxs-lookup"><span data-stu-id="80a65-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="80a65-103">Izmantojiet Office izvietošanas rīku (ODT), lai izvietotu Office 365 Office versijas.</span><span class="sxs-lookup"><span data-stu-id="80a65-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="80a65-104">Office izvietošanas rīku (setupodt.exe) izpilda no komandrindas un izmanto konfigurācijas XML failu, lai noteiktu, kādi iestatījumi jālieto, izvietojot Office.</span><span class="sxs-lookup"><span data-stu-id="80a65-104">The Office Deployment Tool (setupodt.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="80a65-105">Lejupielādējiet jaunāko Office izvietošanas rīka versiju no [Microsoft lejupielādes centra](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="80a65-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="80a65-106">Izmantojiet [Office pielāgošanas rīku (Oct)](https://config.office.com) , lai atlasītu izvietošanas preferences un izveidotu konfigurācijas XML failu.</span><span class="sxs-lookup"><span data-stu-id="80a65-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="80a65-107">Eksportējiet konfigurācijas failu un novietojiet to lokāli tajā pašā mapē, kur atrodas setupodt.exe.</span><span class="sxs-lookup"><span data-stu-id="80a65-107">Export the configuration file and place it locally on the same folder where the setupodt.exe resides.</span></span>

    <span data-ttu-id="80a65-108">**Piezīme:** Office instalēšanas problēmas parasti rodas nepareizi konfigurētu vai malformatted konfigurācijas failu dēļ.</span><span class="sxs-lookup"><span data-stu-id="80a65-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="80a65-109">Lai izvairītos no šādām problēmām, iesakām izmantot Office pielāgošanas rīku, lai izveidotu konfigurācijas failu.</span><span class="sxs-lookup"><span data-stu-id="80a65-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="80a65-110">Varat arī importēt esošos konfigurācijas failus Office pielāgošanas rīkā.</span><span class="sxs-lookup"><span data-stu-id="80a65-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="80a65-111">Priviliģētā komandu uzvednē pārejiet uz atrašanās vietu, kur setupodt.exe atrodas, un palaidiet Office izvietošanas rīku lejupielādes režīmā un norādiet konfigurācijas failu, kuru tikko saglabājāt.</span><span class="sxs-lookup"><span data-stu-id="80a65-111">From an elevated command prompt, switch to the location where setupodt.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="80a65-112">Šajā piemērā konfigurācijas faila nosaukums ir Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="80a65-112">In this example, the configuration file is named Configuration.xml:</span></span>

```setupodt.exe /download Configuration.xml```

<span data-ttu-id="80a65-113">4. palaidiet Office izvietošanas rīku konfigurēšanas režīmā un norādiet konfigurācijas failu.</span><span class="sxs-lookup"><span data-stu-id="80a65-113">4.Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>

```setupodt.exe /configure Configuration.xml```

<span data-ttu-id="80a65-114">**Piezīme:** Šī darbība ir jāveic no klienta datora, kurā vēlaties instalēt Office, un jums ir nepieciešamas lokālā administratora atļaujas šajā datorā.</span><span class="sxs-lookup"><span data-stu-id="80a65-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="80a65-115">Lai uzzinātu vairāk par to, kā izmantot Office izvietošanas rīku Microsoft 365 lietojumprogrammām uzņēmuma izvietošanas scenārijiem, skatiet rakstu [pārskats par Office izvietošanas rīku](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="80a65-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span></span> <span data-ttu-id="80a65-116">Lai iegūtu papildinformāciju par to, kā izmantot Office pielāgošanas rīku, skatiet rakstu [pārskats par Office pielāgošanas rīku](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="80a65-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
