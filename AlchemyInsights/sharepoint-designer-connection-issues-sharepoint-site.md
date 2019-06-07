---
title: SharePoint Online atļauju līmeņus
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760699"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="27f9e-102">SharePoint Designer savienojuma problēmas</span><span class="sxs-lookup"><span data-stu-id="27f9e-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="27f9e-103">Ja SharePoint Designer radušās savienojuma problēmas SharePoint vietnēm, lūdzu, mēģiniet šādus kopīgus risinājumus.</span><span class="sxs-lookup"><span data-stu-id="27f9e-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please attempt the following common solutions.</span></span>

<span data-ttu-id="27f9e-104">1. darbība: Pārliecinieties, vai SharePoint Designer tiek atjaunināts.</span><span class="sxs-lookup"><span data-stu-id="27f9e-104">Step 1: Verify SharePoint Designer is updated.</span></span>

- [<span data-ttu-id="27f9e-105">SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="27f9e-105">SharePoint Designer 2013</span></span>](https://www.microsoft.com/download/details.aspx?id=35491)

- [<span data-ttu-id="27f9e-106">SharePoint Designer 1. servisa pakotne (SP1)</span><span class="sxs-lookup"><span data-stu-id="27f9e-106">SharePoint Designer Service Pack 1 (SP1)</span></span>](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [<span data-ttu-id="27f9e-107">Atjauninājums programmai SharePoint Designer 2013 (KB3114721)</span><span class="sxs-lookup"><span data-stu-id="27f9e-107">Update for SharePoint Designer 2013 (KB3114721)</span></span>](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

<span data-ttu-id="27f9e-108">2. solis: Notīrīt lokālajā kešatmiņā failus</span><span class="sxs-lookup"><span data-stu-id="27f9e-108">Step 2: Clear the local cache files</span></span>

- <span data-ttu-id="27f9e-109">Tuvu SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="27f9e-109">Close SharePoint Designer 2013.</span></span>

- <span data-ttu-id="27f9e-110">Lokālajā datorā, dodieties uz šīm mapēm, lai dzēstu kešatmiņā failus.</span><span class="sxs-lookup"><span data-stu-id="27f9e-110">On the local computer, browse to the following folders to remove cached files.</span></span>

- <span data-ttu-id="27f9e-111">Noklikšķiniet uz Sākt, palaist, kā _ arī izdzēst visus failus atrast katrā no vietām zemāk.</span><span class="sxs-lookup"><span data-stu-id="27f9e-111">Click Start, Run and delete all files found under each of the below locations.</span></span>

<span data-ttu-id="27f9e-112">%AppData%\Microsoft\Web servera Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="27f9e-112">%APPDATA%\Microsoft\Web Server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

<span data-ttu-id="27f9e-113">Atveriet SharePoint Designer 2013 un ievadiet kontu vēlreiz, lai redzētu, vai tas darbojas.</span><span class="sxs-lookup"><span data-stu-id="27f9e-113">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="27f9e-114">3. solis: [Iespējot mūsdienu biroja 2013 ierīcēs, izmantojot Windows autentifikāciju](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="27f9e-114">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span></span>

<span data-ttu-id="27f9e-115">4. solis: Administratoriem būs nepieciešams pielāgots skripts ļauj atļaut savienojumu SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="27f9e-115">Step 4: Administrators will need to Allow Custom Script to allow the SharePoint Designer connection.</span></span>

<span data-ttu-id="27f9e-116">Detalizētām darbībām, piemērus un apsvērumi sk [Atļaut vai aizliegt pielāgotu skriptu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="27f9e-116">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


