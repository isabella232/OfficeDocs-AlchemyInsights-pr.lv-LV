---
title: Nedarbojas DLP kārtula kredītkartes numurs
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e2e93bed44749b9017dc6ff919a151d46da7a3fc
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507413"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="19a11-102">DLP problēmas ar kredītkaršu numuriem</span><span class="sxs-lookup"><span data-stu-id="19a11-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="19a11-103">**Svarīgi**: šo bezprecedenta laiku mēs veicam darbības, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir plaši pieejami. Lai iegūtu papildinformāciju, apmeklējiet [SharePoint Online pagaidu līdzekļu pielāgojumi](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="19a11-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="19a11-104">**DLP problēmas ar kredītkaršu numuriem**</span><span class="sxs-lookup"><span data-stu-id="19a11-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="19a11-105">Vai jums ir problēmas ar **datu zuduma novēršana (DLP)** nedarbojas saturu, kas satur **kredītkartes numuru** , izmantojot DLP konfidenciālu informācijas tipu O365?</span><span class="sxs-lookup"><span data-stu-id="19a11-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="19a11-106">Ja tā ir, pārliecinieties, vai saturs satur nepieciešamo informāciju, lai izraisītu DLP politiku, kad tā tiek novērtēta.</span><span class="sxs-lookup"><span data-stu-id="19a11-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="19a11-107">Piemēram, **kredītkartes politikai** , kas konfigurēta ar ticamības līmeni 85%, tiek novērtēti tālāk minētie un ir jānosaka, lai kārtula izraisītu:</span><span class="sxs-lookup"><span data-stu-id="19a11-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="19a11-108">**[Formāts:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 cipari, kurus var formatēt vai Neformatēt (dddddddddddddd), un ir jānokārto Luhn tests.</span><span class="sxs-lookup"><span data-stu-id="19a11-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="19a11-109">**[Modelis:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Ļoti sarežģīts un spēcīgs modelis, kas atrod kārtis no visiem lielākajiem zīmoliem visā pasaulē, ieskaitot visa, MasterCard, Discover Card, JCB, American Express, dāvanu kartes un pusdienotājs kartes.</span><span class="sxs-lookup"><span data-stu-id="19a11-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="19a11-110">**[Kontrolsumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Jā, Luhn kontrolsumma</span><span class="sxs-lookup"><span data-stu-id="19a11-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="19a11-111">**[Definīcija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** DLP politika ir 85% pārliecināta, ka tā tiek atklāta šāda veida sensitīva informācija, ja tuvums 300 rakstzīmes:</span><span class="sxs-lookup"><span data-stu-id="19a11-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="19a11-112">Funkcija Func_credit_card atrod saturu, kas atbilst paraugam.</span><span class="sxs-lookup"><span data-stu-id="19a11-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="19a11-113">Ir spēkā kāds no šiem:</span><span class="sxs-lookup"><span data-stu-id="19a11-113">One of the following is true:</span></span>

  - <span data-ttu-id="19a11-114">Tiek atrasts atslēgvārds no Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="19a11-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="19a11-115">Tiek atrasts atslēgvārds no Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="19a11-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="19a11-116">Funkcija Func_expiration_date atrod datumu pareizajā datuma formātā.</span><span class="sxs-lookup"><span data-stu-id="19a11-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="19a11-117">Kontrolsumma iet</span><span class="sxs-lookup"><span data-stu-id="19a11-117">The checksum passes</span></span>

    <span data-ttu-id="19a11-118">Piemēram, šādu paraugu izraisīs DLP kredītkartes numuru politika:</span><span class="sxs-lookup"><span data-stu-id="19a11-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="19a11-119">Vīza: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="19a11-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="19a11-120">Beidzas: 2/2009</span><span class="sxs-lookup"><span data-stu-id="19a11-120">Expires: 2/2009</span></span>

<span data-ttu-id="19a11-121">Lai iegūtu papildinformāciju par to, kas ir nepieciešams, lai jūsu saturam tiktu noteikts **kredītkartes numurs** , skatiet tālāk minēto sadaļu šajā rakstā: [kādas sensitīvās informācijas veidi](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number) tiek atrasti, izmantojot kredītkarti #</span><span class="sxs-lookup"><span data-stu-id="19a11-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span></span>
  
<span data-ttu-id="19a11-122">Izmantojot citu iebūvētu sensitīvo informācijas tipu, skatiet šo rakstu, lai iegūtu informāciju par to, kas ir nepieciešams citiem tipiem: [, kāda veida sensitīvo informācijas veidu meklē](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="19a11-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  