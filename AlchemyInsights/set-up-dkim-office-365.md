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
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645679"
---
# <a name="setup-dkim"></a><span data-ttu-id="f305c-102">Setup DKIM</span><span class="sxs-lookup"><span data-stu-id="f305c-102">Setup DKIM</span></span>

<span data-ttu-id="f305c-103">Pilnu instrukciju konfigurēšana DKIM pielāgotu domēnu Microsoft 365 ir [šeit](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="f305c-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="f305c-104">**Katram** pielāgotajam domēnam ir jāizveido **divi** DKIM CNAME ieraksti domēna DNS viesošanas pakalpojumā (parasti domēna reģistrētājā).</span><span class="sxs-lookup"><span data-stu-id="f305c-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="f305c-105">Piemēram, contoso.com un fourthcoffee.com nepieciešami četri DKIM CNAME ieraksti: divi contoso.com un divi fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="f305c-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="f305c-106">DKIM CNAME ierakstus **katram** pielāgotajam domēnam izmantot šādus formātus:</span><span class="sxs-lookup"><span data-stu-id="f305c-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="f305c-107">**Resursdatora nosaukums**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="f305c-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="f305c-108">**Norāda uz adresi vai vērtību**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="f305c-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="f305c-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="f305c-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="f305c-110">**Resursdatora nosaukums**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="f305c-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="f305c-111">**Norāda uz adresi vai vērtību**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="f305c-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="f305c-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="f305c-112">**TTL**: 3600</span></span>

   <span data-ttu-id="f305c-113">\<DomainGUID\> ir teksts, kas atrodas pa kreisi `.mail.protection.outlook.com` no pielāgotā domēna pielāgotā MX ieraksta (piemēram, `contoso-com` domēna contoso.com).</span><span class="sxs-lookup"><span data-stu-id="f305c-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="f305c-114">\<InitialDomain\> ir domēns, kuru izmantojāt, kad Reģistrījāties Microsoft 365 (piemēram, contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="f305c-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="f305c-115">Kad esat izveidojis CNAME ierakstus pielāgotajiem domēniem, izpildiet tālāk sniegtos norādījumus.</span><span class="sxs-lookup"><span data-stu-id="f305c-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="f305c-116">A.</span><span class="sxs-lookup"><span data-stu-id="f305c-116">a.</span></span> <span data-ttu-id="f305c-117">[pierakstieties Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) ar savu darba vai skolas kontu.</span><span class="sxs-lookup"><span data-stu-id="f305c-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="f305c-118">B.</span><span class="sxs-lookup"><span data-stu-id="f305c-118">b.</span></span> <span data-ttu-id="f305c-119">Augšējā kreisajā stūrī atlasiet programmas palaidēja ikonu un izvēlieties **admin**.</span><span class="sxs-lookup"><span data-stu-id="f305c-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="f305c-120">C.</span><span class="sxs-lookup"><span data-stu-id="f305c-120">c.</span></span> <span data-ttu-id="f305c-121">Apakšējā kreisajā navigācijas, izvērsiet **admin** un izvēlieties **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="f305c-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="f305c-122">D.</span><span class="sxs-lookup"><span data-stu-id="f305c-122">d.</span></span> <span data-ttu-id="f305c-123">Iet uz **aizsardzība** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="f305c-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="f305c-124">E.</span><span class="sxs-lookup"><span data-stu-id="f305c-124">e.</span></span> <span data-ttu-id="f305c-125">Atlasiet domēnu un pēc tam izvēlieties **Iespējot** , lai **parakstītu ziņojumus šim domēnam ar DKIM parakstiem**.</span><span class="sxs-lookup"><span data-stu-id="f305c-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="f305c-126">Atkārtojiet šo darbību katram pielāgotajam domēnam.</span><span class="sxs-lookup"><span data-stu-id="f305c-126">Repeat this step for each custom domain.</span></span>
