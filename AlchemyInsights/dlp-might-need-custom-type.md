---
title: DLP var būt nepieciešams pielāgots tips
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 872fca326065ada002300061c951620b3d9a8d0e
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052908"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="f9162-102">DLP var būt nepieciešams pielāgots tips</span><span class="sxs-lookup"><span data-stu-id="f9162-102">DLP might need a custom type</span></span>

<span data-ttu-id="f9162-103">Ar datu zuduma novēršanas (DLP) politiku jūs varat identificēt un aizsargāt sensitīvus datus savā organizācijā.</span><span class="sxs-lookup"><span data-stu-id="f9162-103">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="f9162-104">Dažos gadījumos, lai aizsargātu savas organizācijas datus, iespējams, vajadzēs izveidot **pielāgotu** sensitīvo informācijas tipu.</span><span class="sxs-lookup"><span data-stu-id="f9162-104">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="f9162-105">Piemēram, jūsu organizācijai var būt nepieciešams identificēt un aizsargāt darbinieku ID vai citus datus noteiktā formātā, kas specifisks jūsu organizācijai. Ja tā ir, skatiet šos rakstus, lai iegūtu papildinformāciju.</span><span class="sxs-lookup"><span data-stu-id="f9162-105">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="f9162-106">**Iebūvēta sensitīva informācijas tipa pielāgošana**</span><span class="sxs-lookup"><span data-stu-id="f9162-106">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="f9162-107">Ja iebūvētais sensitīvo informācijas tips atbilst jūsu vajadzībām, izmantojot tikai dažas tweaks, varat [pielāgot iebūvēto sensitīvo informācijas tipu](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="f9162-107">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="f9162-108">Piemēram, varat pievienot vai noņemt atslēgvārdus vai pievienot vai noņemt apstiprinošus pierādījumus, piemēram, datumu vai adresi.</span><span class="sxs-lookup"><span data-stu-id="f9162-108">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="f9162-109">**Pielāgota sensitīva informācijas tipa izveide**</span><span class="sxs-lookup"><span data-stu-id="f9162-109">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="f9162-110">Tomēr, ja jums ir jāidentificē un jāaizsargā cita veida sensitīva informācija, varat [izveidot pielāgotu sensitīvo informācijas tipu](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) drošības & atbilstības centra lietotāja interfeisā.</span><span class="sxs-lookup"><span data-stu-id="f9162-110">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="f9162-111">**Pielāgota sensitīva informācijas tipa izveide drošības & atbilstības centra PowerShell**</span><span class="sxs-lookup"><span data-stu-id="f9162-111">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="f9162-112">Visbeidzot, ja UI nesniedz visas jums nepieciešamo opciju, [drošības & atbilstības centra PowerShell var izveidot pielāgotu sensitīvu informācijas tipu](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="f9162-112">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="f9162-113">Sākot ar XML failu, var izmantot visas pieejamās opcijas.</span><span class="sxs-lookup"><span data-stu-id="f9162-113">By starting with an XML file, you can use every option available.</span></span>
