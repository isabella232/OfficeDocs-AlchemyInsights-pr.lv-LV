---
title: Problēmas, kas izstrādā lietojumprogrammas ar API
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974622"
---
# <a name="issues-developing-applications-with-apis"></a><span data-ttu-id="19c61-102">Problēmas, kas izstrādā lietojumprogrammas ar API</span><span class="sxs-lookup"><span data-stu-id="19c61-102">Issues developing applications with APIs</span></span>

<span data-ttu-id="19c61-103">Lai sāktu izmantot Azure Active Directory Graph API, skatiet [AZURE ad GRAPH API Quickstart Guide](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) vai skatiet [interaktīvo AZURE ad Graph API atsauces dokumentāciju](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span><span class="sxs-lookup"><span data-stu-id="19c61-103">To begin using the Azure Active Directory Graph API, see the [Azure AD Graph API quickstart guide](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , or view the [interactive Azure AD Graph API reference documentation](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span></span>

<span data-ttu-id="19c61-104">**Azure Active Directory autentifikācijas bibliotēkas (ADAL) un Azure AD Graph API (AAD Graph) atbalsta beigas**</span><span class="sxs-lookup"><span data-stu-id="19c61-104">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="19c61-105">**Sākot no 30. jūnija, 2020**, vairs nepievienosit nekādus jaunus līdzekļus, kas ADAL un Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="19c61-105">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="19c61-106">Mēs turpināsim nodrošināt tehnisko atbalstu un drošības atjauninājumus, taču vairs nenodrošinās līdzekļu atjauninājumus.</span><span class="sxs-lookup"><span data-stu-id="19c61-106">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="19c61-107">**Sākot no 30. jūnija, 2022**, mēs NODROŠINĀSIM atbalstu ADAL un Azure AD Graph un vairs nenodrošinās tehnisko atbalstu vai drošības atjauninājumus.</span><span class="sxs-lookup"><span data-stu-id="19c61-107">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="19c61-108">Programmas, kas, izmantojot ADAL, pēc šī laika turpinās darboties, bet nesaņem nekādu tehnisku atbalstu vai drošības atjauninājumus.</span><span class="sxs-lookup"><span data-stu-id="19c61-108">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

<span data-ttu-id="19c61-109">Lietojumprogrammas, kas izmanto Azure AD Graph pēc šī laika, iespējams, vairs nesaņems atbildes no Azure AD Graph galapunkta.</span><span class="sxs-lookup"><span data-stu-id="19c61-109">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="19c61-110">**PārADAL migrācija**</span><span class="sxs-lookup"><span data-stu-id="19c61-110">**ADAL Migration**</span></span>

<span data-ttu-id="19c61-111">Ieteicams atjaunināt [Microsoft autentifikācijas bibliotēkā (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), kurā ir jaunākie līdzekļi un drošības atjauninājumi.</span><span class="sxs-lookup"><span data-stu-id="19c61-111">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="19c61-112">Ja izmantojat Microsoft programmas, zināt, ka korporācija Microsoft pašlaik veic savas lietojumprogrammas migrāciju uz MSAL, izmantojot atbalsta termiņu, nodrošinot, ka tās gūs labumu no MSAL pastāvīgajiem drošības un līdzekļu uzlabojumiem.</span><span class="sxs-lookup"><span data-stu-id="19c61-112">If you're using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="19c61-113">[Lasiet bieži uzdotos jautājumus par ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="19c61-113">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="19c61-114">[Uzziniet, kā migrēt programmas katrā platformā](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="19c61-114">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="19c61-115">Ja jums ir nepieciešama palīdzība, lai izprastu, kura lietojumprogramma izmanto ADAL, iesakām pārskatīt visu savu programmu avota kodu un pēc vajadzības sazināties ar citiem ISV vai lietojumprogrammu nodrošinātājiem.</span><span class="sxs-lookup"><span data-stu-id="19c61-115">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="19c61-116">Microsoft atbalsts var arī nodrošināt, ka jūsu nomniekā ir saraksts ar visām programmām, kas nav Microsoft ADAL.</span><span class="sxs-lookup"><span data-stu-id="19c61-116">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="19c61-117">**AAD Graph migrācija**</span><span class="sxs-lookup"><span data-stu-id="19c61-117">**AAD Graph Migration**</span></span>

<span data-ttu-id="19c61-118">Lietojumprogrammas, kas izmanto Azure AD Graph, izpildiet mūsu norādījumus, lai migrētu [AZURE ad Graph programmas uz Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="19c61-118">For applications that are using Azure AD Graph, follow our guidance to migrate [Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span></span>

1. <span data-ttu-id="19c61-119">[Mūsu migrācijas kontrolsaraksts nodrošina darba sākšanas punktu](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="19c61-119">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
1. <span data-ttu-id="19c61-120">Jūsu Azure lietojumprogrammu reģistrācijas portālā ir parādīts, kuras lietojumprogrammas izmanto AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="19c61-120">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="19c61-121">Iesakām pārskatīt visu savu lietojumprogrammu avota kodu un, ja nepieciešams, sazināties ar citiem ISV vai lietojumprogrammu nodrošinātājiem.</span><span class="sxs-lookup"><span data-stu-id="19c61-121">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="19c61-122">Microsoft atbalsts var arī nodrošināt, lai jūsu nomniekā tiktu parādīts visu AAD Graph izmantošanas saraksts.</span><span class="sxs-lookup"><span data-stu-id="19c61-122">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
1. <span data-ttu-id="19c61-123">Lai jūsu programmai piekļūtu datiem programmā Microsoft Graph, lietotājam vai administratoram tā ir jāpiešķir pareizas atļaujas, izmantojot piekrišanas procesu.</span><span class="sxs-lookup"><span data-stu-id="19c61-123">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="19c61-124">[Microsoft Graph atļauju atsaucēs](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) ir uzskaitītas atļaujas, kas ir saistītas ar katru galveno Microsoft Graph API kopu.</span><span class="sxs-lookup"><span data-stu-id="19c61-124">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="19c61-125">Tajā sniegti arī norādījumi par to, kā izmantot atļaujas.</span><span class="sxs-lookup"><span data-stu-id="19c61-125">It also provides guidance about how to use the permissions.</span></span>
