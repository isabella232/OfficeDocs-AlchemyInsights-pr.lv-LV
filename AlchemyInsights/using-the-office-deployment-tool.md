---
title: Izmantojot Office izvietošanas rīku
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: d941bce524dc797d5dcbb7213bded6919fd01b7d
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010874"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="74885-102">Izmantojot Office izvietošanas rīku (ODT)</span><span class="sxs-lookup"><span data-stu-id="74885-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="74885-103">Office izvietošanas rīks (ODT) izmanto, lai izvietotu Office 365 Office versijas.</span><span class="sxs-lookup"><span data-stu-id="74885-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="74885-104">Office izvietošanas rīks (setup. exe) tiek palaists no komandrindas un izmanto konfigurācijas XML failu, lai noteiktu, kādi iestatījumi jālieto, izvietojot Office.</span><span class="sxs-lookup"><span data-stu-id="74885-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="74885-105">Lejupielādējiet Office izvietošanas rīka jaunāko versiju no [Microsoft lejupielādes centra](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="74885-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="74885-106">Izmantojiet [Office pielāgošanas rīku (Oct)](https://config.office.com) , lai atlasītu izvietošanas preferences un izveidotu konfigurācijas XML failu.</span><span class="sxs-lookup"><span data-stu-id="74885-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="74885-107">Eksportējiet konfigurācijas failu un novietojiet to lokāli tajā pašā mapē, kur atrodas setup. exe.</span><span class="sxs-lookup"><span data-stu-id="74885-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="74885-108">**Piezīme:** Office instalācijas problēmas parasti rodas nepareizas konfigurēšanas vai nepareizi formatētu konfigurācijas failu dēļ.</span><span class="sxs-lookup"><span data-stu-id="74885-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="74885-109">Lai izvairītos no šādām problēmām, ieteicams izmantot Office pielāgošanas rīku, lai izveidotu konfigurācijas failu.</span><span class="sxs-lookup"><span data-stu-id="74885-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="74885-110">Varat arī importēt esošos konfigurācijas failus Office pielāgošanas rīkā.</span><span class="sxs-lookup"><span data-stu-id="74885-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="74885-111">Priviliģētā komandu uzvednē pārslēdzieties uz vietu, kur atrodas setup. exe, un palaidiet rīku Office Deployment lejupielādes režīmā un norādiet tikko saglabāto konfigurācijas failu.</span><span class="sxs-lookup"><span data-stu-id="74885-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="74885-112">Šajā piemērā konfigurācijas faila nosaukums ir Configuration. XML:</span><span class="sxs-lookup"><span data-stu-id="74885-112">In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="74885-113">Palaidiet rīku Office izvietošanas konfigurēšana režīmā un norādiet konfigurācijas failu.</span><span class="sxs-lookup"><span data-stu-id="74885-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="74885-114">**Piezīme:** Šī darbība ir jāpalaiž klienta datorā, kurā vēlaties instalēt Office, un jums ir jābūt lokālā administratora atļaujām šajā datorā.</span><span class="sxs-lookup"><span data-stu-id="74885-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="74885-115">Lai uzzinātu vairāk par Office izvietošanas rīka lietošanu Microsoft 365 lietojumprogrammām uzņēmuma izvietošanas scenārijiem, skatiet [pārskats par Office izvietošanas rīku](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="74885-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span></span> <span data-ttu-id="74885-116">Plašāku informāciju par to, kā izmantot Office pielāgošanas rīku, skatiet sadaļā [pārskats par Office pielāgošanas rīku](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="74885-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
