---
title: DLP kārtula ASV bankas konta numurs nedarbojas
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: bb7d8ca91af73fa4ebed5992ec848128beb18830
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977169"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="cca68-102">DLP problēmas ar ASV bankas kontu numuri</span><span class="sxs-lookup"><span data-stu-id="cca68-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="cca68-103">**Svarīgi**: šo bezprecedenta laikos, mēs veikt pasākumus, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir ļoti pieejami-Lūdzu, apmeklējiet [SharePoint Online pagaidu līdzekļu korekcijas](https://aka.ms/ODSPAdjustments) , lai iegūtu vairāk informācijas.</span><span class="sxs-lookup"><span data-stu-id="cca68-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="cca68-104">**DLP problēmas ar ASV bankas kontu numuri**</span><span class="sxs-lookup"><span data-stu-id="cca68-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="cca68-105">Vai jums ir problēmas ar **datu zuduma novēršana (DLP)** nedarbojas saturu, kas satur **ASV bankas konta numuru** , izmantojot DLP konfidenciālu informācijas tipu O365?</span><span class="sxs-lookup"><span data-stu-id="cca68-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="cca68-106">Ja tā ir, pārliecinieties, ka jūsu saturs satur nepieciešamo informāciju par to, ko DLP politika meklē, kad tas ir novērtēts.</span><span class="sxs-lookup"><span data-stu-id="cca68-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="cca68-107">Piemēram, **ASV bankas konta numuru** politika konfigurēta ar ticamības līmeni 85%, tiek novērtēti un jānosaka kārtulas aktivizācijai:</span><span class="sxs-lookup"><span data-stu-id="cca68-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="cca68-108">**[Formāts:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 cipari</span><span class="sxs-lookup"><span data-stu-id="cca68-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="cca68-109">**[Modelis:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 secīgi cipari.</span><span class="sxs-lookup"><span data-stu-id="cca68-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="cca68-110">**[Kontrolsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nē, nav kontrolsummas</span><span class="sxs-lookup"><span data-stu-id="cca68-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="cca68-111">**[Definīcija:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** DLP politika ir 75% pārliecināta, ka tā tiek atklāta šāda veida sensitīva informācija, ja tuvums 300 rakstzīmes:</span><span class="sxs-lookup"><span data-stu-id="cca68-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="cca68-112">Regulārā izteiksme Regex_usa_bank_account_number atrod saturu, kas atbilst rakstam</span><span class="sxs-lookup"><span data-stu-id="cca68-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="cca68-113">Tiek atrasts atslēgvārds no Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="cca68-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="cca68-114">Piemēram, šādu piemēru varētu izraisīt **ASV bankas konta numuru** politika: norēķinu konts 78344011</span><span class="sxs-lookup"><span data-stu-id="cca68-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="cca68-115">Lai iegūtu papildinformāciju par to, kas ir nepieciešams, lai jūsu saturam tiktu noteikts **ASV bankas konta numurs** , skatiet tālāk minēto sadaļu šajā rakstā: [kāda sensitīva informācijas veida informācija mums šķiet bankas konta numurs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="cca68-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="cca68-116">Izmantojot citu iebūvētu sensitīvo informācijas tipu, skatiet šo rakstu, lai iegūtu informāciju par to, kas ir nepieciešams citiem tipiem: [, kāda veida sensitīvo informācijas veidu meklē](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="cca68-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  