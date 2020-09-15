---
title: DLP rules ASV bankas konta numurs nedarbojas
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679303"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="85d54-102">DLP problēmas ar ASV bankas kontu numuriem</span><span class="sxs-lookup"><span data-stu-id="85d54-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="85d54-103">**Svarīgi**: šo bezprecedenta laiku mēs veicam darbības, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir plaši pieejami. Lai iegūtu papildinformāciju, apmeklējiet [SharePoint Online pagaidu līdzekļu pielāgojumi](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="85d54-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="85d54-104">**DLP problēmas ar ASV bankas kontu numuriem**</span><span class="sxs-lookup"><span data-stu-id="85d54-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="85d54-105">Vai rodas problēmas saistībā ar **datu zuduma novēršanu (DLP)** , kas nestrādā ar saturu, kas satur **ASV bankas konta numuru** , izmantojot DLP sensitīvas informācijas tipu programmā O365?</span><span class="sxs-lookup"><span data-stu-id="85d54-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="85d54-106">Ja tā ir, pārliecinieties, vai saturs satur nepieciešamo informāciju par DLP politikas izskatu, kad tas tiek novērtēts.</span><span class="sxs-lookup"><span data-stu-id="85d54-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="85d54-107">Piemēram, ja **ASV bankas konta numura** politika ir konfigurēta ar 85% ticamības līmeni, tiek novērtētas tālāk norādītās darbības, kas ir jāatrod, lai kārtula tiktu aktivizēta:</span><span class="sxs-lookup"><span data-stu-id="85d54-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="85d54-108">**[Formāts:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 cipari</span><span class="sxs-lookup"><span data-stu-id="85d54-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="85d54-109">**[Modelis:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 secīgi skaitļi.</span><span class="sxs-lookup"><span data-stu-id="85d54-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="85d54-110">**[Kontrolsumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nē, nav kontrolsummas</span><span class="sxs-lookup"><span data-stu-id="85d54-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="85d54-111">**[Definīcija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** DLP politika ir 75% pārliecināts, ka tā ir atklājusi šādu sensitīvas informācijas tipu, ja 300.</span><span class="sxs-lookup"><span data-stu-id="85d54-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="85d54-112">Parastā izteiksme Regex_usa_bank_account_number atrod saturu, kas atbilst rakstam</span><span class="sxs-lookup"><span data-stu-id="85d54-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="85d54-113">Ir atrasts atslēgvārds no Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="85d54-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="85d54-114">Piemēram, tālāk sniegtais piemērs izraisa **ASV bankas konta numura** politiku: konta 78344011 pārbaude</span><span class="sxs-lookup"><span data-stu-id="85d54-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="85d54-115">Lai iegūtu papildinformāciju par to, kas ir nepieciešams **ASV bankas konta numura** noteikšanai, skatiet šī raksta nākamajā sadaļā: [kādi ir sensitīvo informācijas tipi meklēt ASV bankas konta numuru](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="85d54-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span></span>
  
<span data-ttu-id="85d54-116">Citas iebūvētas sensitīvas informācijas tipa izmantošana ir atrodama šajā rakstā, lai iegūtu informāciju par to, kas ir nepieciešams citiem tipiem: [ko nozīmē sensitīvie informācijas tipi](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="85d54-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  