---
title: DKIM Office 365 uzstādīšanas
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: dd908db6a4bc1739b3c1cff059387034d67e093d
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666271"
---
# <a name="setup-dkim-in-office-365"></a><span data-ttu-id="d56c0-102">DKIM Office 365 uzstādīšanas</span><span class="sxs-lookup"><span data-stu-id="d56c0-102">Setup DKIM in Office 365</span></span>

<span data-ttu-id="d56c0-103">Pilnīgas instrukcijas konfigurēšanai DKIM pielāgotiem domēniem Office 365 ir [šeit](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="d56c0-103">The complete instructions for configuring DKIM for custom domains in Office 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="d56c0-104">Par **katru** pielāgoto domēnu, jums ir nepieciešams, lai izveidotu **divas** DKIM CNAME ierakstu jūsu domēna DNS viesošanas pakalpojumā (parasti, domēnu reģistrators).</span><span class="sxs-lookup"><span data-stu-id="d56c0-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="d56c0-105">Piemēram, contoso.com un fourthcoffee.com prasīt četrus DKIM CNAME ierakstu: divi contoso.com un divus fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="d56c0-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="d56c0-106">DKIM CNAME ierakstus par **katru** pielāgoto domēnu izmantot šādus formātus:</span><span class="sxs-lookup"><span data-stu-id="d56c0-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="d56c0-107">**Host nosaukums**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="d56c0-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="d56c0-108">**Norāda uz adresi vai vērtību**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="d56c0-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="d56c0-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="d56c0-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="d56c0-110">**Host nosaukums**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="d56c0-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="d56c0-111">**Norāda uz adresi vai vērtību**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="d56c0-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="d56c0-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="d56c0-112">**TTL**: 3600</span></span>

   <span data-ttu-id="d56c0-113">\<DomainGUID\> ir pa kreisi no teksta `.mail.protection.outlook.com` pielāgotu MX ierakstā par pielāgoto domēnu (piemēram, `contoso-com` par domēnu contoso.com).</span><span class="sxs-lookup"><span data-stu-id="d56c0-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="d56c0-114">\<InitialDomain\> ir domēnu izmantojāt reģistrējoties Office 365 (piemēram, contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="d56c0-114">\<InitialDomain\> is the domain you used when you signed up for Office 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="d56c0-115">Pēc tam, kad esat izveidojis CNAME ierakstu jūsu pielāgoto domēnu, izpildiet šādus norādījumus:</span><span class="sxs-lookup"><span data-stu-id="d56c0-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="d56c0-116">a.</span><span class="sxs-lookup"><span data-stu-id="d56c0-116">a.</span></span> <span data-ttu-id="d56c0-117">[Office 365 pierakstīties](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) ar jūsu darba vai skolas konts.</span><span class="sxs-lookup"><span data-stu-id="d56c0-117">[Sign in to Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="d56c0-118">b.</span><span class="sxs-lookup"><span data-stu-id="d56c0-118">b.</span></span> <span data-ttu-id="d56c0-119">Atlasiet app granātmetējs ikonu augšējā kreisajā un izvēlieties **Admin**.</span><span class="sxs-lookup"><span data-stu-id="d56c0-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="d56c0-120">c.</span><span class="sxs-lookup"><span data-stu-id="d56c0-120">c.</span></span> <span data-ttu-id="d56c0-121">Apakšējā kreisajā navigācijas, izvērsiet **Admin** un izvēlieties **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="d56c0-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="d56c0-122">d.</span><span class="sxs-lookup"><span data-stu-id="d56c0-122">d.</span></span> <span data-ttu-id="d56c0-123">Dodieties uz **aizsardzības** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="d56c0-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="d56c0-124">e.</span><span class="sxs-lookup"><span data-stu-id="d56c0-124">e.</span></span> <span data-ttu-id="d56c0-125">Atlasiet domēnu un pēc tam izvēlieties **Iespējot** **parakstīt**ziņojumu šim domēnam ar DKIM parakstiem.</span><span class="sxs-lookup"><span data-stu-id="d56c0-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="d56c0-126">Atkārtojiet šo darbību ar katru pielāgoto domēnu.</span><span class="sxs-lookup"><span data-stu-id="d56c0-126">Repeat this step for each custom domain.</span></span>
