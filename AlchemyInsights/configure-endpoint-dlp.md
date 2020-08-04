---
title: Galapunkta DLP konfigurēšana
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 039c8f78c5896b66eab5763fb0bbddd3f0b06f2d
ms.sourcegitcommit: 1dada930649a2625eb6d15910b2bfd5e1e00e5b6
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/03/2020
ms.locfileid: "46555556"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="52589-102">Galapunkta DLP konfigurēšana</span><span class="sxs-lookup"><span data-stu-id="52589-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="52589-103">Microsoft galapunkta DLP sniedz iespēju palielināt DLP aizsardzību un pārraudzības iespējas ar sensitīvu informāciju Windows 10 ierīcēs.</span><span class="sxs-lookup"><span data-stu-id="52589-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="52589-104">Kad ierīces ir ierakstītas ierīču vadībā, varat izveidot DLP politikas, lai īstenotu aizsardzības darbības attiecībā uz vienumiem.</span><span class="sxs-lookup"><span data-stu-id="52589-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="52589-105">Darbību pārlūku var izmantot, lai pārraudzītu darbības sensitīviem vienumiem.</span><span class="sxs-lookup"><span data-stu-id="52589-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="52589-106">Lai iegūtu papildinformāciju, skatiet rakstu [ierīču pievienošana ierīču pārvaldībā](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="52589-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="52589-107">Lai sāktu darbu ar galapunktu DLP:</span><span class="sxs-lookup"><span data-stu-id="52589-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="52589-108">Pārliecinieties, vai jums ir atbilstošas SKU/abonementu licences.</span><span class="sxs-lookup"><span data-stu-id="52589-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="52589-109">Papildinformāciju skatiet rakstā [SKU/abonementu licencēšana](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="52589-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="52589-110">Pārbaudiet, kādas atļaujas ir nepieciešamas, lai iespējotu ierīču pārvaldību, piekļūtu borta lapai vai ieslēgtu/izslēgtu ierīces pārraudzību.</span><span class="sxs-lookup"><span data-stu-id="52589-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="52589-111">Papildinformāciju skatiet rakstā [atļaujas](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="52589-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="52589-112">Borta ierīces ierīces vadībā, veicot procedūru reģistrēšanas ierīces.</span><span class="sxs-lookup"><span data-stu-id="52589-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="52589-113">Ja trūkst ierīces reģistrēšanas (priekšskatījuma) opcijas sadaļā M365 atbilstības **Iestatījumi**, apstipriniet, ka jums ir atbilstošas licences un atļaujas, kas minētas iepriekš.</span><span class="sxs-lookup"><span data-stu-id="52589-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="52589-114">Papildinformāciju skatiet rakstā [ierīču](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices)pievienošana.</span><span class="sxs-lookup"><span data-stu-id="52589-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="52589-115">Izveidojiet DLP politikas, lai aizsargātu konfidenciālus vienumus.</span><span class="sxs-lookup"><span data-stu-id="52589-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="52589-116">Informāciju skatiet rakstā [galapunkta DLP politikas scenāriji](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="52589-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="52589-117">Papildinformāciju par Microsoft galapunkta DLP skatiet rakstā [informācija par microsoft 365 galapunkta datu zuduma novēršanas (priekšskatījums)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="52589-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>