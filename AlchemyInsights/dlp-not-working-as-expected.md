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
ms.openlocfilehash: 0ed893420b5813d5d18639c2c226c12f0306a13f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679700"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="41e50-102">DLP nedarbojas, kā paredzēts</span><span class="sxs-lookup"><span data-stu-id="41e50-102">DLP not working as expected</span></span>

<span data-ttu-id="41e50-103">**Svarīgi**: šo bezprecedenta laiku mēs veicam darbības, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir plaši pieejami. Lai iegūtu papildinformāciju, apmeklējiet [SharePoint Online pagaidu līdzekļu pielāgojumi](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="41e50-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="41e50-104">**DLP iestatīšana**</span><span class="sxs-lookup"><span data-stu-id="41e50-104">**Setting up DLP**</span></span>

<span data-ttu-id="41e50-105">Vai rodas problēmas ar **datu zuduma novēršanu (DLP)** sistēmā Office 365, nedarbojas, kā paredzēts?</span><span class="sxs-lookup"><span data-stu-id="41e50-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="41e50-106">Ja jā, pārliecinieties, vai jūsu **DLP politika** ir iestatīta pareizi, un jūsu datos ir norādīts, kā tiek meklēta **DLP politika** , kad tas tiek novērtēts.</span><span class="sxs-lookup"><span data-stu-id="41e50-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="41e50-107">DLP politikas ļauj identificēt un aizsargāt sensitīvu informāciju jūsu organizācijā.</span><span class="sxs-lookup"><span data-stu-id="41e50-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="41e50-108">Lai iestatītu DLP politikas, izmantojiet [šeit](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)esošo informāciju.</span><span class="sxs-lookup"><span data-stu-id="41e50-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="41e50-109">**Ko DLP politikas meklē**</span><span class="sxs-lookup"><span data-stu-id="41e50-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="41e50-110">Izmantojot **iebūvētos sensitīvos informācijas tipus** drošības un atbilstības centros, DLP politikas meklē konkrētus modeļus un elementus, nosakot šos jutīgos tipus.</span><span class="sxs-lookup"><span data-stu-id="41e50-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="41e50-111">**Iebūvētie sensitīvie informācijas tipi**</span><span class="sxs-lookup"><span data-stu-id="41e50-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="41e50-112">Lai iegūtu informāciju par iebūvētajiem sensitīvajiem tipiem un to, kas ir paredzēts DLP politikai, nosakot sensitīvo tipu, skatiet rakstu: [kā izskatās sensitīvās informācijas tipi](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="41e50-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="41e50-113">**Pielāgoti sensitīvie informācijas tipi**</span><span class="sxs-lookup"><span data-stu-id="41e50-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="41e50-114">Ja mēģināt izveidot pielāgotus sensitīvos informācijas tipus, lai iegūtu informāciju par to, kā izveidot pielāgotu sensitīvu datu tipu, izmantojiet tālāk norādīto [rakstu.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="41e50-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="41e50-115">**DLP politikas pārbaude**</span><span class="sxs-lookup"><span data-stu-id="41e50-115">**Test a DLP policy**</span></span>

<span data-ttu-id="41e50-116">Lai testētu savus datus ar iebūvētu vai pielāgotu sensitīvu informācijas tipu, izmantojiet opciju **testa veids** , kas pieejama sadaļā **klasificēti**  >  **sensitīvi informācijas tipi**.</span><span class="sxs-lookup"><span data-stu-id="41e50-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="41e50-117">Papildinformāciju skatiet rakstā [pielāgotu sensitīvo informācijas tipu pārbaude](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="41e50-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="41e50-118">**Atskaites**</span><span class="sxs-lookup"><span data-stu-id="41e50-118">**Reports**</span></span>
  
- <span data-ttu-id="41e50-119">Iegūstiet sensitīvus datus ieskatu ar [DLP atskaitēm.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="41e50-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="41e50-120">Skatiet detalizētu informāciju par notikumu ar [starpgadījumu atskaiti](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="41e50-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
