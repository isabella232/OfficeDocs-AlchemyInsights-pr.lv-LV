---
title: Izvietojot Office 365 ProPlus koplietojuma lietošanai RDS, termināļa serverī vai VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959466"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="2daf4-102">Izvietojot Office 365 ProPlus koplietojuma lietošanai RDS, termināļa serverī vai VDI</span><span class="sxs-lookup"><span data-stu-id="2daf4-102">Deploying Office 365 ProPlus for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="2daf4-103">Lai izvietotu Office 365 ProPlus, izmantojot attālās darbvirsmas pakalpojumu (RDS), iepriekš nosaukto termināļa pakalpojumi:</span><span class="sxs-lookup"><span data-stu-id="2daf4-103">To deploy Office 365 ProPlus using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
- <span data-ttu-id="2daf4-104">Jums ir jābūt Microsoft 365 biznesa plānu vai Office 365 plānu, kas ietver Office 365 ProPlus, piemēram, Office 365 Enterprise E3 vai Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="2daf4-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE] 
   > <span data-ttu-id="2daf4-105">Office 365 Business un Office 365 Business Premium plānos nav iekļauts Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="2daf4-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
- <span data-ttu-id="2daf4-106">Ir jāiespējo [koplietojamā datora aktivizācija](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="2daf4-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

> [!NOTE]
> <span data-ttu-id="2daf4-107">Varat arī lejupielādēt un palaist [Microsoft atbalsta un atkopšanas palīgu](https://aka.ms/SaRA_OfficeSCA_M365Portal) , lai instalētu Office 365 ProPlus koplietojamā datora aktivizācijas režīmā.</span><span class="sxs-lookup"><span data-stu-id="2daf4-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Office 365 ProPlus in shared computer activation mode.</span></span>

<span data-ttu-id="2daf4-108">Lai iegūtu papildinformāciju par priekšnosacījumiem, uzstādīšanas instrukcijas un norādījumus par pielāgotām instalācijām, izmantojot Office izvietošanas rīku, skatiet sadaļu [office 365 ProPlus izvietošana, izmantojot attālās darbvirsmas pakalpojumus](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="2daf4-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>

<span data-ttu-id="2daf4-109">Lai labotu kļūdas, kas saistītas ar koplietojamu datora aktivizāciju:</span><span class="sxs-lookup"><span data-stu-id="2daf4-109">To fix errors related to shared computer activation:</span></span>
- <span data-ttu-id="2daf4-110">Skatiet [problēmu novēršana saistībā ar Office 365 ProPlus koplietojamo datora aktivizāciju](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="2daf4-110">See [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
- <span data-ttu-id="2daf4-111">Skatiet sadaļu [Office 365 ProPlus aktivizācijas stāvokļa atiestatīšana](https://go.microsoft.com/fwlink/?linkid=2109218).</span><span class="sxs-lookup"><span data-stu-id="2daf4-111">See [Reset Office 365 ProPlus activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="2daf4-112">Ja vēlaties instalēt Office 365 ProPlus RDS no Microsoft 365 administrēšanas centrs, ***kas izmanto noklusējuma instalācijas iestatījumus***, rīkojieties šādi:</span><span class="sxs-lookup"><span data-stu-id="2daf4-112">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1.  <span data-ttu-id="2daf4-113">Pārbaudiet, kādi Office 365 plānu jums ir.</span><span class="sxs-lookup"><span data-stu-id="2daf4-113">Check what Office 365 plan you have.</span></span> <span data-ttu-id="2daf4-114">[Uzziniet, kā](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)to darīt.</span><span class="sxs-lookup"><span data-stu-id="2daf4-114">[Learn how](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2.  <span data-ttu-id="2daf4-115">Ja nepieciešams, pārslēdzieties uz citu Office 365 plānu.</span><span class="sxs-lookup"><span data-stu-id="2daf4-115">If necessary, switch to a different Office 365 plan.</span></span> <span data-ttu-id="2daf4-116">[Uzziniet, kā](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)to darīt.</span><span class="sxs-lookup"><span data-stu-id="2daf4-116">[Learn how](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span></span>
3.  <span data-ttu-id="2daf4-117">Ja Office jau ir instalēta RDS serverī, izmantojot citus Office 365 plānus, atinstalējiet to.</span><span class="sxs-lookup"><span data-stu-id="2daf4-117">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="2daf4-118">Piemēram, atverot **vadības paneli** > ,**atinstalējiet programmu**.</span><span class="sxs-lookup"><span data-stu-id="2daf4-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="2daf4-119">Atinstalējiet, izmantojot [Microsoft atbalsta un atkopšanas palīgu](https://aka.ms/SARA-OfficeUninstall-Alchemy) , ja rodas problēmas.</span><span class="sxs-lookup"><span data-stu-id="2daf4-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4.  <span data-ttu-id="2daf4-120">Serverī RDS pierakstieties Microsoft 365 administrēšanas centrā, izmantojot administratora kontu, un [instalējiet Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="2daf4-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5.  <span data-ttu-id="2daf4-121">Pēc Office instalēšanas ***neatveriet vai pierakstieties*** nevienā no Office lietojumprogrammām.</span><span class="sxs-lookup"><span data-stu-id="2daf4-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6.  <span data-ttu-id="2daf4-122">Serverī RDS iespējojiet koplietojamo datora aktivizāciju, rediģējot reģistru, veicot šādas darbības:</span><span class="sxs-lookup"><span data-stu-id="2daf4-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="2daf4-123">Ar peles labo pogu noklikšķiniet uz Windows pogas ekrāna apakšējā kreisajā stūrī un atlasiet **palaist**.</span><span class="sxs-lookup"><span data-stu-id="2daf4-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="2daf4-124">Lodziņā Atvērt ierakstiet **regedit**un pēc tam atlasiet **Labi**.</span><span class="sxs-lookup"><span data-stu-id="2daf4-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="2daf4-125">Atlasiet **Jā** , kad tiek piedāvāts atļaut reģistra redaktoram veikt izmaiņas ierīcē.</span><span class="sxs-lookup"><span data-stu-id="2daf4-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="2daf4-126">Reģistra redaktorā pievienojiet virknes vērtību **Sharedcomputerlicensing** ar iestatījumu 1 zem HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="2daf4-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="2daf4-127">RDS serverī, ***pierakstieties kā lietotājs*** un [Pārbaudiet, vai ir iespējots Office 365 ProPlus koplietojamo datora aktivizācija](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="2daf4-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

