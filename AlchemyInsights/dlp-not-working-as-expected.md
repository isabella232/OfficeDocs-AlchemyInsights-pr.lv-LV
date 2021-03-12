---
title: DLP nedarbojas, kā paredzēts
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707817"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="ace7a-102">DLP nedarbojas, kā paredzēts</span><span class="sxs-lookup"><span data-stu-id="ace7a-102">DLP not working as expected</span></span>

<span data-ttu-id="ace7a-103">**Svarīgi**: šo bezprecedenta laiku mēs veicam darbības, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir plaši pieejami. Lai iegūtu papildinformāciju, apmeklējiet [SharePoint Online pagaidu līdzekļu pielāgojumi](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="ace7a-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="ace7a-104">**DLP iestatīšana**</span><span class="sxs-lookup"><span data-stu-id="ace7a-104">**Setting up DLP**</span></span>

<span data-ttu-id="ace7a-105">Vai rodas problēmas ar **datu zuduma novēršanu (DLP)** sistēmā Office 365, nedarbojas, kā paredzēts?</span><span class="sxs-lookup"><span data-stu-id="ace7a-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="ace7a-106">Ja jā, pārliecinieties, vai jūsu **DLP politika** ir iestatīta pareizi, un jūsu datos ir norādīts, kā tiek meklēta **DLP politika** , kad tas tiek novērtēts.</span><span class="sxs-lookup"><span data-stu-id="ace7a-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="ace7a-107">DLP politikas ļauj identificēt un aizsargāt sensitīvu informāciju jūsu organizācijā.</span><span class="sxs-lookup"><span data-stu-id="ace7a-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="ace7a-108">Lai iestatītu DLP politikas, izmantojiet [šeit](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)esošo informāciju.</span><span class="sxs-lookup"><span data-stu-id="ace7a-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).</span></span>
  
 <span data-ttu-id="ace7a-109">**Ko DLP politikas meklē**</span><span class="sxs-lookup"><span data-stu-id="ace7a-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="ace7a-110">Izmantojot **iebūvētos sensitīvos informācijas tipus** drošības un atbilstības centros, DLP politikas meklē konkrētus modeļus un elementus, nosakot šos jutīgos tipus.</span><span class="sxs-lookup"><span data-stu-id="ace7a-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="ace7a-111">**Iebūvētie sensitīvie informācijas tipi**</span><span class="sxs-lookup"><span data-stu-id="ace7a-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="ace7a-112">Lai iegūtu informāciju par iebūvētajiem sensitīvajiem tipiem un to, kas ir paredzēts DLP politikai, nosakot sensitīvo tipu, skatiet rakstu: [kā izskatās sensitīvās informācijas tipi](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="ace7a-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="ace7a-113">**Pielāgoti sensitīvie informācijas tipi**</span><span class="sxs-lookup"><span data-stu-id="ace7a-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="ace7a-114">Ja mēģināt izveidot pielāgotus sensitīvos informācijas tipus, lai iegūtu informāciju par to, kā izveidot pielāgotu sensitīvu datu tipu, izmantojiet tālāk norādīto [rakstu.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="ace7a-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="ace7a-115">**DLP politikas pārbaude**</span><span class="sxs-lookup"><span data-stu-id="ace7a-115">**Test a DLP policy**</span></span>

<span data-ttu-id="ace7a-116">Lai testētu savus datus ar iebūvētu vai pielāgotu sensitīvu informācijas tipu, izmantojiet opciju **testa veids** , kas pieejama sadaļā **klasificēti**  >  **sensitīvi informācijas tipi**.</span><span class="sxs-lookup"><span data-stu-id="ace7a-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="ace7a-117">Papildinformāciju skatiet rakstā [pielāgotu sensitīvo informācijas tipu pārbaude](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="ace7a-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="ace7a-118">**Atskaites**</span><span class="sxs-lookup"><span data-stu-id="ace7a-118">**Reports**</span></span>
  
- <span data-ttu-id="ace7a-119">Iegūstiet sensitīvus datus ieskatu ar [DLP atskaitēm.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="ace7a-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="ace7a-120">Skatiet detalizētu informāciju par notikumu ar [starpgadījumu atskaiti](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="ace7a-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
