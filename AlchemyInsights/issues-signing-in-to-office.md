---
title: Pierakstīšanās pakalpojumā Office apps jautājumiem
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
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938271"
---
# <a name="blank-sign-in-screen-in-office-apps"></a><span data-ttu-id="b003f-102">Tukša pierakstīšanās ekrāna Office programmās</span><span class="sxs-lookup"><span data-stu-id="b003f-102">Blank sign-in screen in Office apps</span></span>

<span data-ttu-id="b003f-103">Lai atrisinātu šo problēmu, mēģiniet veikt šādas darbības:</span><span class="sxs-lookup"><span data-stu-id="b003f-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="b003f-104">[Windows](https://support.microsoft.com/help/4027667/windows-10-update) un [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)instalētu jaunākos atjauninājumus.</span><span class="sxs-lookup"><span data-stu-id="b003f-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="b003f-105">Atiestatīt programmas Internet Explorer opcijām: iet uz **Tools** > **Interneta opcijas** > **Advanced** > **Atiestatīt Internet Explorer iestatījumus** (ņemiet vērā, ka jūs zaudēsiet pielāgotos iestatījumus) un pēc tam mēģiniet pierakstīties vēlreiz uz biroju.</span><span class="sxs-lookup"><span data-stu-id="b003f-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="b003f-106">Atspējot Windows Defender programma aizsargs (WDAG) vai līdzīgu firewall vai anti-virus programmu:</span><span class="sxs-lookup"><span data-stu-id="b003f-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="b003f-107">Vadības panelī dodieties uz **programmas**un pēc tam izvēlieties **ieslēgt Windows līdzekļu ieslēgšana vai izslēgšana**.</span><span class="sxs-lookup"><span data-stu-id="b003f-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="b003f-108">Aktivizējot Windows Defender programma apsardzes, atspējojiet to.</span><span class="sxs-lookup"><span data-stu-id="b003f-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="b003f-109">**Piezīme:** Jums var būt nepieciešams restartēt datoru.</span><span class="sxs-lookup"><span data-stu-id="b003f-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="b003f-110">Nodrošina, ka Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) nav bloķēti ar jebkuru pieteikumu vai ugunsmūra/anti-virus programmu.</span><span class="sxs-lookup"><span data-stu-id="b003f-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="b003f-111">[Notīrīt biroja akreditācijas datus](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) , izmantojot Windows Credential Manager.</span><span class="sxs-lookup"><span data-stu-id="b003f-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="b003f-112">**Piezīme:** Ir mainījušies 16,0 Office 2016 reģistra ceļus.</span><span class="sxs-lookup"><span data-stu-id="b003f-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="b003f-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="b003f-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="b003f-114">Papildinformāciju skatiet sadaļā [savienojuma problēmas pierakstīšanās pēc Biroja 2016 būvēt 16.0.7967 10 Windows atjauninājums](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="b003f-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>