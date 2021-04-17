---
title: Problēmas ar pierakstīšanos Microsoft 365 programmās
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833046"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="050fc-102">Tukšs pierakstīšanās ekrāns Microsoft 365 programmās</span><span class="sxs-lookup"><span data-stu-id="050fc-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="050fc-103">Lai novērstu šo problēmu, mēģiniet veikt šādas darbības:</span><span class="sxs-lookup"><span data-stu-id="050fc-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="050fc-104">Instalējiet jaunākos [Windows un](https://support.microsoft.com/help/4027667/windows-10-update) [Office atjauninājumus.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="050fc-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="050fc-105">Atiestatiet Internet Explorer opcijas. Dodieties uz Sadaļu Rīki Interneta opcijas Internet Explorer papildu atiestatīšanas iestatījumi (ņemiet vērā, ka zaudēsit pielāgotos iestatījumus) un pēc tam vēlreiz mēģiniet  >    >    >   pierakstīties sistēmā Office.</span><span class="sxs-lookup"><span data-stu-id="050fc-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="050fc-106">Atspējojiet Windows Defender Application Guard (WDAG) vai citu līdzīgu ugunsmūri vai pretvīrusu programmu:</span><span class="sxs-lookup"><span data-stu-id="050fc-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="050fc-107">Vadības panelī dodieties uz **sadaļu Programmas** un pēc tam **izvēlieties Ieslēgt vai izslēgt Windows līdzekļus.**</span><span class="sxs-lookup"><span data-stu-id="050fc-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="050fc-108">Ja līdzeklis Windows Defender Application Guard ir iespējots, mēģiniet to atspējot.</span><span class="sxs-lookup"><span data-stu-id="050fc-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="050fc-109">**Piezīme.** Iespējams, būs jārestartē dators.</span><span class="sxs-lookup"><span data-stu-id="050fc-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="050fc-110">Pārliecinieties, vai Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) spraudni nebloķē neviena lietojumprogramma vai ugunsmūra/pretvīrusu programma.</span><span class="sxs-lookup"><span data-stu-id="050fc-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="050fc-111">[Notīriet Office akreditācijas](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) datus, izmantojot Windows akreditācijas datu pārvaldnieku.</span><span class="sxs-lookup"><span data-stu-id="050fc-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="050fc-112">**Piezīme.** Office 2016 reģistra ceļi ir mainīti uz 16.0.</span><span class="sxs-lookup"><span data-stu-id="050fc-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="050fc-113">(Piemēram, \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="050fc-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="050fc-114">Papildinformāciju skatiet rakstā Savienojuma problēmas pierakstoties pēc atjaunināšanas uz [Office 2016 būvējumu 16.0.7967 operētājsistēmā Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)</span><span class="sxs-lookup"><span data-stu-id="050fc-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>