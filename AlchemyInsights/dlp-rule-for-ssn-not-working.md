---
title: Ar SSN nedarbojošos DLP kārtulu
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679376"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="9a260-102">DLP problēmas ar sociālās drošības numuriem</span><span class="sxs-lookup"><span data-stu-id="9a260-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="9a260-103">**Svarīgi**: šo bezprecedenta laiku mēs veicam darbības, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir plaši pieejami. Lai iegūtu papildinformāciju, apmeklējiet [SharePoint Online pagaidu līdzekļu pielāgojumi](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="9a260-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="9a260-104">**DLP problēmas ar SSNs**</span><span class="sxs-lookup"><span data-stu-id="9a260-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="9a260-105">Vai rodas problēmas ar **datu zuduma novēršanu (DLP)** , kas nestrādā ar saturu, kurā ir iekļauts **sociālās drošības numurs (SAN)** , ja programmā Microsoft 365 izmantojat sensitīvu informācijas tipu?</span><span class="sxs-lookup"><span data-stu-id="9a260-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="9a260-106">Ja tā ir, pārliecinieties, vai saturs satur nepieciešamo informāciju par DLP politikas izskatu.</span><span class="sxs-lookup"><span data-stu-id="9a260-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="9a260-107">Piemēram, ja SSN politika ir konfigurēta ar 85% ticamības līmeni, tiek novērtēti tālāk norādītie un ir jānosaka, ka kārtula tiek aktivizēta:</span><span class="sxs-lookup"><span data-stu-id="9a260-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="9a260-108">**[Formāts:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 cipari, kas var būt formatētā vai neformatētā modelī</span><span class="sxs-lookup"><span data-stu-id="9a260-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="9a260-109">**[Modelis:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Četras funkcijas meklē SSNs četros dažādos modeļos:</span><span class="sxs-lookup"><span data-stu-id="9a260-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="9a260-110">Func_ssn atrod SSNs, izmantojot iepriekš 2011 stipru formatējumu, kas formatēts ar defisēm vai atstarpēm (DDD-dd-dddd vai DDD dd dddd)</span><span class="sxs-lookup"><span data-stu-id="9a260-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="9a260-111">Func_unformatted_ssn atrod SSNs, izmantojot iepriekš 2011 stipru formatējumu, kas nav formatēts kā deviņi secīgi cipari (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="9a260-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="9a260-112">Func_randomized_formatted_ssn atrod ziņu par 2011 SSNs, kas formatēta ar defisēm vai atstarpēm (DDD-dd-dddd vai DDD dd dddd)</span><span class="sxs-lookup"><span data-stu-id="9a260-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="9a260-113">Func_randomized_unformatted_ssn atrod post-2011 SSNs, kas nav formatēti kā deviņi secīgi cipari (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="9a260-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="9a260-114">**[Kontrolsumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Nē, nav kontrolsummas</span><span class="sxs-lookup"><span data-stu-id="9a260-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="9a260-115">**[Definīcija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** DLP politika ir 85% pārliecināts, ka tā ir atklājusi šādu sensitīvas informācijas tipu, ja 300.</span><span class="sxs-lookup"><span data-stu-id="9a260-115">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="9a260-116">[Funkcija Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) atrod saturu, kas atbilst rakstam.</span><span class="sxs-lookup"><span data-stu-id="9a260-116">The [function Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="9a260-117">Ir atrasts atslēgvārds no [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) .</span><span class="sxs-lookup"><span data-stu-id="9a260-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) is found.</span></span> <span data-ttu-id="9a260-118">Atslēgvārdu piemēri ietver:  *Social Security, Social Security #, SOC SEC, SSN*  .</span><span class="sxs-lookup"><span data-stu-id="9a260-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="9a260-119">Piemēram, tālāk sniegtais piemērs izraisa DLP SSN politiku: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="9a260-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="9a260-120">Lai iegūtu papildinformāciju par to [, kas ir](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn) nepieciešams, lai SSNs jūsu saturam, skatiet tālāk šajā rakstā norādītās iespējas.</span><span class="sxs-lookup"><span data-stu-id="9a260-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="9a260-121">Citas iebūvētas sensitīvas informācijas tipa izmantošana ir atrodama šajā rakstā, lai iegūtu informāciju par to, kas ir nepieciešams citiem tipiem: [ko nozīmē sensitīvie informācijas tipi](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="9a260-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  