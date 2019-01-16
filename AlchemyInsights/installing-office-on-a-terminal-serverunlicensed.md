---
title: Office instalēšanas termināla serverī - nelicencētu
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 73d5128b55cae7712c48be9e2d05e558c3ba2e5c
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/15/2019
ms.locfileid: "28300567"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="5858b-102">Instalējot Office termināļu serverī</span><span class="sxs-lookup"><span data-stu-id="5858b-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="5858b-103">Par to, kā izvietot Office 365 ProPlus Windows serverī, izmantojot attālās darbvirsmas pakalpojumu (RDS), iepriekš dēvēts par termināļa pakalpojumi:</span><span class="sxs-lookup"><span data-stu-id="5858b-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="5858b-p101">Datorā jābūt instalētai Office 365 plānu, kas ietver Office 365 ProPlus, piemēram, Office 365 Enterprise E3 vai uzņēmuma E5. Office 365 Business un Office 365 Business Premium plāni nav iekļauti Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="5858b-p101">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5. The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
    
- <span data-ttu-id="5858b-106">Ir jāiespējo [koplietojamās datora aktivizāciju](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="5858b-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>
    
<span data-ttu-id="5858b-107">Ja vēlaties instalēt Office 365 ProPlus RDS no portāla Office 365 \* \* *kas izmanto instalācijas noklusējuma iestatījumus* \* \*, rīkojieties šādi:</span><span class="sxs-lookup"><span data-stu-id="5858b-107">If you want to install Office 365 ProPlus on RDS from the Office 365 portal, \*\* *which uses default installation settings* \*\*, follow these steps:</span></span> 
  
1. <span data-ttu-id="5858b-p102">Pārbaudiet, kāda Office 365 plānu, kas jums ir. [Uzzināt cik](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)</span><span class="sxs-lookup"><span data-stu-id="5858b-p102">Check what Office 365 plan you have. [Learn how](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)</span></span>
    
2. <span data-ttu-id="5858b-p103">Ja nepieciešams, pārslēdzieties uz citu Office 365 plānu. [Uzzināt cik](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)</span><span class="sxs-lookup"><span data-stu-id="5858b-p103">If necessary, switch to a different Office 365 plan. [Learn how](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)</span></span>
    
3. <span data-ttu-id="5858b-p104">Ja RDS servera, izmantojot citas Office 365 plāni jau ir instalēta Office, noņemt tās instalāciju. Piemēram, dodoties uz Control Panel \> atinstalēt programmu. Atinstalējiet to, izmantojot [Microsoft atbalsts un palīgs atgūšanas](https://aka.ms/SARA-OfficeUninstall-Alchemy) , ja jūs strādājat par jautājumiem.</span><span class="sxs-lookup"><span data-stu-id="5858b-p104">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it. For example, by going to Control Panel \> Uninstall a program. Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span> 
    
4. <span data-ttu-id="5858b-115">RDS serverī, pierakstieties pakalpojumā Office 365 portāls ar administratora kontu un [instalēt Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="5858b-115">On the RDS server, sign in to the Office 365 portal with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
    
5. <span data-ttu-id="5858b-116">Pēc tam, kad ir instalēta Office \* \* *nav atvērts vai pierakstieties* \* \* lai visas Office lietojumprogrammas.</span><span class="sxs-lookup"><span data-stu-id="5858b-116">After Office is installed, \*\* *don't open or sign in* \*\* to any Office applications.</span></span> 
    
6. <span data-ttu-id="5858b-117">Serverī RDS iespējotu koplietojamās datora aktivizāciju, rediģējot reģistru, veicot šādas darbības:</span><span class="sxs-lookup"><span data-stu-id="5858b-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
    
1. <span data-ttu-id="5858b-p105">Ar peles labo pogu noklikšķiniet uz Windows pogas ekrāna kreisajā apakšējā stūrī un izvēlieties Run. Lodziņā Atvērt ierakstiet **regedit**un pēc tam izvēlieties Labi.</span><span class="sxs-lookup"><span data-stu-id="5858b-p105">Right-click the Windows button in the lower left-hand corner of your screen and select Run. In the Open box, type **regedit**, and then select OK.</span></span> 
    
2. <span data-ttu-id="5858b-120">Izvēlieties Jā, ja tiek prasīts atļaut Registry Editor veikt izmaiņas jūsu ierīcē.</span><span class="sxs-lookup"><span data-stu-id="5858b-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>
    
3. <span data-ttu-id="5858b-121">Reģistra redaktoru, pievienot virknes vērtība ir **SharedComputerLicensing** , kurā 1 zem HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="5858b-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span> 
    
7. <span data-ttu-id="5858b-122">Serverī RDS \* \* *, pierakstieties kā lietotājs* \* \* un [pārbaudīt, ka koplietojama datora aktivizēšana ir iespējota Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="5858b-122">On the RDS server, \*\* *sign in as an end user* \*\* and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>
    
<span data-ttu-id="5858b-123">Sīkāku informāciju par priekšnoteikumiem, uzstādīšanas instrukcijas un norādījumi par pielāgoto instalāciju, izmantojot rīku Office izvietošanu, lūdzu skatīt [Izvietot Office 365 ProPlus, izmantojot attālās darbvirsmas pakalpojumu](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="5858b-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="5858b-124">Lai novērstu kļūdas, kas attiecas uz koplietojamās datora aktivizāciju, lūdzu, skatiet [novērst problēmas, kas saistītas ar koplietojama datora aktivizāciju Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="5858b-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  

