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
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402437"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="0222f-102">Galapunkta DLP konfigurēšana</span><span class="sxs-lookup"><span data-stu-id="0222f-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="0222f-103">Microsoft galapunkta DLP ļauj paplašināt DLP aizsardzību un uzraudzības iespējas, iekļaujot sensitīvu informāciju Windows 10 ierīcēs.</span><span class="sxs-lookup"><span data-stu-id="0222f-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="0222f-104">Pēc tam, kad ierīces ir iekļautas ierīču pārvaldībā, varat izveidot DLP politikas, lai ieviestu informācijas aizsardzības darbības ar vienumiem.</span><span class="sxs-lookup"><span data-stu-id="0222f-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="0222f-105">Darbību pārlūku var izmantot, lai pārraudzītu sensitīvu vienumu darbības.</span><span class="sxs-lookup"><span data-stu-id="0222f-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="0222f-106">Papildinformāciju skatiet rakstā [Ierīču pievienošana ierīču pārvaldībai](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="0222f-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="0222f-107">Lai sāktu darbu ar Galapunkta DLP.</span><span class="sxs-lookup"><span data-stu-id="0222f-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="0222f-108">Pārliecinieties, vai jums ir atbilstoša SKU/abonementu licencēšana.</span><span class="sxs-lookup"><span data-stu-id="0222f-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="0222f-109">Papildinformāciju skatiet rakstā [SKU/abonementu licencēšanas](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="0222f-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="0222f-110">Pārbaudiet atļaujas, kas nepieciešamas, lai iespējotu ierīces pārvaldību, piekļūtu pievienošanas lapai vai ieslēgtu/izslēgtu ierīces uzraudzību.</span><span class="sxs-lookup"><span data-stu-id="0222f-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="0222f-111">Papildinformāciju skatiet rakstā [Licenču piešķiršana](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="0222f-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="0222f-112">Pievienojiet ierīces ierīču pārvaldībai, veicot pievienošanas ierīču procedūru.</span><span class="sxs-lookup"><span data-stu-id="0222f-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="0222f-113">Ja sadaļā M365 atbilstības **iestatījumi** trūkst opcijas Ierīces iebūvēšana (priekšskatījums), pārliecinieties, ka jums ir iepriekš minētā atbilstošā licence un atļaujas.</span><span class="sxs-lookup"><span data-stu-id="0222f-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="0222f-114">Papildinformāciju skatiet rakstā [Ierīču pievienošana](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="0222f-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="0222f-115">Izveidojiet DLP politikas, lai aizsargātu savus sensitīvos vienumus.</span><span class="sxs-lookup"><span data-stu-id="0222f-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="0222f-116">Papildinformāciju skatiet rakstā [Galapunkta DLP politikas scenāriji](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="0222f-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span></span>

<span data-ttu-id="0222f-117">Papildinformāciju par Microsoft galapunkta DLP skatiet rakstā [Papildinformācija par Microsoft 365 galapunkta datu zuduma novēršanu (priekšskatījums)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="0222f-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="0222f-118">**Svarīgas datu apkopošanas darbības, ja nepieciešams atbalsts.**</span><span class="sxs-lookup"><span data-stu-id="0222f-118">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="0222f-119">Lejupielādējiet MDATP klienta analizētāja priekšskatījumu no [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span><span class="sxs-lookup"><span data-stu-id="0222f-119">Download MDATP Client Analyzer Preview from [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span></span>
2. <span data-ttu-id="0222f-120">Palaidiet rīku kā administrators, izmantojot cmd logu:</span><span class="sxs-lookup"><span data-stu-id="0222f-120">Run the tool as Admin from the cmd window:</span></span>
3. <span data-ttu-id="0222f-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span><span class="sxs-lookup"><span data-stu-id="0222f-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span></span>
4. <span data-ttu-id="0222f-122">Kad tiek prasīts “Ievadiet minūšu skaitu, lai apkopotu izsekošanas vaicājumus:”, ievadiet minūšu skaitu, kas nepieciešams scenārija izpildei</span><span class="sxs-lookup"><span data-stu-id="0222f-122">When prompted with “Enter the number of minutes to collect traces: ", enter the number of minutes that are required to run the scenario</span></span>
5. <span data-ttu-id="0222f-123">Palaist scenāriju</span><span class="sxs-lookup"><span data-stu-id="0222f-123">Run the scenario</span></span>

<span data-ttu-id="0222f-124">Zip faila izvades apkopošana, kas jāpiešķir atbalsta dienesta darbiniekam.</span><span class="sxs-lookup"><span data-stu-id="0222f-124">Collect the Zip file output to be given to the Support agent.</span></span>
