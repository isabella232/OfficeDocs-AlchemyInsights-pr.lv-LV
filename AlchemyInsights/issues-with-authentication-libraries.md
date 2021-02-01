---
title: Problēmas ar autentifikācijas bibliotēkām
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004333"
- "7731"
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063637"
---
# <a name="issues-with-authentication-libraries"></a><span data-ttu-id="bf313-102">Problēmas ar autentifikācijas bibliotēkām</span><span class="sxs-lookup"><span data-stu-id="bf313-102">Issues with Authentication Libraries</span></span>

1. <span data-ttu-id="bf313-103">[Microsoft identitātes platformas autentifikācijas bibliotēkas](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) norāda Microsoft atbalstītās un saderīgās klienta un starpprogrammatūras bibliotēkas.</span><span class="sxs-lookup"><span data-stu-id="bf313-103">[Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) lists Microsoft-supported and compatible client and middleware libraries.</span></span>
2. <span data-ttu-id="bf313-104">Microsoft autentifikācijas bibliotēka (MSAL) atbalsta vairākas [autentifikācijas plūsmas](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) , kas jāizmanto dažādos lietojumprogrammas scenārijos.</span><span class="sxs-lookup"><span data-stu-id="bf313-104">The Microsoft Authentication Library (MSAL) supports several [authentication flows](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) for use in different application scenarios.</span></span>
3. <span data-ttu-id="bf313-105">Lai autentificētu un iegūtu marķierierīces, kodā inicializējiet jaunu publisku vai konfidenciālu klienta lietojumprogrammu.</span><span class="sxs-lookup"><span data-stu-id="bf313-105">To authenticate and acquire tokens, you initialize a new public or confidential client application in your code.</span></span> <span data-ttu-id="bf313-106">Varat iestatīt vairākas konfigurācijas opcijas, ja inicializējat klienta programmu Microsoft autentifikācijas bibliotēkā (MSAL).</span><span class="sxs-lookup"><span data-stu-id="bf313-106">You can set several configuration options when you initialize the client app in the Microsoft Authentication Library (MSAL).</span></span> <span data-ttu-id="bf313-107">Lai uzzinātu vairāk, skatiet sadaļu [lietojumprogrammas konfigurācijas opcijas](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span><span class="sxs-lookup"><span data-stu-id="bf313-107">To learn more, see [Application configuration options](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span></span>

<span data-ttu-id="bf313-108">**Azure Active Directory autentifikācijas bibliotēkas (ADAL) un Azure AD Graph API (AAD Graph) atbalsta beigas**</span><span class="sxs-lookup"><span data-stu-id="bf313-108">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="bf313-109">**Sākot no 30. jūnija, 2020**, vairs nepievienosit nekādus jaunus līdzekļus, kas ADAL un Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="bf313-109">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="bf313-110">Mēs turpināsim nodrošināt tehnisko atbalstu un drošības atjauninājumus, bet vairs nenodrošināsim līdzekļu atjauninājumus.</span><span class="sxs-lookup"><span data-stu-id="bf313-110">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="bf313-111">**Sākot no 30. jūnija, 2022**, mēs NODROŠINĀSIM atbalstu ADAL un Azure AD Graph un vairs nenodrošinās tehnisko atbalstu vai drošības atjauninājumus.</span><span class="sxs-lookup"><span data-stu-id="bf313-111">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="bf313-112">Programmas, kas, izmantojot ADAL, pēc šī laika turpinās darboties, bet *nesaņem nekādu tehnisku atbalstu vai drošības atjauninājumus*.</span><span class="sxs-lookup"><span data-stu-id="bf313-112">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="bf313-113">Lietojumprogrammas, kas izmanto Azure AD Graph pēc šī laika, iespējams, vairs nesaņems atbildes no Azure AD Graph galapunkta.</span><span class="sxs-lookup"><span data-stu-id="bf313-113">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="bf313-114">**PārADAL migrācija**</span><span class="sxs-lookup"><span data-stu-id="bf313-114">**ADAL Migration**</span></span>

<span data-ttu-id="bf313-115">Iesakām veikt atjaunināšanu uz [Microsoft autentifikācijas bibliotēku (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), kurā ir jaunākie līdzekļi un drošības atjauninājumi.</span><span class="sxs-lookup"><span data-stu-id="bf313-115">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="bf313-116">Ja izmantojat Microsoft programmas, zināt, ka korporācija Microsoft pašlaik veic savu lietojumprogrammu migrēšanu uz MSAL, izmantojot atbalsta termiņu, lai nodrošinātu, ka tās gūs labumu no MSAL pašreizējiem drošības un līdzekļu uzlabojumiem.</span><span class="sxs-lookup"><span data-stu-id="bf313-116">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they will benefit from MSAL's ongoing security and feature improvements.</span></span>

<span data-ttu-id="bf313-117">Papildinformāciju skatiet šeit:</span><span class="sxs-lookup"><span data-stu-id="bf313-117">For more information, see:</span></span>

1. [<span data-ttu-id="bf313-118">Lasīt bieži uzdotos jautājumus par ADAL</span><span class="sxs-lookup"><span data-stu-id="bf313-118">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="bf313-119">Uzziniet, kā migrēt lietojumprogrammas katrā platformā</span><span class="sxs-lookup"><span data-stu-id="bf313-119">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="bf313-120">Ja jums ir nepieciešama palīdzība, lai izprastu, kura lietojumprogramma izmanto ADAL, iesakām pārskatīt visu savu programmu avota kodu un pēc vajadzības sazināties ar citiem ISV vai lietojumprogrammu nodrošinātājiem.</span><span class="sxs-lookup"><span data-stu-id="bf313-120">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="bf313-121">Microsoft atbalsta dienests var jums sniegt sarakstu ar visām jūsu nomniekā esošajām lietojumprogrammām, kas nav Microsoft ADAL lietojumprogrammas.</span><span class="sxs-lookup"><span data-stu-id="bf313-121">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="bf313-122">**AAD Graph migrācija**</span><span class="sxs-lookup"><span data-stu-id="bf313-122">**AAD Graph Migration**</span></span>

<span data-ttu-id="bf313-123">Lietojumprogrammas, kas izmanto Azure AD Graph, izpildiet mūsu norādījumus, lai [migrētu AZURE ad Graph programmas uz Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span><span class="sxs-lookup"><span data-stu-id="bf313-123">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. [<span data-ttu-id="bf313-124">Mūsu migrācijas kontrolsaraksts nodrošina darba sākšanas punktu.</span><span class="sxs-lookup"><span data-stu-id="bf313-124">Our migration checklist provides a getting started point.</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. <span data-ttu-id="bf313-125">Azure lietojumprogrammu reģistrācijas portālā tiek rādīts, kuras lietojumprogrammas izmanto AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="bf313-125">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="bf313-126">Iesakām pārskatīt visu jūsu lietojumprogrammu pirmkodu un, ja nepieciešams, sazināties ar jebkuru ISV vai lietojumprogrammu nodrošinātāju.</span><span class="sxs-lookup"><span data-stu-id="bf313-126">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="bf313-127">Microsoft atbalsts var arī nodrošināt, lai jūsu nomniekā tiktu parādīts visu AAD Graph izmantošanas saraksts.</span><span class="sxs-lookup"><span data-stu-id="bf313-127">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="bf313-128">Lai jūsu programmai piekļūtu datiem programmā Microsoft Graph, lietotājam vai administratoram tā ir jāpiešķir pareizas atļaujas, izmantojot piekrišanas procesu.</span><span class="sxs-lookup"><span data-stu-id="bf313-128">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="bf313-129">[Microsoft Graph atļauju atsaucēs](https://docs.microsoft.com/graph/permissions-reference) ir uzskaitītas atļaujas, kas ir saistītas ar katru galveno Microsoft Graph API kopu.</span><span class="sxs-lookup"><span data-stu-id="bf313-129">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="bf313-130">Tajā sniegti arī norādījumi par to, kā izmantot atļaujas.</span><span class="sxs-lookup"><span data-stu-id="bf313-130">It also provides guidance about how to use the permissions.</span></span>
