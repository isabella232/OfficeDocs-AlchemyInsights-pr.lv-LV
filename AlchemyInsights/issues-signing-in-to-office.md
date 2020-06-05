---
title: Problēmas pierakstoties Microsoft 365 Apps
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579908"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="d1a75-102">Tukšu pierakstīšanās ekrānu Microsoft 365 Apps</span><span class="sxs-lookup"><span data-stu-id="d1a75-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="d1a75-103">Lai atrisinātu šo problēmu, mēģiniet veikt šādas darbības:</span><span class="sxs-lookup"><span data-stu-id="d1a75-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="d1a75-104">Instalējiet jaunākos [Windows](https://support.microsoft.com/help/4027667/windows-10-update) un [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)atjauninājumus.</span><span class="sxs-lookup"><span data-stu-id="d1a75-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="d1a75-105">Atiestatīt Internet Explorer opcijas: dodieties uz **Rīki**,  >  **interneta opcijas**  >  **Advanced**  >  ,**Atiestatīt Internet Explorer iestatījumus** (ņemiet vērā, ka tiks zaudēti pielāgotie iestatījumi) un pēc tam mēģiniet pierakstīties pakalpojumā Office vēlreiz.</span><span class="sxs-lookup"><span data-stu-id="d1a75-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="d1a75-106">Atspējojiet Windows Defender lietojumprogrammu aizsargs (WDAG) vai citu līdzīgu ugunsmūri vai pretvīrusu programmu:</span><span class="sxs-lookup"><span data-stu-id="d1a75-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="d1a75-107">Vadības panelī atveriet **programmas**un pēc tam izvēlieties **ieslēgt vai izslēgt Windows līdzekļus**.</span><span class="sxs-lookup"><span data-stu-id="d1a75-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="d1a75-108">Ja ir iespējots Windows Defender lietojumprogrammu aizsargs, atspējojiet to.</span><span class="sxs-lookup"><span data-stu-id="d1a75-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="d1a75-109">**Piezīme:** Iespējams, būs jārestartē dators.</span><span class="sxs-lookup"><span data-stu-id="d1a75-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="d1a75-110">Pārliecinieties, ka Microsoft. AAD. BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) nav bloķē jebkura lietojumprogramma vai ugunsmūra/anti-virus programmu.</span><span class="sxs-lookup"><span data-stu-id="d1a75-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="d1a75-111">[Notīrīt Office akreditācijas datus](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) , izmantojot Windows akreditācijas datu pārvaldnieku.</span><span class="sxs-lookup"><span data-stu-id="d1a75-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="d1a75-112">**Piezīme:** Office 2016 reģistra ceļi ir mainījušies 16,0.</span><span class="sxs-lookup"><span data-stu-id="d1a75-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="d1a75-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="d1a75-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="d1a75-114">Lai iegūtu papildinformāciju, skatiet [savienojuma problēmas pierakstīšanās pēc atjauninājuma Office 2016 veidot 16.0.7967 operētājsistēmā Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="d1a75-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>