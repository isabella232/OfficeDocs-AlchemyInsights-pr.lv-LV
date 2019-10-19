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
ms.openlocfilehash: 51d1a66fdf9774bbe58bfdbe89317bc93834be09
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 10/18/2019
ms.locfileid: "37205416"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="ed67b-102">Office instalēšana termināļa serverī</span><span class="sxs-lookup"><span data-stu-id="ed67b-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="ed67b-103">Office 365 ProPlus izvietošanai Windows serverī, izmantojot attālās darbvirsmas pakalpojumus (RDS), iepriekš nosauktus termināļa pakalpojumus:</span><span class="sxs-lookup"><span data-stu-id="ed67b-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="ed67b-104">Jums ir jābūt Office 365 plānu, kas ietver Office 365 ProPlus, piemēram, Office 365 Enterprise E3 vai Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="ed67b-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="ed67b-105">Office 365 Business un Office 365 Business Premium plānos nav iekļauts Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="ed67b-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="ed67b-106">Ir jāiespējo [koplietojamā datora aktivizācija](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="ed67b-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="ed67b-107">Ja vēlaties instalēt Office 365 ProPlus RDS no Microsoft 365 administrēšanas centrs, ***kas izmanto noklusējuma instalācijas iestatījumus***, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="ed67b-107">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="ed67b-108">Varat arī lejupielādēt un palaist [Microsoft atbalsta un atkopšanas palīgu](https://aka.ms/SaRA_OfficeSCA_M365Portal) , lai instalētu Office 365 ProPlus koplietojamā datora aktivizācijas režīmā.</span><span class="sxs-lookup"><span data-stu-id="ed67b-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Office 365 ProPlus in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="ed67b-109">Pārbaudiet, kādi Office 365 plānu jums ir.</span><span class="sxs-lookup"><span data-stu-id="ed67b-109">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="ed67b-110">Uzziniet, kā</span><span class="sxs-lookup"><span data-stu-id="ed67b-110">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="ed67b-111">Ja nepieciešams, pārslēdzieties uz citu Office 365 plānu.</span><span class="sxs-lookup"><span data-stu-id="ed67b-111">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="ed67b-112">Uzziniet, kā</span><span class="sxs-lookup"><span data-stu-id="ed67b-112">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="ed67b-113">Ja Office jau ir instalēta RDS serverī, izmantojot citus Office 365 plānus, atinstalējiet to.</span><span class="sxs-lookup"><span data-stu-id="ed67b-113">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="ed67b-114">Piemēram, atverot vadības paneli \> , atinstalējiet programmu.</span><span class="sxs-lookup"><span data-stu-id="ed67b-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="ed67b-115">Atinstalējiet, izmantojot [Microsoft atbalsta un atkopšanas palīgu](https://aka.ms/SARA-OfficeUninstall-Alchemy) , ja rodas problēmas.</span><span class="sxs-lookup"><span data-stu-id="ed67b-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="ed67b-116">Serverī RDS pierakstieties Microsoft 365 administrēšanas centrā, izmantojot administratora kontu, un [instalējiet Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="ed67b-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="ed67b-117">Pēc Office instalēšanas ***neatveriet vai pierakstieties*** nevienā no Office lietojumprogrammām.</span><span class="sxs-lookup"><span data-stu-id="ed67b-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="ed67b-118">Serverī RDS iespējojiet koplietojamo datora aktivizāciju, rediģējot reģistru, veicot šādas darbības:</span><span class="sxs-lookup"><span data-stu-id="ed67b-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="ed67b-119">Ar peles labo pogu noklikšķiniet uz Windows pogas ekrāna kreisajā apakšējā stūrī un atlasiet palaist.</span><span class="sxs-lookup"><span data-stu-id="ed67b-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="ed67b-120">Lodziņā Atvērt ierakstiet **regedit**un pēc tam atlasiet Labi.</span><span class="sxs-lookup"><span data-stu-id="ed67b-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="ed67b-121">Atlasiet Jā, kad tiek piedāvāts atļaut reģistra redaktoram veikt izmaiņas ierīcē.</span><span class="sxs-lookup"><span data-stu-id="ed67b-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="ed67b-122">Reģistra redaktorā pievienojiet virknes vērtību **Sharedcomputerlicensing** ar iestatījumu 1 zem HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="ed67b-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="ed67b-123">RDS serverī, ***pierakstieties kā lietotājs*** un [Pārbaudiet, vai ir iespējots Office 365 ProPlus koplietojamo datora aktivizācija](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="ed67b-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="ed67b-124">Lai iegūtu papildinformāciju par priekšnosacījumi, uzstādīšanas instrukcijas un norādījumus par pielāgoto instalāciju, izmantojot Office izvietošanas rīks, lūdzu, skatiet [izvietot office 365 ProPlus, izmantojot attālās darbvirsmas pakalpojumu](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="ed67b-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="ed67b-125">Lai labotu kļūdas, kas saistītas ar koplietojamu datora aktivizāciju, lūdzu, skatiet [problēmu novēršana saistībā ar Office 365 ProPlus koplietojamo datora aktivizāciju](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="ed67b-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  