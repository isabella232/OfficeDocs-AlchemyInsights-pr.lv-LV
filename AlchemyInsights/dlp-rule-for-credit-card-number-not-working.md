---
title: Jūsu kredītkartes numura DLP noteikums nedarbojas
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
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679448"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="d3402-102">DLP problēmas ar kredītkaršu numuriem</span><span class="sxs-lookup"><span data-stu-id="d3402-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="d3402-103">**Svarīgi**: šo bezprecedenta laiku mēs veicam darbības, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir plaši pieejami. Lai iegūtu papildinformāciju, apmeklējiet [SharePoint Online pagaidu līdzekļu pielāgojumi](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="d3402-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="d3402-104">**DLP problēmas ar kredītkaršu numuriem**</span><span class="sxs-lookup"><span data-stu-id="d3402-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="d3402-105">Vai rodas problēmas saistībā ar **datu zuduma novēršanu (DLP)** , kas nestrādā ar saturu, kas satur **kredītkartes numuru** , izmantojot DLP sensitīvas informācijas tipu programmā O365?</span><span class="sxs-lookup"><span data-stu-id="d3402-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="d3402-106">Ja jā, pārliecinieties, vai saturs satur nepieciešamo informāciju, lai aktivizētu DLP politiku, kad tas tiek novērtēts.</span><span class="sxs-lookup"><span data-stu-id="d3402-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="d3402-107">Piemēram, **kredītkaršu politikai** , kas konfigurēta ar 85% ticamības līmeni, tiek novērtētas tālāk norādītās darbības un ir jānosaka, ka kārtula tiek aktivizēta:</span><span class="sxs-lookup"><span data-stu-id="d3402-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="d3402-108">**[Formāts:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 cipari, kas var būt formatēti vai neformatēti (dddddddddddddddd), un ir jāiztur Luhn pārbaude.</span><span class="sxs-lookup"><span data-stu-id="d3402-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="d3402-109">**[Modelis:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Ļoti sarežģīts un robusts modelis, kas atklāj kartes no galvenajiem zīmoliem visā pasaulē, tostarp visa, MasterCard, Discovery Card, JCB, American Express, dāvanu kartes un Diner Cards.</span><span class="sxs-lookup"><span data-stu-id="d3402-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="d3402-110">**[Kontrolsumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Jā, Luhn kontrolsumma</span><span class="sxs-lookup"><span data-stu-id="d3402-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="d3402-111">**[Definīcija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** DLP politika ir 85% pārliecināts, ka tā ir atklājusi šādu sensitīvas informācijas tipu, ja 300.</span><span class="sxs-lookup"><span data-stu-id="d3402-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="d3402-112">Funkcija Func_credit_card atrod saturu, kas atbilst rakstam.</span><span class="sxs-lookup"><span data-stu-id="d3402-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="d3402-113">Ir patiess viens no šiem apgalvojumiem:</span><span class="sxs-lookup"><span data-stu-id="d3402-113">One of the following is true:</span></span>

  - <span data-ttu-id="d3402-114">Ir atrasts atslēgvārds no Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="d3402-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="d3402-115">Ir atrasts atslēgvārds no Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="d3402-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="d3402-116">Funkcija Func_expiration_date atrod datumu pareizajā datuma formātā.</span><span class="sxs-lookup"><span data-stu-id="d3402-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="d3402-117">Kontrolsummas caurlaides</span><span class="sxs-lookup"><span data-stu-id="d3402-117">The checksum passes</span></span>

    <span data-ttu-id="d3402-118">Piemēram, tālāk norādītie paraugi izraisītu DLP kredītkaršu numuru politiku:</span><span class="sxs-lookup"><span data-stu-id="d3402-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="d3402-119">Vīza: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="d3402-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="d3402-120">Derīgums beidzas: 2/2009</span><span class="sxs-lookup"><span data-stu-id="d3402-120">Expires: 2/2009</span></span>

<span data-ttu-id="d3402-121">Lai iegūtu papildinformāciju par to, kas ir nepieciešams **kredītkartes numura** noteikšanai jūsu saturam, skatiet šī raksta nākamajā sadaļā: [kādi ir sensitīvo informācijas tipi](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number) .</span><span class="sxs-lookup"><span data-stu-id="d3402-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span></span>
  
<span data-ttu-id="d3402-122">Citas iebūvētas sensitīvas informācijas tipa izmantošana ir atrodama šajā rakstā, lai iegūtu informāciju par to, kas ir nepieciešams citiem tipiem: [ko nozīmē sensitīvie informācijas tipi](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="d3402-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  