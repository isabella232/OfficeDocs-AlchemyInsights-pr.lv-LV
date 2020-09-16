---
title: SharePoint Designer savienojuma problēmas
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727178"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="5f7c7-102">SharePoint Designer savienojuma problēmas</span><span class="sxs-lookup"><span data-stu-id="5f7c7-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="5f7c7-103">Ja programmā SharePoint Designer ir radušās savienojuma problēmas ar SharePoint vietnēm, izmēģiniet šos bieži izmantotos risinājumus.</span><span class="sxs-lookup"><span data-stu-id="5f7c7-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="5f7c7-104">1. darbība: Pārbaudiet, vai SharePoint Designer 2013 ir atjaunināts, izmantojot [SharePoint Designer 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) . un [2016 2. augusta SharePoint Designer 2013 atjauninājumu](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="5f7c7-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="5f7c7-105">2. darbība: notīriet lokālos kešatmiņas failus:</span><span class="sxs-lookup"><span data-stu-id="5f7c7-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="5f7c7-106">SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="5f7c7-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="5f7c7-107">Lokālajā datorā noņemiet visus failus, kas atrasti katrā no šīm mapēm.</span><span class="sxs-lookup"><span data-stu-id="5f7c7-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="5f7c7-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="5f7c7-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="5f7c7-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="5f7c7-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="5f7c7-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="5f7c7-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="5f7c7-111">Atveriet SharePoint Designer 2013 un vēlreiz ievadiet kontu, lai uzzinātu, vai tas darbojas.</span><span class="sxs-lookup"><span data-stu-id="5f7c7-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="5f7c7-112">3. darbība: [modernās autentifikācijas iespējošana sistēmai Office 2013 Windows ierīcēs](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="5f7c7-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>

<span data-ttu-id="5f7c7-113">4. darbība: administratoriem ir **jāatļauj pielāgot skriptu** SharePoint administrēšanas centra iestatījumos, lai atļautu SharePoint Designer savienojumu.</span><span class="sxs-lookup"><span data-stu-id="5f7c7-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="5f7c7-114">Papildinformāciju skatiet rakstā [pielāgota skripta atļaušana vai novēršana](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) .</span><span class="sxs-lookup"><span data-stu-id="5f7c7-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


