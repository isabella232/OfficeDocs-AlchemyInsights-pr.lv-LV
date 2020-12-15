---
title: Microsoft Intune izmantošana, lai pārvaldītu tīmekļa piekļuvi pārlūkprogrammā Microsoft Edge darbam ar iOS un Android
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
ms.openlocfilehash: 4d6ab4df4ff9588ce5052421602e347c76c91c3f
ms.sourcegitcommit: a7952283882d341515623d5ae58eda14d0553449
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/10/2020
ms.locfileid: "49678260"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="02a3d-102">Microsoft Intune izmantošana, lai pārvaldītu tīmekļa piekļuvi pārlūkprogrammā Microsoft Edge darbam ar iOS un Android</span><span class="sxs-lookup"><span data-stu-id="02a3d-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="02a3d-103">Microsoft Edge darbam ar iOS un Android ļauj lietotājam pārlūkot tīmekli no vairākiem pilnīgi atsevišķiem profiliem.</span><span class="sxs-lookup"><span data-stu-id="02a3d-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="02a3d-104">Microsoft 365 datu lielākās aizsardzības iespējas kļūst pieejamas, ja abonējat Enterprise Mobility + Security Suite, kurā ietilpst Microsoft Intune un Azure Active Directory Premium līdzekļi, piemēram, piekļuve nosacījumam.</span><span class="sxs-lookup"><span data-stu-id="02a3d-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="02a3d-105">Vismaz jūs vēlaties izvietot nosacījuma piekļuves politiku, kas (1) ļauj lietotājiem izveidot savienojumu no mobilajām ierīcēm uz pārlūkprogrammu Microsoft Edge operētājsistēmai iOS un Android un (2) ievieš Microsoft Intune programmu aizsardzības politiku, kas nodrošina aizsargātu pārlūkošanas pieredzi.</span><span class="sxs-lookup"><span data-stu-id="02a3d-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="02a3d-106">Lai izprastu, kā varat izmantot ierobežotu piekļuvi un politikas, skatiet:</span><span class="sxs-lookup"><span data-stu-id="02a3d-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="02a3d-107">Azure Active Directory nosacījuma piekļuves politikas lietošana</span><span class="sxs-lookup"><span data-stu-id="02a3d-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="02a3d-108">Microsoft Intune programmu aizsardzības politiku izveide</span><span class="sxs-lookup"><span data-stu-id="02a3d-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="02a3d-109">Vienotās pierakstīšanās izmantošana pakalpojumam Azure Active Directory — Savienotās tīmekļa lietojumprogrammas politikas aizsargātās pārlūkprogrammās</span><span class="sxs-lookup"><span data-stu-id="02a3d-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="02a3d-110">Lietojumprogrammas konfigurācijas izmantošana, lai pārvaldītu pārlūkošanas pieredzi</span><span class="sxs-lookup"><span data-stu-id="02a3d-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="02a3d-111">Atļaut tikai darba un mācību kontu lietošanu</span><span class="sxs-lookup"><span data-stu-id="02a3d-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="02a3d-112">Vispārīgo programmu konfigurācijas politiku izvietošana</span><span class="sxs-lookup"><span data-stu-id="02a3d-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="02a3d-113">Lietojumprogrammas konfigurācijas politikas izvietošana datu aizsardzībai</span><span class="sxs-lookup"><span data-stu-id="02a3d-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="02a3d-114">Microsoft Endpoint Manager izmantošana, lai izvietotu lietojumprogrammas konfigurācijas politikas</span><span class="sxs-lookup"><span data-stu-id="02a3d-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="02a3d-115">Lai uzzinātu, kā piekļūt pārvaldīto lietojumprogrammu žurnāliem, skatiet rakstu [Microsoft Edge darbam ar iOS un Android izmantošana, lai piekļūtu pārvaldīto lietojumprogrammu žurnāliem](https://go.microsoft.com/fwlink/?linkid=2132578).</span><span class="sxs-lookup"><span data-stu-id="02a3d-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
