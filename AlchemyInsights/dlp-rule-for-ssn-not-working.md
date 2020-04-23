---
title: Nav darba SSN kārtula DLP
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 5af843c2b70b5b2e1aaf82c9f01356546929d840
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43788709"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="4c8a9-102">DLP jautājumi ar sociālās apdrošināšanas numuriem</span><span class="sxs-lookup"><span data-stu-id="4c8a9-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="4c8a9-103">**Svarīgi**: šo bezprecedenta laiku mēs veicam darbības, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir plaši pieejami. Lai iegūtu papildinformāciju, apmeklējiet [SharePoint Online pagaidu līdzekļu pielāgojumi](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="4c8a9-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="4c8a9-104">**DLP problēmas ar SSNs**</span><span class="sxs-lookup"><span data-stu-id="4c8a9-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="4c8a9-105">Vai jums ir problēmas ar **datu zuduma novēršana (DLP)** nestrādā saturu, kas satur **sociālās apdrošināšanas numurs (SSN)** , izmantojot sensitīvu informācijas tipa Microsoft 365?</span><span class="sxs-lookup"><span data-stu-id="4c8a9-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="4c8a9-106">Ja tā ir, pārliecinieties, ka jūsu saturs satur nepieciešamo informāciju par to, ko DLP politika meklē.</span><span class="sxs-lookup"><span data-stu-id="4c8a9-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="4c8a9-107">Piemēram, SSN politika, kas konfigurēta ar ticamības līmeni 85%, tiek novērtēti un ir jānosaka kārtulu aktivizācijai:</span><span class="sxs-lookup"><span data-stu-id="4c8a9-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="4c8a9-108">**[Formāts:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 cipari, kas var būt formatēts vai Neformatēts raksts</span><span class="sxs-lookup"><span data-stu-id="4c8a9-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="4c8a9-109">**[Modelis:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Četras funkcijas meklē SSNs četros dažādos modeļos:</span><span class="sxs-lookup"><span data-stu-id="4c8a9-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="4c8a9-110">Func_ssn atrod SSNs ar Pre-2011 spēcīgu formatējumu, kas formatēts domuzīmes vai atstarpes (DDD-dd-dddd vai DDD dd dddd)</span><span class="sxs-lookup"><span data-stu-id="4c8a9-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="4c8a9-111">Func_unformatted_ssn atrod SSNs ar Pre-2011 spēcīgu formatējumu, kas ir Neformatēts kā deviņus secīgus ciparus (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="4c8a9-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="4c8a9-112">Func_randomized_formatted_ssn atrod pēc-2011 SSNs, kas formatēti ar domuzīmes vai atstarpes (DDD-dd-dddd vai DDD dd dddd)</span><span class="sxs-lookup"><span data-stu-id="4c8a9-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="4c8a9-113">Func_randomized_unformatted_ssn atrod post-2011 SSNs, kas ir Neformatēts kā deviņus secīgus ciparus (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="4c8a9-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="4c8a9-114">**[Kontrolsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nē, nav kontrolsummas</span><span class="sxs-lookup"><span data-stu-id="4c8a9-114">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="4c8a9-115">**[Definīcija:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP politika ir 85% pārliecināta, ka tā tiek atklāta šāda veida sensitīva informācija, ja tuvums 300 rakstzīmes:</span><span class="sxs-lookup"><span data-stu-id="4c8a9-115">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="4c8a9-116">[Funkcija Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) atrod saturu, kas atbilst paraugam.</span><span class="sxs-lookup"><span data-stu-id="4c8a9-116">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="4c8a9-117">Tiek atrasts atslēgvārds no [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) .</span><span class="sxs-lookup"><span data-stu-id="4c8a9-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="4c8a9-118">Atslēgvārdu piemēri ietver: *sociālo nodrošinājumu, sociālo nodrošinājumu #, SOC SEC, SSN* .</span><span class="sxs-lookup"><span data-stu-id="4c8a9-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="4c8a9-119">Piemēram, šāda parauga izraisītu DLP SSN politika: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="4c8a9-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="4c8a9-120">Lai iegūtu papildinformāciju par to, kas ir nepieciešams noteikt SSNs saturu, skatiet šajā sadaļā šo rakstu: [kāda sensitīva informācijas tipi meklē SSN](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="4c8a9-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="4c8a9-121">Izmantojot citu iebūvētu sensitīvo informācijas tipu, skatiet šo rakstu, lai iegūtu informāciju par to, kas ir nepieciešams citiem tipiem: [, kāda veida sensitīvo informācijas veidu meklē](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="4c8a9-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  