---
title: Galapunkta DLP konfigurēšana
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657936"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="8ec46-102">Galapunkta DLP konfigurēšana</span><span class="sxs-lookup"><span data-stu-id="8ec46-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="8ec46-103">Microsoft galapunkta DLP ļauj paplašināt DLP aizsardzību un uzraudzības iespējas, iekļaujot sensitīvu informāciju Windows 10 ierīcēs.</span><span class="sxs-lookup"><span data-stu-id="8ec46-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="8ec46-104">Pēc tam, kad ierīces ir iekļautas ierīču pārvaldībā, varat izveidot DLP politikas, lai ieviestu informācijas aizsardzības darbības ar vienumiem.</span><span class="sxs-lookup"><span data-stu-id="8ec46-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="8ec46-105">Darbību pārlūku var izmantot, lai pārraudzītu sensitīvu vienumu darbības.</span><span class="sxs-lookup"><span data-stu-id="8ec46-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="8ec46-106">Papildinformāciju skatiet rakstā [Ierīču pievienošana ierīču pārvaldībai](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="8ec46-106">For more info, see [Onboarding devices into device management](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="8ec46-107">Lai sāktu darbu ar Galapunkta DLP.</span><span class="sxs-lookup"><span data-stu-id="8ec46-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="8ec46-108">Pārliecinieties, vai jums ir atbilstoša SKU/abonementu licencēšana.</span><span class="sxs-lookup"><span data-stu-id="8ec46-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="8ec46-109">Papildinformāciju skatiet rakstā [SKU/abonementu licencēšanas](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="8ec46-109">For more info, see [SKU/subscriptions licensing](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="8ec46-110">Pārbaudiet atļaujas, kas nepieciešamas, lai iespējotu ierīces pārvaldību, piekļūtu pievienošanas lapai vai ieslēgtu/izslēgtu ierīces uzraudzību.</span><span class="sxs-lookup"><span data-stu-id="8ec46-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="8ec46-111">Papildinformāciju skatiet rakstā [Licenču piešķiršana](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="8ec46-111">For more info, see [Permissions](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="8ec46-112">Pievienojiet ierīces ierīču pārvaldībai, veicot pievienošanas ierīču procedūru.</span><span class="sxs-lookup"><span data-stu-id="8ec46-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="8ec46-113">Papildinformāciju skatiet rakstā [Ierīču pievienošana](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="8ec46-113">For more info, see [Onboarding devices](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="8ec46-114">Izveidojiet DLP politikas, lai aizsargātu savus sensitīvos vienumus.</span><span class="sxs-lookup"><span data-stu-id="8ec46-114">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="8ec46-115">Papildinformāciju skatiet rakstā [Galapunkta DLP politikas scenāriji](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="8ec46-115">For info, see [Endpoint DLP policy scenarios](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="8ec46-116">Papildinformāciju par Microsoft galapunkta DLP skatiet rakstā [Papildinformācija par Microsoft 365 galapunkta datu zuduma novēršanu (priekšskatījums)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="8ec46-116">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="8ec46-117">**Svarīgas datu apkopošanas darbības, ja nepieciešams atbalsts.**</span><span class="sxs-lookup"><span data-stu-id="8ec46-117">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="8ec46-118">Lejupielādējiet [MDATP klienta analizētāja priekšskatījumu.](https://aka.ms/betamdatpanalyzer)</span><span class="sxs-lookup"><span data-stu-id="8ec46-118">Download [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span></span>
1. <span data-ttu-id="8ec46-119">Palaidiet rīku kā administrators, izmantojot cmd logu:</span><span class="sxs-lookup"><span data-stu-id="8ec46-119">Run the tool as Admin from the cmd window:</span></span>

    <span data-ttu-id="8ec46-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span><span class="sxs-lookup"><span data-stu-id="8ec46-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span></span>

1. <span data-ttu-id="8ec46-121">Ja tiek **prasīts, kā ievadīt izsekošanas apkopošanas minūšu skaitu:**, ievadiet minūšu skaitu, kas nepieciešams scenārija izpildē.</span><span class="sxs-lookup"><span data-stu-id="8ec46-121">When prompted with **Enter the number of minutes to collect traces:**, enter the number of minutes required to run the scenario.</span></span>
1. <span data-ttu-id="8ec46-122">Palaidiet scenāriju.</span><span class="sxs-lookup"><span data-stu-id="8ec46-122">Run the scenario.</span></span>

<span data-ttu-id="8ec46-123">Apkopojiet ZIP faila izvadi, lai to sniegtu atbalsta dienesta pārstāvim.</span><span class="sxs-lookup"><span data-stu-id="8ec46-123">Collect the Zip file output to give to the Support agent.</span></span>
