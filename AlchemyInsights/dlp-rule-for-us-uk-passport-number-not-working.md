---
title: DLP kārtula US / UK pases numurs nedarbojas
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: ec7f11676982b56a46c83bf276c2212ce765ba6f
ms.sourcegitcommit: ca06ef831226d629de3057a0df85e017b80f3356
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/08/2019
ms.locfileid: "29786705"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="b3b63-102">Problēmas ar DLP - US / UK pases numuri</span><span class="sxs-lookup"><span data-stu-id="b3b63-102">Problems with DLP - US/UK Passport Numbers</span></span>

<span data-ttu-id="b3b63-p101">Vai rodas problēmas ar darba saturu, kas satur **Datu zaudējumu novēršanas (DLP)** **ASV / UK pases numurs** lietojot DLP sensitīvu informāciju tipa O365? Šādā gadījumā pārliecinieties, ka jūsu saturs satur nepieciešamo informāciju par to, ko meklē DLP politikas, kad tās tiek novērtētas.</span><span class="sxs-lookup"><span data-stu-id="b3b63-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK Passport Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="b3b63-105">Piemēram, **US / UK pases numurs** politika, kas konfigurēts ar 75 % ticamības pakāpei, šādi tiek novērtētas un ir noteikusi kārtulas, lai iedarbinātu</span><span class="sxs-lookup"><span data-stu-id="b3b63-105">For example, for a **US/UK Passport Number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span> 
  
- <span data-ttu-id="b3b63-106">**[Formāts:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Deviņu ciparu</span><span class="sxs-lookup"><span data-stu-id="b3b63-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span> 
    
- <span data-ttu-id="b3b63-107">**[Modelis:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Deviņus secīgus ciparus</span><span class="sxs-lookup"><span data-stu-id="b3b63-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span> 
    
- <span data-ttu-id="b3b63-108">**[Kontrolsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nē, nav neviena kontrolsumma</span><span class="sxs-lookup"><span data-stu-id="b3b63-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="b3b63-109">**[Definīcija:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP politika ir 75 % ir pārliecināti, ka tas ir konstatējusi šāda veida konfidenciālu informāciju, ja laikā tuvumu 300 rakstzīmes:</span><span class="sxs-lookup"><span data-stu-id="b3b63-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="b3b63-110">Func_usa_uk_passport funkcija konstatē saturu, kas atbilst rakstam.</span><span class="sxs-lookup"><span data-stu-id="b3b63-110">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="b3b63-111">No Keyword_passport atslēgvārds ir atrasts.</span><span class="sxs-lookup"><span data-stu-id="b3b63-111">A keyword from Keyword_passport is found.</span></span>
    
    <span data-ttu-id="b3b63-112">Piemēram, lai izraisītu šādu paraugu **US / UK pases numurs** politika: ASV pases numurs 123456789</span><span class="sxs-lookup"><span data-stu-id="b3b63-112">For example, the following sample would trigger for the **US/UK Passport Number** policy: U.S. Passport number 123456789</span></span> 
    
<span data-ttu-id="b3b63-113">Lai iegūtu vairāk informācijas par to, kas ir nepieciešama ASV / UK pases numurs tiktu atrasta jūsu saturu, skatiet nākošo sadaļu šajā pantā: [ko jutīgas informācijas tipus meklēt ASV / UK pases numurs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="b3b63-113">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="b3b63-114">Izmantojot dažādas iebūvētas sensitīvu informāciju tipu, skatiet šajā rakstā informāciju par to, kas ir nepieciešami citi veidi: [Meklēt ko jutīgas informācijas veidus](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="b3b63-114">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

