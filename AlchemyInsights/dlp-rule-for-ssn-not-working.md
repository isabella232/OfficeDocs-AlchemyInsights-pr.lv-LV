---
title: Nav darba SSN kārtula DLP
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
ms.openlocfilehash: 0b83a858975ffe1bb70f16a7452a13d57dff5340
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932535"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="589d2-102">DLP jautājumi ar sociālās apdrošināšanas numuriem</span><span class="sxs-lookup"><span data-stu-id="589d2-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="589d2-103">**Svarīgi**: daudzi SharePoint Online un OneDrive klienti darbojas kritiskās biznesa lietojumprogrammas pret pakalpojumu, kas darbojas fonā.</span><span class="sxs-lookup"><span data-stu-id="589d2-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="589d2-104">Tie ietver satura migrācija, datu zuduma novēršana (DLP) un dublēšanas risinājumi.</span><span class="sxs-lookup"><span data-stu-id="589d2-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="589d2-105">Šo bezprecedenta reižu laikā mēs rīkojam, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir ļoti pieejami un uzticami lietotājiem, kuri ir atkarīgi no pakalpojuma vairāk nekā jebkad agrāk attālos darba scenārijos.</span><span class="sxs-lookup"><span data-stu-id="589d2-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="589d2-106">Lai atbalstītu šo mērķi, mēs esam ieviesuši stingrākus ierobežošanas ierobežojumus fona lietotnēs (migrācija, DLP un dublēšanas risinājumi) darba dienās dienas laikā.</span><span class="sxs-lookup"><span data-stu-id="589d2-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="589d2-107">Jums vajadzētu sagaidīt, ka šīs lietojumprogrammas šajā laikā sasniegs ļoti ierobežotu caurlaidspēju.</span><span class="sxs-lookup"><span data-stu-id="589d2-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="589d2-108">Tomēr reģiona vakara un nedēļas nogales stundās pakalpojums būs gatavs apstrādāt ievērojami lielāku pieprasījumu apjomu no fona lietotnēm.</span><span class="sxs-lookup"><span data-stu-id="589d2-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="589d2-109">**DLP problēmas ar SSNs**</span><span class="sxs-lookup"><span data-stu-id="589d2-109">**DLP issues with SSNs**</span></span>

<span data-ttu-id="589d2-110">Vai jums ir problēmas ar **datu zuduma novēršana (DLP)** nestrādā saturu, kas satur **sociālās apdrošināšanas numurs (SSN)** , izmantojot sensitīvu informācijas tipa Office 365?</span><span class="sxs-lookup"><span data-stu-id="589d2-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="589d2-111">Ja tā ir, pārliecinieties, ka jūsu saturs satur nepieciešamo informāciju par to, ko DLP politika meklē.</span><span class="sxs-lookup"><span data-stu-id="589d2-111">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="589d2-112">Piemēram, SSN politika, kas konfigurēta ar ticamības līmeni 85%, tiek novērtēti un ir jānosaka kārtulu aktivizācijai:</span><span class="sxs-lookup"><span data-stu-id="589d2-112">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="589d2-113">**[Formāts:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 cipari, kas var būt formatēts vai Neformatēts raksts</span><span class="sxs-lookup"><span data-stu-id="589d2-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="589d2-114">**[Modelis:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Četras funkcijas meklē SSNs četros dažādos modeļos:</span><span class="sxs-lookup"><span data-stu-id="589d2-114">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="589d2-115">Func_ssn atrod SSNs ar Pre-2011 spēcīgu formatējumu, kas formatēts domuzīmes vai atstarpes (DDD-dd-dddd vai DDD dd dddd)</span><span class="sxs-lookup"><span data-stu-id="589d2-115">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="589d2-116">Func_unformatted_ssn atrod SSNs ar Pre-2011 spēcīgu formatējumu, kas ir Neformatēts kā deviņus secīgus ciparus (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="589d2-116">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="589d2-117">Func_randomized_formatted_ssn atrod pēc-2011 SSNs, kas formatēti ar domuzīmes vai atstarpes (DDD-dd-dddd vai DDD dd dddd)</span><span class="sxs-lookup"><span data-stu-id="589d2-117">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="589d2-118">Func_randomized_unformatted_ssn atrod post-2011 SSNs, kas ir Neformatēts kā deviņus secīgus ciparus (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="589d2-118">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="589d2-119">**[Kontrolsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nē, nav kontrolsummas</span><span class="sxs-lookup"><span data-stu-id="589d2-119">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="589d2-120">**[Definīcija:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP politika ir 85% pārliecināta, ka tā tiek atklāta šāda veida sensitīva informācija, ja tuvums 300 rakstzīmes:</span><span class="sxs-lookup"><span data-stu-id="589d2-120">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="589d2-121">[Funkcija Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) atrod saturu, kas atbilst paraugam.</span><span class="sxs-lookup"><span data-stu-id="589d2-121">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="589d2-122">Tiek atrasts atslēgvārds no [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) .</span><span class="sxs-lookup"><span data-stu-id="589d2-122">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="589d2-123">Atslēgvārdu piemēri ietver: *sociālo nodrošinājumu, sociālo nodrošinājumu #, SOC SEC, SSN* .</span><span class="sxs-lookup"><span data-stu-id="589d2-123">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="589d2-124">Piemēram, šāda parauga izraisītu DLP SSN politika: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="589d2-124">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="589d2-125">Lai iegūtu papildinformāciju par to, kas ir nepieciešams noteikt SSNs saturu, skatiet šajā sadaļā šo rakstu: [kāda sensitīva informācijas tipi meklē SSN](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="589d2-125">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="589d2-126">Izmantojot citu iebūvētu sensitīvo informācijas tipu, skatiet šo rakstu, lai iegūtu informāciju par to, kas ir nepieciešams citiem tipiem: [, kāda veida sensitīvo informācijas veidu meklē](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="589d2-126">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  