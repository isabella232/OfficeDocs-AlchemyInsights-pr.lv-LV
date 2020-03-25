---
title: DLP nedarbojas, kā paredzēts
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932629"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="486ee-102">DLP nedarbojas, kā paredzēts</span><span class="sxs-lookup"><span data-stu-id="486ee-102">DLP not working as expected</span></span>

<span data-ttu-id="486ee-103">**Svarīgi**: daudzi SharePoint Online un OneDrive klienti darbojas kritiskās biznesa lietojumprogrammas pret pakalpojumu, kas darbojas fonā.</span><span class="sxs-lookup"><span data-stu-id="486ee-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="486ee-104">Tie ietver satura migrācija, datu zuduma novēršana (DLP) un dublēšanas risinājumi.</span><span class="sxs-lookup"><span data-stu-id="486ee-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="486ee-105">Šo bezprecedenta reižu laikā mēs rīkojam, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir ļoti pieejami un uzticami lietotājiem, kuri ir atkarīgi no pakalpojuma vairāk nekā jebkad agrāk attālos darba scenārijos.</span><span class="sxs-lookup"><span data-stu-id="486ee-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="486ee-106">Lai atbalstītu šo mērķi, mēs esam ieviesuši stingrākus ierobežošanas ierobežojumus fona lietotnēs (migrācija, DLP un dublēšanas risinājumi) darba dienās dienas laikā.</span><span class="sxs-lookup"><span data-stu-id="486ee-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="486ee-107">Jums vajadzētu sagaidīt, ka šīs lietojumprogrammas šajā laikā sasniegs ļoti ierobežotu caurlaidspēju.</span><span class="sxs-lookup"><span data-stu-id="486ee-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="486ee-108">Tomēr reģiona vakara un nedēļas nogales stundās pakalpojums būs gatavs apstrādāt ievērojami lielāku pieprasījumu apjomu no fona lietotnēm.</span><span class="sxs-lookup"><span data-stu-id="486ee-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

 <span data-ttu-id="486ee-109">**DLP iestatīšana**</span><span class="sxs-lookup"><span data-stu-id="486ee-109">**Setting up DLP**</span></span>

<span data-ttu-id="486ee-110">Vai jums ir problēmas ar **datu zuduma novēršana (DLP)** Office 365 nedarbojas, kā paredzēts?</span><span class="sxs-lookup"><span data-stu-id="486ee-110">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="486ee-111">Ja tā ir, pārliecinieties, vai **DLP politika** ir iestatīta pareizi un jūsu dati satur **DLP politika** meklē, kad tas tiek novērtēts.</span><span class="sxs-lookup"><span data-stu-id="486ee-111">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="486ee-112">DLP politika ļauj identificēt un aizsargāt sensitīvu informāciju jūsu organizācijā.</span><span class="sxs-lookup"><span data-stu-id="486ee-112">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="486ee-113">Lai iestatītu DLP politikas, izmantojiet [šeit](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)informāciju.</span><span class="sxs-lookup"><span data-stu-id="486ee-113">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="486ee-114">**Kāda DLP politika meklē**</span><span class="sxs-lookup"><span data-stu-id="486ee-114">**What DLP policies look for**</span></span>
  
<span data-ttu-id="486ee-115">Izmantojot **iebūvēto sensitīvo informācijas tipu** Office 365 drošības un atbilstības centru, DLP politikas meklēt konkrētu modeļu un elementi, nosakot šo sensitīvo tipu.</span><span class="sxs-lookup"><span data-stu-id="486ee-115">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="486ee-116">**Iebūvēti sensitīvi informācijas veidi**</span><span class="sxs-lookup"><span data-stu-id="486ee-116">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="486ee-117">Lai iegūtu informāciju par iebūvētiem sensitīviem tipiem un to, kāda ir DLP politika, kad tiek noteikta sensitīva tipa noteikšana, skatiet: [kāda veida sensitīvo informācijas tipu meklē](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="486ee-117">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="486ee-118">**Pielāgoti sensitīvi informācijas tipi**</span><span class="sxs-lookup"><span data-stu-id="486ee-118">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="486ee-119">Ja mēģināt izveidot pielāgotu konfidenciālus informācijas tipus, izmantojiet šo rakstu, lai iegūtu informāciju par to, kā izveidot pielāgotu sensitīvu tipu: [izveidojiet pielāgotu sensitīvo informācijas tipu](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="486ee-119">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="486ee-120">**DLP politikas pārbaude**</span><span class="sxs-lookup"><span data-stu-id="486ee-120">**Test a DLP policy**</span></span>

<span data-ttu-id="486ee-121">Lai pārbaudītu datus ar iebūvētu vai pielāgotu sensitīvu informācijas tipu, izmantojiet opciju **testa tips** sadaļā **klasifikācija** > **sensitīvo informācijas tipi**.</span><span class="sxs-lookup"><span data-stu-id="486ee-121">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="486ee-122">Papildinformāciju skatiet sadaļā [pielāgotu sensitīvo informācijas tipu testēšana](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="486ee-122">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="486ee-123">**Ziņojumi**</span><span class="sxs-lookup"><span data-stu-id="486ee-123">**Reports**</span></span>
  
- <span data-ttu-id="486ee-124">Iegūstiet sensitīvu datu ieskati ar [DLP pārskatiem.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="486ee-124">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="486ee-125">Skatiet detalizētu informāciju par notikumu, izmantojot [ziņojumu par incidentu](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="486ee-125">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
