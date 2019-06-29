---
title: DLP kārtula nedarbojas SSN
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: fffd355279b064b31c0a8bf60518b15ee1ed1848
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389440"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="123c6-102">DLP problēmas, kas saistītas ar sociālās apdrošināšanas numurus</span><span class="sxs-lookup"><span data-stu-id="123c6-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="123c6-103">Vai jums ir problēmas ar **Datu zaudējumu novēršanas (DLP)** saturu, lietojot Office 365 konfidenciālas informācijas tips, kas satur **Sociālās apdrošināšanas numurs (SAN)** nedarbojas?</span><span class="sxs-lookup"><span data-stu-id="123c6-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="123c6-104">Šādā gadījumā pārliecinieties, ka jūsu saturs satur nepieciešamo informāciju par to, ko meklē DLP politiku.</span><span class="sxs-lookup"><span data-stu-id="123c6-104">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="123c6-105">Piemēram, SSN politikai, kas konfigurēts ar ticamības līmeni, 85 %, šādi tiek novērtētas un ir noteikusi kārtulas, lai iedarbinātu:</span><span class="sxs-lookup"><span data-stu-id="123c6-105">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="123c6-106">**[Formāts:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 cipari, kas var būt paraugs formatētu vai neformatētu</span><span class="sxs-lookup"><span data-stu-id="123c6-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="123c6-107">**[Modelis:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Četras funkcijas meklēt SSNs četrus dažādus modeļus:</span><span class="sxs-lookup"><span data-stu-id="123c6-107">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="123c6-108">Func_ssn atrod SSNs ar pre-2011 spēcīgu formatējumu, kas ir formatētas defises vai atstarpes (ddd dd dddd OR ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="123c6-108">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="123c6-109">Func_unformatted_ssn atrod SSNs ar pre-2011 spēcīgu formatējumu, kas ir formatēta kā deviņus secīgus ciparus (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="123c6-109">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="123c6-110">Func_randomized_formatted_ssn atrod amatā 2011 SSNs, kas ir formatētas defises vai atstarpes (ddd dd dddd OR ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="123c6-110">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="123c6-111">Func_randomized_unformatted_ssn atrod amatā 2011 SSNs, kas ir formatēta kā deviņus secīgus ciparus (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="123c6-111">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="123c6-112">**[Kontrolsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nē, nav neviena kontrolsumma</span><span class="sxs-lookup"><span data-stu-id="123c6-112">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="123c6-113">**[Definīcija:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP politika ir 85 % ir pārliecināti, ka tas ir konstatējusi šāda veida konfidenciālu informāciju, ja laikā tuvumu 300 rakstzīmes:</span><span class="sxs-lookup"><span data-stu-id="123c6-113">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="123c6-114">[Func_ssn funkcija](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) atrod saturu, kas atbilst rakstam.</span><span class="sxs-lookup"><span data-stu-id="123c6-114">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="123c6-115">No [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) atslēgvārds ir atrasts.</span><span class="sxs-lookup"><span data-stu-id="123c6-115">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="123c6-116">Atslēgvārdi piemēri ietver: *sociālās apdrošināšanas, sociālās nodrošināšanas #, Soc. Sec, SSN* .</span><span class="sxs-lookup"><span data-stu-id="123c6-116">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="123c6-117">Piemēram, šādas izlases izraisītu DLP SSN politikā: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="123c6-117">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="123c6-118">Papildinformāciju par to, kādām ir jābūt SSNs tiktu atrasta jūsu saturu, skatiet šī raksta sadaļā šādi: [Kāda jutīgas informācijas tipus meklēt SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="123c6-118">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="123c6-119">Izmantojot dažādas iebūvētas sensitīvu informāciju tipu, skatiet šajā rakstā informāciju par to, kas ir nepieciešami citi veidi: [Meklēt ko jutīgas informācijas veidus](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="123c6-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  