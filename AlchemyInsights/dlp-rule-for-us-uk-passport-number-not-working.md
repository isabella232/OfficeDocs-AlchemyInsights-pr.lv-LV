---
title: DLP rules ASV/Apvienotās Karalistes pases numurs nedarbojas
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679231"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="2bd3d-102">Problēmas ar DLP-US/UK Passport numuriem</span><span class="sxs-lookup"><span data-stu-id="2bd3d-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="2bd3d-103">**Svarīgi**: šo bezprecedenta laiku mēs veicam darbības, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir plaši pieejami. Lai iegūtu papildinformāciju, apmeklējiet [SharePoint Online pagaidu līdzekļu pielāgojumi](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="2bd3d-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="2bd3d-104">**DLP problēmas ar ASV/Apvienotās Karalistes pases numuriem**</span><span class="sxs-lookup"><span data-stu-id="2bd3d-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="2bd3d-105">Vai rodas problēmas saistībā ar **datu zuduma novēršanu (DLP)** , kas nestrādā ar saturu, kas ietver **ASV/Apvienotās Karalistes pases numuru** , ja izmantojat datu tipu DLP ar O365?</span><span class="sxs-lookup"><span data-stu-id="2bd3d-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="2bd3d-106">Ja tā ir, pārliecinieties, vai saturs satur nepieciešamo informāciju par DLP politikas izskatu, kad tas tiek novērtēts.</span><span class="sxs-lookup"><span data-stu-id="2bd3d-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="2bd3d-107">Piemēram, **ASV/Apvienotās Karalistes pases numuru** politikai, kas konfigurēta ar 75% ticamības līmeni, tiek novērtētas un ir jānosaka, ka kārtula tiek aktivizēta</span><span class="sxs-lookup"><span data-stu-id="2bd3d-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="2bd3d-108">**[Formāts:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Deviņi cipari</span><span class="sxs-lookup"><span data-stu-id="2bd3d-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nine digits</span></span>

- <span data-ttu-id="2bd3d-109">**[Modelis:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Deviņi secīgi cipari</span><span class="sxs-lookup"><span data-stu-id="2bd3d-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="2bd3d-110">**[Kontrolsumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nē, nav kontrolsummas</span><span class="sxs-lookup"><span data-stu-id="2bd3d-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="2bd3d-111">**[Definīcija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** DLP politika ir 75% pārliecināts, ka tā ir atklājusi šādu sensitīvas informācijas tipu, ja 300.</span><span class="sxs-lookup"><span data-stu-id="2bd3d-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="2bd3d-112">Funkcija Func_usa_uk_passport atrod saturu, kas atbilst rakstam.</span><span class="sxs-lookup"><span data-stu-id="2bd3d-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="2bd3d-113">Ir atrasts atslēgvārds no Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="2bd3d-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="2bd3d-114">Piemēram, tālāk sniegtais piemērs izraisa **ASV/Apvienotās Karalistes pases numuru** politiku: ASV pases numurs 123456789</span><span class="sxs-lookup"><span data-stu-id="2bd3d-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="2bd3d-115">Lai iegūtu papildinformāciju par to, kas ir nepieciešams ASV/Apvienotās Karalistes pases numura satura noteikšanai, skatiet šī raksta nākamajā sadaļā: [kādi ir sensitīvo informācijas tipi meklēt ASV/Apvienotās Karalistes pases numuru](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="2bd3d-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span></span>
  
<span data-ttu-id="2bd3d-116">Citas iebūvētas sensitīvas informācijas tipa izmantošana ir atrodama šajā rakstā, lai iegūtu informāciju par to, kas ir nepieciešams citiem tipiem: [ko nozīmē sensitīvie informācijas tipi](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="2bd3d-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  