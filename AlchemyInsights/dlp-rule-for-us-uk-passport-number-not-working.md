---
title: DLP noteikums ASV/Lielbritānijas pases numurs nedarbojas
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 534e258c31a9a71c618765511487487c53f455b5
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977113"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="ed168-102">Problēmas ar DLP-US/UK pases numuru</span><span class="sxs-lookup"><span data-stu-id="ed168-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="ed168-103">**Svarīgi**: šo bezprecedenta laikos, mēs veikt pasākumus, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir ļoti pieejami-Lūdzu, apmeklējiet [SharePoint Online pagaidu līdzekļu korekcijas](https://aka.ms/ODSPAdjustments) , lai iegūtu vairāk informācijas.</span><span class="sxs-lookup"><span data-stu-id="ed168-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="ed168-104">**DLP jautājumi ar ASV/Lielbritānijas pases numuriem**</span><span class="sxs-lookup"><span data-stu-id="ed168-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="ed168-105">Vai jums ir problēmas ar **datu zuduma novēršana (DLP)** nestrādā par saturu, kas satur **ASV/UK pases numuru** , izmantojot DLP konfidenciālu informāciju tipa O365?</span><span class="sxs-lookup"><span data-stu-id="ed168-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="ed168-106">Ja tā ir, pārliecinieties, ka jūsu saturs satur nepieciešamo informāciju par to, ko DLP politika meklē, kad tas ir novērtēts.</span><span class="sxs-lookup"><span data-stu-id="ed168-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="ed168-107">Piemēram, **ASV/Apvienotās Karalistes pases numuru** politikai, kas konfigurēta ar ticamības līmeni 75%, tiek novērtēti tālāk minētie, un tie ir jānosaka, lai kārtula izraisītu</span><span class="sxs-lookup"><span data-stu-id="ed168-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="ed168-108">**[Formāts:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Deviņi cipari</span><span class="sxs-lookup"><span data-stu-id="ed168-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="ed168-109">**[Modelis:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Deviņus secīgus ciparus</span><span class="sxs-lookup"><span data-stu-id="ed168-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="ed168-110">**[Kontrolsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nē, nav kontrolsummas</span><span class="sxs-lookup"><span data-stu-id="ed168-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="ed168-111">**[Definīcija:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP politika ir 75% pārliecināta, ka tā tiek atklāta šāda veida sensitīva informācija, ja tuvums 300 rakstzīmes:</span><span class="sxs-lookup"><span data-stu-id="ed168-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="ed168-112">Funkcija Func_usa_uk_passport atrod saturu, kas atbilst paraugam.</span><span class="sxs-lookup"><span data-stu-id="ed168-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="ed168-113">Tiek atrasts atslēgvārds no Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="ed168-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="ed168-114">Piemēram, šādu paraugu izraisītu **ASV/Lielbritānijas pases numuru** politika: ASV pases numurs 123456789</span><span class="sxs-lookup"><span data-stu-id="ed168-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="ed168-115">Lai iegūtu papildinformāciju par to, kas ir nepieciešams, lai jūsu saturam tiktu noteikts ASV/Apvienotās Karalistes pases numurs, skatiet šajā rakstā minēto sadaļu: [kādas sensitīvās informācijas veidi meklē US/UK pases numuru](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="ed168-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="ed168-116">Izmantojot citu iebūvētu sensitīvo informācijas tipu, skatiet šo rakstu, lai iegūtu informāciju par to, kas ir nepieciešams citiem tipiem: [, kāda veida sensitīvo informācijas veidu meklē](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="ed168-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  