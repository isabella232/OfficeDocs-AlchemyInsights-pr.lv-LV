---
title: Microsoft Intune izmantošana, lai pārvaldītu piekļuvi tīmeklim pārlūkprogrammā Microsoft Edge darbam ar iOS un Android
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003846"
- "6895"
- "9006502"
- "11144"
ms.openlocfilehash: a6c6f9563933b7cf6b71c4758c29ffd94617c4be
ms.sourcegitcommit: 7a406a3d4680662e81f0056454f7e25fb2f52504
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/17/2021
ms.locfileid: "52989681"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="e3438-102">Microsoft Intune izmantošana, lai pārvaldītu piekļuvi tīmeklim pārlūkprogrammā Microsoft Edge darbam ar iOS un Android</span><span class="sxs-lookup"><span data-stu-id="e3438-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="e3438-103">Microsoft Edge iOS un Android ierīcēm ļauj lietotājam pārlūkot tīmekli no vairākiem pilnībā atsevišķiem profiliem.</span><span class="sxs-lookup"><span data-stu-id="e3438-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="e3438-104">Platākās aizsardzības iespējas Microsoft 365 datiem kļūst pieejamas, ja abonējat Enterprise Mobility + Security komplektu, kurā ietilpst Microsoft Intune un Azure Active Directory Premium līdzekļi, piemēram, nosacījuma piekļuve.</span><span class="sxs-lookup"><span data-stu-id="e3438-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="e3438-105">Jūs vēlaties ieviest nosacījumu piekļuves politiku, (1) ļauj lietotājiem izveidot savienojumu no mobilajām ierīcēm ar Microsoft Edge operētājsistēmām iOS un Android un šī (2) ievieš Microsoft Intune programmu aizsardzības politiku, kas nodrošina aizsargātas pārlūkošanas iespējas.</span><span class="sxs-lookup"><span data-stu-id="e3438-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="e3438-106">Lai saprastu, kā varat izmantot nosacījum piekļuvi un politikas, skatiet:</span><span class="sxs-lookup"><span data-stu-id="e3438-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="e3438-107">Azure Active Directory nosacījum piekļuves politiku lietot</span><span class="sxs-lookup"><span data-stu-id="e3438-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="e3438-108">Microsoft Intune programmu aizsardzības politiku izveide</span><span class="sxs-lookup"><span data-stu-id="e3438-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="e3438-109">Vienotās pierakstīšanās izmantošana Azure Active Directory tīmekļa lietojumprogrammām, kas pievienotas ar politiku aizsargātās pārlūkprogrammās</span><span class="sxs-lookup"><span data-stu-id="e3438-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="e3438-110">Izmantojiet programmu konfigurāciju, lai pārvaldītu pārlūkošanas iespējas</span><span class="sxs-lookup"><span data-stu-id="e3438-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="e3438-111">Atļaut izmantot tikai darba un mācību iestādes kontus</span><span class="sxs-lookup"><span data-stu-id="e3438-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="e3438-112">Vispārīgo programmu konfigurācijas politiku izvietošana</span><span class="sxs-lookup"><span data-stu-id="e3438-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="e3438-113">Lietojumprogrammu konfigurācijas politiku izvietošana datu aizsardzībai</span><span class="sxs-lookup"><span data-stu-id="e3438-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="e3438-114">Microsoft Endpoint Manager izmantošana, lai izvietotu programmu konfigurācijas politikas</span><span class="sxs-lookup"><span data-stu-id="e3438-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="e3438-115">Lai uzzinātu, kā piekļūt pārvaldīto programmu žurnāliem, skatiet rakstu Microsoft Edge darbam ar iOS un Android izmantošana, lai piekļūtu [pārvaldītajiem programmu žurnāliem.](https://go.microsoft.com/fwlink/?linkid=2132578)</span><span class="sxs-lookup"><span data-stu-id="e3438-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
