---
title: Office instalēšana termināļa serverī-nelicencēta
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 7252efdc0f55b8923e685ec89f9b3c63882aa6b0
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763224"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="bd3ca-102">Office instalēšana termināļa serverī</span><span class="sxs-lookup"><span data-stu-id="bd3ca-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="bd3ca-103">Lai izvietotu Microsoft 365 Apps Enterprise Windows Server, izmantojot attālās darbvirsmas pakalpojumu (RDS), iepriekš nosaukto termināļa pakalpojumi:</span><span class="sxs-lookup"><span data-stu-id="bd3ca-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="bd3ca-104">Jums ir jābūt Microsoft 365 abonements, kas ietver Microsoft 365 lietojumprogrammas uzņēmumiem, piemēram, Office 365 Enterprise E3 vai Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="bd3ca-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="bd3ca-105">Microsoft 365 lietojumprogrammas uzņēmumiem un Microsoft 365 lietojumprogrammām Business Premium plāniem neietver Microsoft 365 lietojumprogrammas uzņēmumiem.</span><span class="sxs-lookup"><span data-stu-id="bd3ca-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="bd3ca-106">Ir jāiespējo [koplietojamā datora aktivizācija](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="bd3ca-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="bd3ca-107">Ja vēlaties instalēt Microsoft 365 Apps Enterprise RDS no Microsoft 365 administrēšanas centrs, ***kas izmanto noklusējuma instalācijas iestatījumus***, rīkojieties šādi.</span><span class="sxs-lookup"><span data-stu-id="bd3ca-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="bd3ca-108">Varat arī lejupielādēt un palaist [Microsoft atbalsta un atkopšanas palīgu](https://aka.ms/SaRA_OfficeSCA_M365Portal) , lai instalētu Microsoft 365 lietojumprogrammas Enterprise koplietojamo datoru aktivizācijas režīmā.</span><span class="sxs-lookup"><span data-stu-id="bd3ca-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="bd3ca-109">Pārbaudiet, kāds ir Microsoft 365 abonements.</span><span class="sxs-lookup"><span data-stu-id="bd3ca-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="bd3ca-110">Uzziniet, kā</span><span class="sxs-lookup"><span data-stu-id="bd3ca-110">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="bd3ca-111">Ja nepieciešams, pārslēdzieties uz citu Microsoft 365 abonementu.</span><span class="sxs-lookup"><span data-stu-id="bd3ca-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="bd3ca-112">Uzziniet, kā</span><span class="sxs-lookup"><span data-stu-id="bd3ca-112">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="bd3ca-113">Ja Office jau ir instalēta RDS serverī, izmantojot citu Microsoft 365 abonementu, atinstalējiet to.</span><span class="sxs-lookup"><span data-stu-id="bd3ca-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="bd3ca-114">Piemēram, atverot vadības paneli \> , atinstalējiet programmu.</span><span class="sxs-lookup"><span data-stu-id="bd3ca-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="bd3ca-115">Atinstalējiet, izmantojot [Microsoft atbalsta un atkopšanas palīgu](https://aka.ms/SARA-OfficeUninstall-Alchemy) , ja rodas problēmas.</span><span class="sxs-lookup"><span data-stu-id="bd3ca-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="bd3ca-116">RDS serverī, pierakstieties Microsoft 365 administrēšanas centrs ar administratora kontu un [instalēt Microsoft 365 lietojumprogrammas uzņēmumiem](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="bd3ca-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="bd3ca-117">Pēc Office instalēšanas ***neatveriet vai pierakstieties*** nevienā no Office lietojumprogrammām.</span><span class="sxs-lookup"><span data-stu-id="bd3ca-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="bd3ca-118">Serverī RDS iespējojiet koplietojamo datora aktivizāciju, rediģējot reģistru, veicot šādas darbības:</span><span class="sxs-lookup"><span data-stu-id="bd3ca-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="bd3ca-119">Ar peles labo pogu noklikšķiniet uz Windows pogas ekrāna kreisajā apakšējā stūrī un atlasiet palaist.</span><span class="sxs-lookup"><span data-stu-id="bd3ca-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="bd3ca-120">Lodziņā Atvērt ierakstiet **regedit**un pēc tam atlasiet Labi.</span><span class="sxs-lookup"><span data-stu-id="bd3ca-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="bd3ca-121">Atlasiet Jā, kad tiek piedāvāts atļaut reģistra redaktoram veikt izmaiņas ierīcē.</span><span class="sxs-lookup"><span data-stu-id="bd3ca-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="bd3ca-122">Reģistra redaktorā pievienojiet virknes vērtību **Sharedcomputerlicensing** ar iestatījumu 1 zem HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="bd3ca-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="bd3ca-123">RDS serverī, ***pierakstieties kā lietotājs*** un [Pārbaudiet, vai ir iespējota Microsoft 365 lietojumprogrammas uzņēmumiem koplietojamā datora aktivizācija](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="bd3ca-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="bd3ca-124">Lai iegūtu papildinformāciju par priekšnosacījumi, uzstādīšanas instrukcijas un norādījumus par pielāgoto instalāciju, izmantojot Office izvietošanas rīks, lūdzu, skatiet [izvietot Microsoft 365 lietojumprogrammas uzņēmumiem, izmantojot attālās darbvirsmas pakalpojumu](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="bd3ca-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="bd3ca-125">Lai labotu kļūdas, kas saistītas ar koplietojamu datora aktivizāciju, lūdzu, skatiet [problēmu novēršana saistībā ar koplietojamo datora aktivizēšanu Microsoft 365 lietojumprogrammām uzņēmumam](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="bd3ca-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  