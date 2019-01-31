---
title: DLP kārtula nedarbojas kredītkartes numuru
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 4b8897c5cc8286bc4bd49860658a5a94ad17380d
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/30/2019
ms.locfileid: "29657474"
---
<span data-ttu-id="1f3fb-p101">Vai jums ir problēmas ar **Datu zaudējumu novēršanas (DLP)** nav darba saturs, kurā **Kredītkartes numuru** , lietojot DLP sensitīvu informāciju tipa O365? Šādā gadījumā pārliecinieties, ka jūsu saturs ietver visu vajadzīgo informāciju, lai iedarbinātu DLP politiku, ja tas tiek novērtēts. Piemēram, **kredītkaršu politikas** konfigurēta ar ticamības līmeni, 85 % šādu tiek novērtētas un ir noteikusi kārtulas, lai iedarbinātu:</span><span class="sxs-lookup"><span data-stu-id="1f3fb-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated. For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="1f3fb-105">**[Formāts:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 cipari, kuru var formatēt vai neformatētu (dddddddddddddddd) un jāiziet Luhn tests.</span><span class="sxs-lookup"><span data-stu-id="1f3fb-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span> 
    
- <span data-ttu-id="1f3fb-106">**[Modelis:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Ļoti sarežģīta un spēcīgu modelis, kas atklāj kārtis no visiem galvenajiem zīmoliem visā pasaulē, tai skaitā Visa, Mastercard, Discover Card, JCB, American Express, dāvanu kartes un pusdienotājs kārtis.</span><span class="sxs-lookup"><span data-stu-id="1f3fb-106">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span> 
    
- <span data-ttu-id="1f3fb-107">**[Kontrolsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Jā, Luhn kontrolsumma</span><span class="sxs-lookup"><span data-stu-id="1f3fb-107">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span> 
    
- <span data-ttu-id="1f3fb-108">**[Definīcija:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP politika ir 85 % ir pārliecināti, ka tas ir konstatējusi šāda veida konfidenciālu informāciju, ja laikā tuvumu 300 rakstzīmes:</span><span class="sxs-lookup"><span data-stu-id="1f3fb-108">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="1f3fb-109">Func_credit_card funkcija konstatē saturu, kas atbilst rakstam.</span><span class="sxs-lookup"><span data-stu-id="1f3fb-109">The function Func_credit_card finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="1f3fb-110">Ir spēkā kāds no šiem:</span><span class="sxs-lookup"><span data-stu-id="1f3fb-110">One of the following is true:</span></span> 
    
  - <span data-ttu-id="1f3fb-111">No Keyword_cc_verification atslēgvārds ir atrasts.</span><span class="sxs-lookup"><span data-stu-id="1f3fb-111">A keyword from Keyword_cc_verification is found.</span></span>
    
  - <span data-ttu-id="1f3fb-112">No Keyword_cc_name atslēgvārds ir atrasts</span><span class="sxs-lookup"><span data-stu-id="1f3fb-112">A keyword from Keyword_cc_name is found</span></span>
    
  - <span data-ttu-id="1f3fb-113">Func_expiration_date funkcija atrod datuma pareizā datuma formātā.</span><span class="sxs-lookup"><span data-stu-id="1f3fb-113">The function Func_expiration_date finds a date in the right date format.</span></span>
    
  - <span data-ttu-id="1f3fb-114">Kontrolsumma caurlaides</span><span class="sxs-lookup"><span data-stu-id="1f3fb-114">The checksum passes</span></span>
    
    <span data-ttu-id="1f3fb-115">Piemēram, šādas izlases izraisītu DLP kredītkartes numuru politiku:</span><span class="sxs-lookup"><span data-stu-id="1f3fb-115">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>
    
  - <span data-ttu-id="1f3fb-116">Vīzas: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="1f3fb-116">Visa: 4485 3647 3952 7352</span></span> 
    
  - <span data-ttu-id="1f3fb-117">Expires: 2/2009</span><span class="sxs-lookup"><span data-stu-id="1f3fb-117">Expires: 2/2009</span></span>
    
<span data-ttu-id="1f3fb-118">Papildinformāciju par to, kas tiek prasīts **Kredītkartes numurs** tiktu atrasta jūsu saturu, skatiet šī raksta sadaļā šādi: [Ko jutīgas informācijas tipus meklēt kredītkartes #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="1f3fb-118">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="1f3fb-119">Izmantojot dažādas iebūvētas sensitīvu informāciju tipu, skatiet šajā rakstā informāciju par to, kas ir nepieciešami citi veidi: [Meklēt ko jutīgas informācijas veidus](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="1f3fb-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

