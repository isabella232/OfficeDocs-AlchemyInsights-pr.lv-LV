---
title: Darbs ar autentifikācijas bibliotēkām
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035828"
---
# <a name="working-with-authentication-libraries"></a><span data-ttu-id="b9af1-102">Darbs ar autentifikācijas bibliotēkām</span><span class="sxs-lookup"><span data-stu-id="b9af1-102">Working with Authentication Libraries</span></span>

<span data-ttu-id="b9af1-103">Lai atrisinātu Microsoft autentifikācijas bibliotēkas (MSAL) problēmu, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="b9af1-103">To resolve Microsoft Authentication Library (MSAL) issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="b9af1-104">**Darbs ar MSAL**: [Microsoft identitātes platformas autentifikācijas bibliotēkas](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) — šis raksts rāda Microsoft autentifikācijas bibliotēkas atbalstu vairākiem lietojumprogrammas tipiem.</span><span class="sxs-lookup"><span data-stu-id="b9af1-104">**Working with MSAL**: [Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - This article shows Microsoft Authentication Library support for several application types.</span></span> <span data-ttu-id="b9af1-105">Tajā ir iekļautas saites uz bibliotēkas avota kodu; kur iegūt pakotnes lietojumprogrammas projektu. un vai bibliotēka atbalsta lietotāja pierakstīšanos (autentifikāciju), piekļuvi aizsargātajiem tīmekļa API (autorizācija) vai abiem.</span><span class="sxs-lookup"><span data-stu-id="b9af1-105">It includes links to library source code; where to get the package for your app's project; and whether the library supports user sign-in (authentication), access to protected web APIs (authorization), or both.</span></span>

2. <span data-ttu-id="b9af1-106">**Autentifikācijas problēmu novēršana**: MSAL atbalsta vairākas autentifikācijas plūsmas, kas jāizmanto dažādos lietojumprogrammas scenārijos.</span><span class="sxs-lookup"><span data-stu-id="b9af1-106">**Troubleshoot Authentication**: The MSAL supports several authentication flows for use in different application scenarios.</span></span> <span data-ttu-id="b9af1-107">Atkarībā no tā, kā jūsu klienta lietojumprogramma ir veidota, MSAL var izmantot vienu vai vairākas autentifikācijas plūsmas, ko atbalsta Microsoft Identity Platform.</span><span class="sxs-lookup"><span data-stu-id="b9af1-107">Depending on how your client application is built, the MSAL can use one or more of the authentication flows supported by the Microsoft identity platform.</span></span> <span data-ttu-id="b9af1-108">Šīs plūsmas var izveidot dažāda veida marķierus un autorizācijas kodus, kā arī pieprasīt atšķirīgas pilnvaras, lai tās darbotos.</span><span class="sxs-lookup"><span data-stu-id="b9af1-108">These flows can produce several types of tokens and authorization codes, and require different tokens to make them work.</span></span>

3. <span data-ttu-id="b9af1-109">**Piekļuves pilnvaras**: [Microsoft identitātes platformas piekļuves marķieri](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) — Uzziniet, kā jūsu API var validēt un izmantot prasības piekļuves pilnvarā.</span><span class="sxs-lookup"><span data-stu-id="b9af1-109">**Access Tokens**: [Microsoft identity platform access tokens](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - Learn how your API can validate and use the claims inside an access token.</span></span> <span data-ttu-id="b9af1-110">Visa šī raksta dokumentācija, izņemot gadījumus, kad tas ir norādīts, attiecas tikai uz pilnvarām, kas emitētas par jūsu reģistrēto API.</span><span class="sxs-lookup"><span data-stu-id="b9af1-110">All documentation in this article, except where noted, applies only to tokens issued for APIs you've registered.</span></span> <span data-ttu-id="b9af1-111">Tas neattiecas uz pilnvarām, kas ir izsniegtas korporācijai Microsoft piederošiem API, un šīs pilnvaras nevar izmantot, lai validētu, kā Microsoft identitātes platforma izdos marķierus jūsu izveidotajam API.</span><span class="sxs-lookup"><span data-stu-id="b9af1-111">It does not apply to tokens issued for Microsoft-owned APIs, nor can those tokens be used to validate how the Microsoft identity platform will issue tokens for an API you create.</span></span>

<span data-ttu-id="b9af1-112">**Azure Active Directory autentifikācijas bibliotēkas atbalsta beigas (ADAL)**</span><span class="sxs-lookup"><span data-stu-id="b9af1-112">**End of support for Azure Active Directory Authentication Library (ADAL)**</span></span>

- <span data-ttu-id="b9af1-113">**Sākot no 30. jūnija, 2020,** vairs nepievienosit nekādus jaunus līdzekļus, kas ADAL un Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="b9af1-113">**Starting June 30th, 2020,** we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="b9af1-114">Mēs turpināsim nodrošināt tehnisko atbalstu un drošības atjauninājumus, bet vairs nenodrošināsim līdzekļu atjauninājumus.</span><span class="sxs-lookup"><span data-stu-id="b9af1-114">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>
- <span data-ttu-id="b9af1-115">**Sākot no 30. jūnija, 2022,** mēs NODROŠINĀSIM atbalstu ADAL un Azure AD Graph un vairs nenodrošinās tehnisko atbalstu vai drošības atjauninājumus.</span><span class="sxs-lookup"><span data-stu-id="b9af1-115">**Starting June 30th, 2022,** we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>
- <span data-ttu-id="b9af1-116">Programmas, kas, izmantojot ADAL, pēc šī laika turpinās darboties, bet *nesaņem nekādu tehnisku atbalstu vai drošības atjauninājumus*.</span><span class="sxs-lookup"><span data-stu-id="b9af1-116">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>
- <span data-ttu-id="b9af1-117">Lietojumprogrammas, kas izmanto Azure AD Graph pēc šī laika, iespējams, vairs nesaņems atbildes no Azure AD Graph galapunkta.</span><span class="sxs-lookup"><span data-stu-id="b9af1-117">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="b9af1-118">**PārADAL migrācija**</span><span class="sxs-lookup"><span data-stu-id="b9af1-118">**ADAL Migration**</span></span>

- <span data-ttu-id="b9af1-119">Ieteicams atjaunināt uz MSAL, kurā ir jaunākie līdzekļi un drošības atjauninājumi.</span><span class="sxs-lookup"><span data-stu-id="b9af1-119">We recommend updating to the MSAL, which has the latest features and security updates.</span></span>
- <span data-ttu-id="b9af1-120">Ja izmantojat Microsoft apps, zināt, ka korporācija Microsoft turpina migrēt savas lietojumprogrammas uz MSAL pēc atbalsta termiņa beigām, nodrošinot, ka tās gūs labumu no MSAL pastāvīgajiem drošības un līdzekļu uzlabojumiem.</span><span class="sxs-lookup"><span data-stu-id="b9af1-120">If you're using Microsoft apps, know that Microsoft is in the process of migrating its apps to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="b9af1-121">[Lasiet bieži uzdotos jautājumus par ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="b9af1-121">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
2. <span data-ttu-id="b9af1-122">[Uzziniet, kā migrēt programmas katrā platformā](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).</span><span class="sxs-lookup"><span data-stu-id="b9af1-122">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).</span></span>
3. <span data-ttu-id="b9af1-123">Ja pēc ceļveža izlasīšanas lietojumprogrammas platformā jums ir papildu jautājumi, varat publicēt [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) ar atzīmi [Azure-AD-ADAL-deprecat] vai atvērt problēmu bibliotēkas GitHub repozitorijā.</span><span class="sxs-lookup"><span data-stu-id="b9af1-123">If, after reading the guide for your app's platform, you have additional questions, you can post on [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) with the tag [azure-ad-adal-deprecation] or open an issue in library's GitHub repository.</span></span> <span data-ttu-id="b9af1-124">**MSAL pārskata** raksta sadaļā [valodas un struktūras](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) skatiet saites uz katras bibliotēkas repo.</span><span class="sxs-lookup"><span data-stu-id="b9af1-124">See the [Languages and frameworks](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) section of the **MSAL overview** article for links to each library's repo.</span></span>
4. <span data-ttu-id="b9af1-125">**Ja jums ir nepieciešama palīdzība, lai izprastu, kuras jūsu lietojumprogrammas izmanto ADAL**, iesakām pārskatīt visu programmas avota kodu.</span><span class="sxs-lookup"><span data-stu-id="b9af1-125">**If you need help understanding which of your apps use ADAL**, we recommend you review all of your apps' source code.</span></span> <span data-ttu-id="b9af1-126">Ja nepieciešams, sazinieties ar visiem neatkarīgiem programmatūras piegādātājiem (ISV) vai lietojumprogrammu nodrošinātājiem.</span><span class="sxs-lookup"><span data-stu-id="b9af1-126">If applicable, reach out to any Independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="b9af1-127">Microsoft atbalsta dienests var jums sniegt sarakstu ar visām jūsu nomniekā esošajām lietojumprogrammām, kas nav Microsoft ADAL lietojumprogrammas.</span><span class="sxs-lookup"><span data-stu-id="b9af1-127">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>







