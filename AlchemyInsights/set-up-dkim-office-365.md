---
title: Setup DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0acaed476dbd06bc933bf466f9bf6116413a44bb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509391"
---
# <a name="setup-dkim"></a><span data-ttu-id="10dfb-102">Setup DKIM</span><span class="sxs-lookup"><span data-stu-id="10dfb-102">Setup DKIM</span></span>

<span data-ttu-id="10dfb-103">Pilnu instrukciju konfigurēšana DKIM pielāgotu domēnu Microsoft 365 ir [šeit](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="10dfb-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="10dfb-104">**Katram** pielāgotajam domēnam ir jāizveido **divi** DKIM CNAME ieraksti domēna DNS viesošanas pakalpojumā (parasti domēna reģistrētājā).</span><span class="sxs-lookup"><span data-stu-id="10dfb-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="10dfb-105">Piemēram, contoso.com un fourthcoffee.com nepieciešami četri DKIM CNAME ieraksti: divi contoso.com un divi fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="10dfb-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="10dfb-106">DKIM CNAME ierakstus **katram** pielāgotajam domēnam izmantot šādus formātus:</span><span class="sxs-lookup"><span data-stu-id="10dfb-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="10dfb-107">**Resursdatora nosaukums**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="10dfb-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="10dfb-108">**Norāda uz adresi vai vērtību**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="10dfb-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="10dfb-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="10dfb-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="10dfb-110">**Resursdatora nosaukums**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="10dfb-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="10dfb-111">**Norāda uz adresi vai vērtību**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="10dfb-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="10dfb-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="10dfb-112">**TTL**: 3600</span></span>

   <span data-ttu-id="10dfb-113">\<DomainGUID\>ir teksts pa kreisi no `.mail.protection.outlook.com` Pielāgotā domēna PIELĀGOTĀ MX ieraksta (piemēram, `contoso-com` domēna contoso.com).</span><span class="sxs-lookup"><span data-stu-id="10dfb-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="10dfb-114">\<InitialDomain\>ir domēns, ko izmantojāt, kad reģistrījāties Microsoft 365 (piemēram, contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="10dfb-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="10dfb-115">Kad esat izveidojis CNAME ierakstus pielāgotajiem domēniem, izpildiet tālāk sniegtos norādījumus.</span><span class="sxs-lookup"><span data-stu-id="10dfb-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="10dfb-116">A.</span><span class="sxs-lookup"><span data-stu-id="10dfb-116">a.</span></span> <span data-ttu-id="10dfb-117">[pierakstieties Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) ar savu darba vai skolas kontu.</span><span class="sxs-lookup"><span data-stu-id="10dfb-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="10dfb-118">B.</span><span class="sxs-lookup"><span data-stu-id="10dfb-118">b.</span></span> <span data-ttu-id="10dfb-119">Augšējā kreisajā stūrī atlasiet programmas palaidēja ikonu un izvēlieties **admin**.</span><span class="sxs-lookup"><span data-stu-id="10dfb-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="10dfb-120">C.</span><span class="sxs-lookup"><span data-stu-id="10dfb-120">c.</span></span> <span data-ttu-id="10dfb-121">Apakšējā kreisajā navigācijas, izvērsiet **admin** un izvēlieties **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="10dfb-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="10dfb-122">D.</span><span class="sxs-lookup"><span data-stu-id="10dfb-122">d.</span></span> <span data-ttu-id="10dfb-123">Iet uz **aizsardzība**  >  **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="10dfb-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="10dfb-124">E.</span><span class="sxs-lookup"><span data-stu-id="10dfb-124">e.</span></span> <span data-ttu-id="10dfb-125">Atlasiet domēnu un pēc tam izvēlieties **Iespējot** , lai **parakstītu ziņojumus šim domēnam ar DKIM parakstiem**.</span><span class="sxs-lookup"><span data-stu-id="10dfb-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="10dfb-126">Atkārtojiet šo darbību katram pielāgotajam domēnam.</span><span class="sxs-lookup"><span data-stu-id="10dfb-126">Repeat this step for each custom domain.</span></span>
