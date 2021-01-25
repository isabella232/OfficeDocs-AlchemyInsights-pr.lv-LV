---
title: Problēmas, izstrādājot lietojumprogrammas
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974471"
---
# <a name="issues-developing-applications"></a><span data-ttu-id="2852b-102">Problēmas, izstrādājot lietojumprogrammas</span><span class="sxs-lookup"><span data-stu-id="2852b-102">Issues developing applications</span></span>

<span data-ttu-id="2852b-103">Lai novērstu izplatītākās problēmas, būvējot Azure Active Directory (AD) lietojumprogrammas, skatiet šos rakstus:</span><span class="sxs-lookup"><span data-stu-id="2852b-103">To troubleshoot the most common problems when building Azure Active Directory (AD) apps, see the following articles:</span></span>

- [<span data-ttu-id="2852b-104">Man ir problēmas ar pierakstīšanos lietojumprogrammā (-ām), izmantojot tikai Chrome pārlūkprogrammu</span><span class="sxs-lookup"><span data-stu-id="2852b-104">I am seeing trouble signing in to application(s) using Chrome browser only</span></span>](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [<span data-ttu-id="2852b-105">Es nezinu, kā mainīt marķierierīces ilguma noklusējumus manā lietojumprogrammā</span><span class="sxs-lookup"><span data-stu-id="2852b-105">I don't know how to change the token lifetime defaults for my application</span></span>](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [<span data-ttu-id="2852b-106">Esmu apjucis, kā darbojas lietojumprogrammu piekrišana</span><span class="sxs-lookup"><span data-stu-id="2852b-106">I am confused about how application consent works</span></span>](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [<span data-ttu-id="2852b-107">Es nezinu, kā piešķirt atļaujas manai lietojumprogrammai</span><span class="sxs-lookup"><span data-stu-id="2852b-107">I don't know how to grant permissions to my application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [<span data-ttu-id="2852b-108">Nesaprotu atšķirību starp deleģētajām un lietojumprogrammas atļaujām</span><span class="sxs-lookup"><span data-stu-id="2852b-108">I don't understand the difference between delegated and application permissions</span></span>](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

<span data-ttu-id="2852b-109">\***Azure Active Directory autentifikācijas bibliotēkas (ADAL) un AZURE ad GRAPH API (AAD Graph) atbalsta beigas**</span><span class="sxs-lookup"><span data-stu-id="2852b-109">\***End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)** _</span></span>

- <span data-ttu-id="2852b-110">Sākot no 30. jūnija, 2020 vairs nepievienosit jaunus līdzekļus Azure Active Directory autentifikācijas bibliotēkai (ADAL) un Azure AD Graph API (AAD Graph).</span><span class="sxs-lookup"><span data-stu-id="2852b-110">Starting June 30th, 2020, we will no longer add any new features to Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph).</span></span> <span data-ttu-id="2852b-111">Mēs turpināsim nodrošināt tehnisko atbalstu un drošības atjauninājumus, taču vairs nenodrošinās līdzekļu atjauninājumus.</span><span class="sxs-lookup"><span data-stu-id="2852b-111">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

- <span data-ttu-id="2852b-112">Sākot no 30. jūnija, 2022, mēs nodrošināsim atbalstu ADAL un AAD Graph un vairs nenodrošinās tehnisko atbalstu vai drošības atjauninājumus.</span><span class="sxs-lookup"><span data-stu-id="2852b-112">Starting June 30th, 2022, we will end support for ADAL and AAD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="2852b-113">Šī nosacījuma rezultātā ietekmēs tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="2852b-113">As a result of this condition, the following are the implications:</span></span>

    - <span data-ttu-id="2852b-114">Programmas, kas, izmantojot ADAL, pēc šī laika turpinās darboties, bet nesaņem nekādu tehnisku atbalstu vai drošības atjauninājumus.</span><span class="sxs-lookup"><span data-stu-id="2852b-114">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

    - <span data-ttu-id="2852b-115">Lietojumprogrammas, kas izmanto AAD Graph pēc šī laika, var vairs nesaņemt atbildes no AAD Graph galapunkta</span><span class="sxs-lookup"><span data-stu-id="2852b-115">Apps using AAD Graph after this time may no longer receive responses from the AAD Graph endpoint</span></span>

<span data-ttu-id="2852b-116">*PārADAL migrācija*\*</span><span class="sxs-lookup"><span data-stu-id="2852b-116">_ *ADAL Migration*\*</span></span>

<span data-ttu-id="2852b-117">Ja izmantojat Microsoft apps, iesakām atjaunināt Microsoft autentifikācijas bibliotēkā (MSAL), kurā ir jaunākie līdzekļi un drošības atjauninājumi.</span><span class="sxs-lookup"><span data-stu-id="2852b-117">If you're using Microsoft apps, we recommend updating to the Microsoft Authentication Library (MSAL), which has the latest features and security updates.</span></span> <span data-ttu-id="2852b-118">Šis ieteikums ir paredzēts korporācijai Microsoft, kas uzsāk procesu, lai migrētu tās lietojumprogrammas uz MSAL pēc atbalsta termiņa beigām.</span><span class="sxs-lookup"><span data-stu-id="2852b-118">This recommendation is in the context of Microsoft initiating the process of migrating its apps to MSAL by the end-of-support deadline.</span></span> 

<span data-ttu-id="2852b-119">Migrēšana, ko korporācija Microsoft ir MSAL, nodrošina, ka lietojumprogrammas izmanto MSAL drošības un līdzekļu uzlabojumus.</span><span class="sxs-lookup"><span data-stu-id="2852b-119">The migration by Microsoft of its apps to MSAL ensures that the apps benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="2852b-120">ADAL bieži uzdoto jautājumu lasīšana</span><span class="sxs-lookup"><span data-stu-id="2852b-120">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [<span data-ttu-id="2852b-121">Uzziniet, kā migrēt programmas katrā platformā</span><span class="sxs-lookup"><span data-stu-id="2852b-121">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. <span data-ttu-id="2852b-122">Ja jums ir nepieciešama palīdzība, lai izprastu, kuras jūsu lietojumprogrammas izmanto ADAL, iesakām pārskatīt visu savu programmu avota kodu un, ja nepieciešams, sazināties ar visiem neatkarīgiem programmatūras piegādātājiem (ISV) vai lietojumprogrammu nodrošinātājiem.</span><span class="sxs-lookup"><span data-stu-id="2852b-122">If you need help in understanding which of your apps use ADAL, we recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="2852b-123">Microsoft atbalsts var arī nodrošināt, ka jūsu nomniekā ir saraksts ar visām programmām, kas nav Microsoft ADAL.</span><span class="sxs-lookup"><span data-stu-id="2852b-123">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="2852b-124">**AAD Graph migrācija**</span><span class="sxs-lookup"><span data-stu-id="2852b-124">**AAD Graph Migration**</span></span>

<span data-ttu-id="2852b-125">Attiecībā uz lietojumprogrammām, kas izmanto AAD Graph, izpildiet mūsu norādījumus par to, kā migrēt AAD Graph programmas uz Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="2852b-125">For applications that are using AAD Graph, follow our guidance to migrate AAD Graph apps to Microsoft Graph:</span></span>

1. <span data-ttu-id="2852b-126">[Mūsu migrācijas kontrolsaraksts nodrošina darba sākšanas punktu](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="2852b-126">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
2. <span data-ttu-id="2852b-127">Jūsu Azure lietojumprogrammu reģistrācijas portālā ir parādīts, kuras lietojumprogrammas izmanto AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="2852b-127">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="2852b-128">Iesakām pārskatīt visu savu lietojumprogrammu avota kodu un, ja nepieciešams, sazināties ar visiem neatkarīgiem programmatūras piegādātājiem (ISV) vai lietojumprogrammu nodrošinātājiem.</span><span class="sxs-lookup"><span data-stu-id="2852b-128">We recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="2852b-129">Microsoft atbalsts var arī sniegt informāciju par AAD Graph lietošanu nomniekā.</span><span class="sxs-lookup"><span data-stu-id="2852b-129">Microsoft support can also provide you information on AAD Graph usage in your tenant.</span></span>







