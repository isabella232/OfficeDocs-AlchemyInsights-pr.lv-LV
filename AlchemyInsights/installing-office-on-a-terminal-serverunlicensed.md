---
title: Office instalēšanas termināla serverī - nelicencētu
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 971edd9c064b448446ba16361e99df4a2291c14f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/23/2019
ms.locfileid: "32410129"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="e8bfe-102">Instalējot Office termināļu serverī</span><span class="sxs-lookup"><span data-stu-id="e8bfe-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="e8bfe-103">Par to, kā izvietot Office 365 ProPlus Windows serverī, izmantojot attālās darbvirsmas pakalpojumu (RDS), iepriekš dēvēts par termināļa pakalpojumi:</span><span class="sxs-lookup"><span data-stu-id="e8bfe-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="e8bfe-104">Datorā jābūt instalētai Office 365 plānu, kas ietver Office 365 ProPlus, piemēram, Office 365 Enterprise E3 vai uzņēmuma E5.</span><span class="sxs-lookup"><span data-stu-id="e8bfe-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="e8bfe-105">Office 365 Business un Office 365 Business Premium plāni nav iekļauti Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="e8bfe-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
    
- <span data-ttu-id="e8bfe-106">Ir jāiespējo [koplietojamās datora aktivizāciju](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="e8bfe-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>
    
<span data-ttu-id="e8bfe-107">Ja vēlaties instalēt Office 365 ProPlus RDS no portāla Office 365 \* \* *kas izmanto instalācijas noklusējuma iestatījumus* \* \*, rīkojieties šādi:</span><span class="sxs-lookup"><span data-stu-id="e8bfe-107">If you want to install Office 365 ProPlus on RDS from the Office 365 portal, \*\* *which uses default installation settings* \*\*, follow these steps:</span></span> 
  
1. <span data-ttu-id="e8bfe-108">Pārbaudiet, kāda Office 365 plānu, kas jums ir.</span><span class="sxs-lookup"><span data-stu-id="e8bfe-108">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="e8bfe-109">Uzziniet, kā</span><span class="sxs-lookup"><span data-stu-id="e8bfe-109">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)
    
2. <span data-ttu-id="e8bfe-110">Ja nepieciešams, pārslēdzieties uz citu Office 365 plānu.</span><span class="sxs-lookup"><span data-stu-id="e8bfe-110">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="e8bfe-111">Uzziniet, kā</span><span class="sxs-lookup"><span data-stu-id="e8bfe-111">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)
    
3. <span data-ttu-id="e8bfe-112">Ja RDS servera, izmantojot citas Office 365 plāni jau ir instalēta Office, noņemt tās instalāciju.</span><span class="sxs-lookup"><span data-stu-id="e8bfe-112">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="e8bfe-113">Piemēram, dodoties uz Control Panel \> atinstalēt programmu.</span><span class="sxs-lookup"><span data-stu-id="e8bfe-113">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="e8bfe-114">Atinstalējiet to, izmantojot [Microsoft atbalsts un palīgs atgūšanas](https://aka.ms/SARA-OfficeUninstall-Alchemy) , ja jūs strādājat par jautājumiem.</span><span class="sxs-lookup"><span data-stu-id="e8bfe-114">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span> 
    
4. <span data-ttu-id="e8bfe-115">RDS serverī, pierakstieties pakalpojumā Office 365 portāls ar administratora kontu un [instalēt Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="e8bfe-115">On the RDS server, sign in to the Office 365 portal with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
    
5. <span data-ttu-id="e8bfe-116">Pēc tam, kad ir instalēta Office \* \* *nav atvērts vai pierakstieties* \* \* lai visas Office lietojumprogrammas.</span><span class="sxs-lookup"><span data-stu-id="e8bfe-116">After Office is installed, \*\* *don't open or sign in* \*\* to any Office applications.</span></span> 
    
6. <span data-ttu-id="e8bfe-117">Serverī RDS iespējotu koplietojamās datora aktivizāciju, rediģējot reģistru, veicot šādas darbības:</span><span class="sxs-lookup"><span data-stu-id="e8bfe-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
    
1. <span data-ttu-id="e8bfe-118">Ar peles labo pogu noklikšķiniet uz Windows pogas ekrāna kreisajā apakšējā stūrī un izvēlieties Run.</span><span class="sxs-lookup"><span data-stu-id="e8bfe-118">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="e8bfe-119">Lodziņā Atvērt ierakstiet **regedit**un pēc tam izvēlieties Labi.</span><span class="sxs-lookup"><span data-stu-id="e8bfe-119">In the Open box, type **regedit**, and then select OK.</span></span> 
    
2. <span data-ttu-id="e8bfe-120">Izvēlieties Jā, ja tiek prasīts atļaut Registry Editor veikt izmaiņas jūsu ierīcē.</span><span class="sxs-lookup"><span data-stu-id="e8bfe-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>
    
3. <span data-ttu-id="e8bfe-121">Reģistra redaktoru, pievienot virknes vērtība ir **SharedComputerLicensing** , kurā 1 zem HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="e8bfe-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span> 
    
7. <span data-ttu-id="e8bfe-122">Serverī RDS \* \* *, pierakstieties kā lietotājs* \* \* un [pārbaudīt, ka koplietojama datora aktivizēšana ir iespējota Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="e8bfe-122">On the RDS server, \*\* *sign in as an end user* \*\* and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>
    
<span data-ttu-id="e8bfe-123">Sīkāku informāciju par priekšnoteikumiem, uzstādīšanas instrukcijas un norādījumi par pielāgoto instalāciju, izmantojot rīku Office izvietošanu, lūdzu skatīt [Izvietot Office 365 ProPlus, izmantojot attālās darbvirsmas pakalpojumu](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="e8bfe-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="e8bfe-124">Lai novērstu kļūdas, kas attiecas uz koplietojamās datora aktivizāciju, lūdzu, skatiet [novērst problēmas, kas saistītas ar koplietojama datora aktivizāciju Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="e8bfe-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  

