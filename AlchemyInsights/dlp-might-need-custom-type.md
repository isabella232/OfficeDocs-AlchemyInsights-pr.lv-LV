---
title: DLP, iespējams, ir jābūt pielāgotam tipam
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 72b16d437f97de27cbdc364f022c3e2059b31ef0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712191"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="98add-102">DLP, iespējams, ir jābūt pielāgotam tipam</span><span class="sxs-lookup"><span data-stu-id="98add-102">DLP might need a custom type</span></span>

<span data-ttu-id="98add-103">**Svarīgi**: šo bezprecedenta laiku mēs veicam darbības, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir plaši pieejami. Lai iegūtu papildinformāciju, apmeklējiet [SharePoint Online pagaidu līdzekļu pielāgojumi](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="98add-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="98add-104">**DLP var būt nepieciešams pielāgotas informācijas tips**</span><span class="sxs-lookup"><span data-stu-id="98add-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="98add-105">Izmantojot datu zuduma novēršanas (DLP) politiku, varat identificēt un aizsargāt konfidenciālus datus savā organizācijā.</span><span class="sxs-lookup"><span data-stu-id="98add-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="98add-106">Lai aizsargātu savas organizācijas datus, dažos scenārijos var būt nepieciešams izveidot savu **pielāgoto** sensitīvās informācijas tipu.</span><span class="sxs-lookup"><span data-stu-id="98add-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="98add-107">Piemēram, jūsu organizācijai, iespējams, ir jāidentificē un jāaizsargā darbinieku ID vai citi dati kādā jūsu organizācijas specifiskā formātā. Ja tā ir, skatiet tālāk norādītos rakstus, lai iegūtu papildinformāciju.</span><span class="sxs-lookup"><span data-stu-id="98add-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="98add-108">**Iebūvētas sensitīvas informācijas tipa pielāgošana**</span><span class="sxs-lookup"><span data-stu-id="98add-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="98add-109">Ja iebūvētais sensitīvās informācijas tips atbilst jūsu vajadzībām, izmantojot tikai dažas tweaks, varat [pielāgot iebūvēto sensitīvās informācijas tipu](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="98add-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="98add-110">Piemēram, varat pievienot vai noņemt atslēgvārdus vai pievienot vai noņemt apstiprinošus pierādījumus, piemēram, datumu vai adresi.</span><span class="sxs-lookup"><span data-stu-id="98add-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="98add-111">**Pielāgota sensitīvas informācijas tipa izveide**</span><span class="sxs-lookup"><span data-stu-id="98add-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="98add-112">Taču, ja ir jāidentificē un jāaizsargā dažāda veida konfidenciāla informācija, varat [izveidot pielāgotu sensitīvas informācijas tipu](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) drošības & atbilstības centra lietotāja interfeisā.</span><span class="sxs-lookup"><span data-stu-id="98add-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="98add-113">**Pielāgota sensitīvas informācijas tipa izveide drošības & atbilstības centra PowerShell**</span><span class="sxs-lookup"><span data-stu-id="98add-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="98add-114">Visbeidzot, ja UI nenodrošina visas nepieciešamās opcijas, varat [izveidot pielāgotu sensitīvas informācijas tipu drošības & atbilstības centra PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="98add-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="98add-115">Sākot ar XML failu, varat izmantot visas pieejamās opcijas.</span><span class="sxs-lookup"><span data-stu-id="98add-115">By starting with an XML file, you can use every option available.</span></span>
