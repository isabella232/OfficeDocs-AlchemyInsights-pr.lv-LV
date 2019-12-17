---
title: SharePoint Designer savienojuma problēmas
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 9730bd66afd494385db3de605f5fe68d0f274ed3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051720"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="c18d5-102">SharePoint Designer savienojuma problēmas</span><span class="sxs-lookup"><span data-stu-id="c18d5-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="c18d5-103">Ja programmā SharePoint Designer ir radušās savienojuma problēmas ar SharePoint vietnēm, lūdzu, izmēģiniet tālāk minētie Kopīgie risinājumi.</span><span class="sxs-lookup"><span data-stu-id="c18d5-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="c18d5-104">1. darbība: Pārbaudiet, vai SharePoint Designer 2013 tiek atjaunināts ar [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) un [2. augusts 2016 atjaunināt SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="c18d5-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="c18d5-105">2. darbība: notīriet lokālās kešatmiņas failus.</span><span class="sxs-lookup"><span data-stu-id="c18d5-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="c18d5-106">Aizveriet SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="c18d5-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="c18d5-107">Lokālajā datorā, noņemiet visus failus atrasti katrā no šīm mapēm.</span><span class="sxs-lookup"><span data-stu-id="c18d5-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="c18d5-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="c18d5-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="c18d5-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="c18d5-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="c18d5-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="c18d5-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="c18d5-111">Atveriet SharePoint Designer 2013 un ievadiet kontu vēlreiz, lai redzētu, vai tā darbojas.</span><span class="sxs-lookup"><span data-stu-id="c18d5-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="c18d5-112">3. darbība: [Iespējot mūsdienu autentifikācijas Office 2013 Windows ierīcēs](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="c18d5-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span></span>

<span data-ttu-id="c18d5-113">4. darbība: administratoriem ir **jāatļauj pielāgotu skriptu** SharePoint administrēšanas centrs iestatījumus, lai atļautu SharePoint Designer savienojumu.</span><span class="sxs-lookup"><span data-stu-id="c18d5-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="c18d5-114">Papildinformāciju skatiet sadaļā [Atļaut vai aizliegt pielāgotu skriptu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) .</span><span class="sxs-lookup"><span data-stu-id="c18d5-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


