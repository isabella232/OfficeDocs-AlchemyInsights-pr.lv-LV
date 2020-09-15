---
title: Office instalēšana termināļa serverī — nelicencēts
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663124"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="1b738-102">Office instalēšana termināļa serverī</span><span class="sxs-lookup"><span data-stu-id="1b738-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="1b738-103">Microsoft 365 lietojumprogrammu izvietošanai uzņēmumam Windows serverī, izmantojot attālās darbvirsmas pakalpojumus (RDS), kas iepriekš nosaukta par termināļa pakalpojumiem:</span><span class="sxs-lookup"><span data-stu-id="1b738-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="1b738-104">Jums ir jābūt Microsoft 365 abonementam, kurā ietilpst Microsoft 365 lietojumprogrammas uzņēmumam, piemēram, Office 365 Enterprise E3 vai Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="1b738-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="1b738-105">Microsoft 365 programmās darbam un Microsoft 365 programmas darbam Premium plāniem nav iekļautas Microsoft 365 lietojumprogrammas darbam ar Enterprise.</span><span class="sxs-lookup"><span data-stu-id="1b738-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="1b738-106">Ir jāiespējo [koplietojamā datora aktivizēšana](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="1b738-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="1b738-107">Ja vēlaties instalēt Microsoft 365 lietojumprogrammas uzņēmumam RDS no Microsoft 365 administrēšanas centra, ***kas izmanto noklusējuma instalācijas iestatījumus***, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="1b738-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="1b738-108">Varat arī lejupielādēt un palaist [Microsoft atbalsta un atkopšanas palīgu](https://aka.ms/SaRA_OfficeSCA_M365Portal) , lai instalētu Microsoft 365 lietojumprogrammas uzņēmumam koplietojamā datora aktivizēšanas režīmā.</span><span class="sxs-lookup"><span data-stu-id="1b738-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="1b738-109">Pārbaudiet, kāds ir Microsoft 365 abonements.</span><span class="sxs-lookup"><span data-stu-id="1b738-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="1b738-110">Uzziniet, kā</span><span class="sxs-lookup"><span data-stu-id="1b738-110">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="1b738-111">Ja nepieciešams, pārslēdzieties uz citu Microsoft 365 abonementu.</span><span class="sxs-lookup"><span data-stu-id="1b738-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="1b738-112">Uzziniet, kā</span><span class="sxs-lookup"><span data-stu-id="1b738-112">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. <span data-ttu-id="1b738-113">Ja sistēma Office jau ir instalēta RDS serverī, izmantojot jebkurus citus Microsoft 365 abonementus, atinstalējiet to.</span><span class="sxs-lookup"><span data-stu-id="1b738-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="1b738-114">Piemēram, atverot vadības paneļa \> Atinstalēt programmu.</span><span class="sxs-lookup"><span data-stu-id="1b738-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="1b738-115">Ja rodas problēmas, atinstalējiet [, izmantojot Microsoft atbalsta un atkopšanas palīgu](https://aka.ms/SARA-OfficeUninstall-Alchemy) .</span><span class="sxs-lookup"><span data-stu-id="1b738-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="1b738-116">RDS serverī pierakstieties Microsoft 365 administrēšanas centrā ar administratora kontu un [instalējiet microsoft 365 lietojumprogrammas uzņēmumam Enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="1b738-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="1b738-117">Pēc Office instalēšanas ***neatveriet vai pierakstieties*** jebkurā Office lietojumprogrammā.</span><span class="sxs-lookup"><span data-stu-id="1b738-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="1b738-118">RDS serverī iespējojiet koplietotu datora aktivizāciju, rediģējot reģistru, veicot tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="1b738-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="1b738-119">Ar peles labo pogu noklikšķiniet uz Windows pogas ekrāna kreisajā apakšējā stūrī un atlasiet palaist.</span><span class="sxs-lookup"><span data-stu-id="1b738-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="1b738-120">Lodziņā Atvērt ierakstiet **regedit**un pēc tam atlasiet Labi.</span><span class="sxs-lookup"><span data-stu-id="1b738-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="1b738-121">Atlasiet Jā, kad tiek parādīta uzvedne ar aicinājumu atļaut reģistra redaktoru veikt izmaiņas jūsu ierīcē.</span><span class="sxs-lookup"><span data-stu-id="1b738-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="1b738-122">Reģistra redaktorā pievienojiet **SharedComputerLicensing** virknes vērtību ar 1 HKEY_LOCAL_MACHINE \software\microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="1b738-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="1b738-123">RDS serverī ***pierakstieties kā lietotājs*** un [Pārbaudiet, vai koplietojamā datora aktivizācija ir iespējota Microsoft 365 lietojumprogrammām darbam ar Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="1b738-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="1b738-124">Lai iegūtu detalizētāku informāciju par priekšnosacījumiem, iestatīšanas norādījumiem un norādījumiem par pielāgotām instalācijām, izmantojot Office izvietošanas rīku, skatiet rakstu [Microsoft 365 lietojumprogrammu izvietošana uzņēmumam, izmantojot attālās darbvirsmas pakalpojumus](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="1b738-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="1b738-125">Lai labotu kļūdas, kas saistītas ar koplietojamu datora aktivizāciju, skatiet rakstu [problēmu novēršana saistībā ar koplietojamu datora aktivizāciju Microsoft 365 programmās darbam ar Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="1b738-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  