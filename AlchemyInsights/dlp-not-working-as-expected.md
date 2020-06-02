---
title: DLP nedarbojas, kā paredzēts
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: e96904e2f0da2fe1fafb3f8722465eaf22681b71
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507485"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="abe8b-102">DLP nedarbojas, kā paredzēts</span><span class="sxs-lookup"><span data-stu-id="abe8b-102">DLP not working as expected</span></span>

<span data-ttu-id="abe8b-103">**Svarīgi**: šo bezprecedenta laiku mēs veicam darbības, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir plaši pieejami. Lai iegūtu papildinformāciju, apmeklējiet [SharePoint Online pagaidu līdzekļu pielāgojumi](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="abe8b-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="abe8b-104">**DLP iestatīšana**</span><span class="sxs-lookup"><span data-stu-id="abe8b-104">**Setting up DLP**</span></span>

<span data-ttu-id="abe8b-105">Vai jums ir problēmas ar **datu zuduma novēršana (DLP)** Office 365 nedarbojas, kā paredzēts?</span><span class="sxs-lookup"><span data-stu-id="abe8b-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="abe8b-106">Ja tā ir, pārliecinieties, vai **DLP politika** ir iestatīta pareizi un jūsu dati satur **DLP politika** meklē, kad tas tiek novērtēts.</span><span class="sxs-lookup"><span data-stu-id="abe8b-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="abe8b-107">DLP politika ļauj identificēt un aizsargāt sensitīvu informāciju jūsu organizācijā.</span><span class="sxs-lookup"><span data-stu-id="abe8b-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="abe8b-108">Lai iestatītu DLP politikas, izmantojiet [šeit](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)informāciju.</span><span class="sxs-lookup"><span data-stu-id="abe8b-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="abe8b-109">**Kāda DLP politika meklē**</span><span class="sxs-lookup"><span data-stu-id="abe8b-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="abe8b-110">Izmantojot **iebūvēto sensitīvo informācijas tipu** drošības un atbilstības centros, DLP politikas meklēt konkrētu modeļu un elementi, nosakot šo sensitīvo tipu.</span><span class="sxs-lookup"><span data-stu-id="abe8b-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="abe8b-111">**Iebūvēti sensitīvi informācijas veidi**</span><span class="sxs-lookup"><span data-stu-id="abe8b-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="abe8b-112">Lai iegūtu informāciju par iebūvētiem sensitīviem tipiem un to, kāda ir DLP politika, kad tiek noteikta sensitīva tipa noteikšana, skatiet: [kāda veida sensitīvo informācijas tipu meklē](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="abe8b-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="abe8b-113">**Pielāgoti sensitīvi informācijas tipi**</span><span class="sxs-lookup"><span data-stu-id="abe8b-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="abe8b-114">Ja mēģināt izveidot pielāgotu konfidenciālus informācijas tipus, izmantojiet šo rakstu, lai iegūtu informāciju par to, kā izveidot pielāgotu sensitīvu tipu: [izveidojiet pielāgotu sensitīvo informācijas tipu](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="abe8b-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="abe8b-115">**DLP politikas pārbaude**</span><span class="sxs-lookup"><span data-stu-id="abe8b-115">**Test a DLP policy**</span></span>

<span data-ttu-id="abe8b-116">Lai pārbaudītu datus ar iebūvētu vai pielāgotu sensitīvu informācijas tipu, izmantojiet opciju **testa tips** sadaļā **klasifikācija**  >  **sensitīvo informācijas tipi**.</span><span class="sxs-lookup"><span data-stu-id="abe8b-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="abe8b-117">Papildinformāciju skatiet sadaļā [pielāgotu sensitīvo informācijas tipu testēšana](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="abe8b-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="abe8b-118">**Ziņojumi**</span><span class="sxs-lookup"><span data-stu-id="abe8b-118">**Reports**</span></span>
  
- <span data-ttu-id="abe8b-119">Iegūstiet sensitīvu datu ieskati ar [DLP pārskatiem.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="abe8b-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="abe8b-120">Skatiet detalizētu informāciju par notikumu, izmantojot [ziņojumu par incidentu](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="abe8b-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
