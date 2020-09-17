---
title: Iestatīšanas DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808714"
---
# <a name="setup-dkim"></a><span data-ttu-id="53546-102">Iestatīšanas DKIM</span><span class="sxs-lookup"><span data-stu-id="53546-102">Setup DKIM</span></span>

<span data-ttu-id="53546-103">Visi norādījumi par DKIM konfigurēšanu pielāgotiem domēniem pakalpojumā Microsoft 365 ir pieejami [šeit](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="53546-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="53546-104">**Katram** pielāgotam domēnam ir jāizveido **divi** DKIM CNAME ieraksti jūsu domēna DNS viesošanas pakalpojumā (parasti domēnu reģistrētājs).</span><span class="sxs-lookup"><span data-stu-id="53546-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="53546-105">Piemēram, contoso.com un fourthcoffee.com prasa četrus DKIM CNAME ierakstus: divas for contoso.com un divas for fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="53546-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="53546-106">DKIM CNAME ieraksti **katram** pielāgotam domēnam tiek izmantoti šādos formātos:</span><span class="sxs-lookup"><span data-stu-id="53546-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="53546-107">**Resursdatora nosaukums**: `selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="53546-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="53546-108">**Norāda uz adresi vai vērtību**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="53546-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="53546-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="53546-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="53546-110">**Resursdatora nosaukums**: `selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="53546-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="53546-111">**Norāda uz adresi vai vērtību**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="53546-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="53546-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="53546-112">**TTL**: 3600</span></span>

   <span data-ttu-id="53546-113">\<DomainGUID\> ir teksts, kas atrodas pa kreisi no pielāgotā `.mail.protection.outlook.com` domēna pielāgotā MX ieraksta (piemēram, `contoso-com` domēna contoso.com).</span><span class="sxs-lookup"><span data-stu-id="53546-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="53546-114">\<InitialDomain\> ir domēns, ko izmantojāt, reģistrējoties Microsoft 365 (piemēram, contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="53546-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="53546-115">Pēc tam, kad esat izveidojis savam pielāgotajiem domēniem CNAME ierakstus, izpildiet šos norādījumus:</span><span class="sxs-lookup"><span data-stu-id="53546-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="53546-116">izveide.</span><span class="sxs-lookup"><span data-stu-id="53546-116">a.</span></span> <span data-ttu-id="53546-117">[pierakstieties pakalpojumā Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) ar savu darba vai mācību iestādes kontu.</span><span class="sxs-lookup"><span data-stu-id="53546-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="53546-118">b.</span><span class="sxs-lookup"><span data-stu-id="53546-118">b.</span></span> <span data-ttu-id="53546-119">Augšējā kreisajā stūrī atlasiet lietojumprogrammu palaidēja ikonu un izvēlieties **administrators**.</span><span class="sxs-lookup"><span data-stu-id="53546-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="53546-120">c.</span><span class="sxs-lookup"><span data-stu-id="53546-120">c.</span></span> <span data-ttu-id="53546-121">Apakšējā kreisajā navigācijas rūtī izvērsiet **administrators** un izvēlieties **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="53546-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="53546-122">d.</span><span class="sxs-lookup"><span data-stu-id="53546-122">d.</span></span> <span data-ttu-id="53546-123">Dodieties uz **aizsardzības**  >  **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="53546-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="53546-124">e.</span><span class="sxs-lookup"><span data-stu-id="53546-124">e.</span></span> <span data-ttu-id="53546-125">Atlasiet domēnu un pēc tam izvēlieties **Iespējot** , lai **parakstītu ziņojumus šajā domēnā ar DKIM parakstiem**.</span><span class="sxs-lookup"><span data-stu-id="53546-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="53546-126">Atkārtojiet šo darbību katram pielāgotam domēnam.</span><span class="sxs-lookup"><span data-stu-id="53546-126">Repeat this step for each custom domain.</span></span>
