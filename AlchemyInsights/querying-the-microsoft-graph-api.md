---
title: Microsoft Graph API vaicājumu
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
- "9004345"
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974422"
---
# <a name="querying-the-microsoft-graph-api"></a><span data-ttu-id="1c4a1-102">Microsoft Graph API vaicājumu</span><span class="sxs-lookup"><span data-stu-id="1c4a1-102">Querying the Microsoft Graph API</span></span>

<span data-ttu-id="1c4a1-103">Šī tēma var attiekties arī uz izstrādātājiem, kuri joprojām izmanto Azure AD Graph API.</span><span class="sxs-lookup"><span data-stu-id="1c4a1-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="1c4a1-104">Tomēr ir **stingri** ieteicams izmantot programmu Microsoft Graph visiem jūsu direktorija, identitātes un piekļuves pārvaldības scenārijiem.</span><span class="sxs-lookup"><span data-stu-id="1c4a1-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="1c4a1-105">**Autentifikācijas vai autorizācijas problēmas**</span><span class="sxs-lookup"><span data-stu-id="1c4a1-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="1c4a1-106">Ja jūsu lietojumprogramma **nevar iegūt pilnvaras** , lai sasauktu Microsoft Graph, izvēlieties problēmu, kas rodas, **iegūstot piekļuves marķiera (autentifikāciju)** Microsoft Graph kategoriju, lai saņemtu konkrētāku palīdzību un atbalstu šajā tēmā.</span><span class="sxs-lookup"><span data-stu-id="1c4a1-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="1c4a1-107">Ja jūsu programma **saņem 401 vai 403 autorizācijas kļūdas** , zvanot uz Microsoft Graph, izvēlieties, vai Microsoft Graph API kategorijā iegūt **Access denied kļūdu (autorizācija)** .</span><span class="sxs-lookup"><span data-stu-id="1c4a1-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="1c4a1-108">**Es vēlos izmantot programmu Microsoft Graph, taču neesat pārliecināts, kur sākt**</span><span class="sxs-lookup"><span data-stu-id="1c4a1-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

<span data-ttu-id="1c4a1-109">Lai uzzinātu vairāk par Microsoft Graph, skatiet:</span><span class="sxs-lookup"><span data-stu-id="1c4a1-109">To learn more about Microsoft Graph, see:</span></span>

- [<span data-ttu-id="1c4a1-110">Pārskats par Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1c4a1-110">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="1c4a1-111">Pārskats par identitāti un piekļuves pārvaldību programmā Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1c4a1-111">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="1c4a1-112">Darba sākšana Microsoft Graph programmu izveidē</span><span class="sxs-lookup"><span data-stu-id="1c4a1-112">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="1c4a1-113">**Microsoft Graph Explorer** — testējiet Microsoft Graph API nomniekā vai demonstrācijas nomniekā</span><span class="sxs-lookup"><span data-stu-id="1c4a1-113">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="1c4a1-114">**Es vēlos izmantot Microsoft Graph, bet vai tas atbalsta v 1.0 direktorija API, kas man ir nepieciešams?**</span><span class="sxs-lookup"><span data-stu-id="1c4a1-114">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="1c4a1-115">Microsoft Graph ir ieteicamais API direktorijam, identitātei un piekļuves pārvaldībai.</span><span class="sxs-lookup"><span data-stu-id="1c4a1-115">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="1c4a1-116">Tomēr ir vēl dažas atšķirības starp to, kas ir iespējams Azure AD Graph un Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1c4a1-116">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="1c4a1-117">Pārskatiet tālāk norādītos rakstus, kas izceļ visaktuālākās atšķirības, lai palīdzētu jums izvēlēties:</span><span class="sxs-lookup"><span data-stu-id="1c4a1-117">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="1c4a1-118">Resursu tipa atšķirības starp Azure AD Graph un Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1c4a1-118">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="1c4a1-119">Rekvizītu atšķirības starp Azure AD Graph un Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1c4a1-119">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="1c4a1-120">Metodes atšķirības starp Azure AD un Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1c4a1-120">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="1c4a1-121">**Veicot vaicājumu *lietotāja* objektam, trūkst daudz tā rekvizītu**</span><span class="sxs-lookup"><span data-stu-id="1c4a1-121">**When I query the *user* object, many of its properties are missing**</span></span>

<span data-ttu-id="1c4a1-122">`GET https://graph.microsoft.com/v1.0/users` atgriež tikai 11 rekvizītus, jo Microsoft Graph automātiski atlasa noklusējuma *lietotāju* rekvizītu kopu, kas jāatgriež.</span><span class="sxs-lookup"><span data-stu-id="1c4a1-122">`GET https://graph.microsoft.com/v1.0/users` only returns 11 properties, as Microsoft Graph auto-selects a default set of *user* properties to return.</span></span> <span data-ttu-id="1c4a1-123">Ja ir nepieciešami citi *lietotāja* rekvizīti, izmantojiet $SELECT, lai izvēlētos lietojumprogrammas rekvizītus.</span><span class="sxs-lookup"><span data-stu-id="1c4a1-123">If you need other *user* properties, use $select to pick the properties your application needs.</span></span> <span data-ttu-id="1c4a1-124">Vispirms izmēģiniet to programmā **Microsoft Graph Explorer** .</span><span class="sxs-lookup"><span data-stu-id="1c4a1-124">Try it out in **Microsoft Graph Explorer** first.</span></span>

<span data-ttu-id="1c4a1-125">**Dažas lietotāja rekvizīta vērtības ir *Null* , kaut gan es zinu, ka tās ir iestatītas**</span><span class="sxs-lookup"><span data-stu-id="1c4a1-125">**Some user property values are *null* even though I know they are set**</span></span>

<span data-ttu-id="1c4a1-126">Visticamākais skaidrojums ir tāds, ka lietojumprogrammai ir piešķirts *lietotājs. ReadBasic. All* permissions.</span><span class="sxs-lookup"><span data-stu-id="1c4a1-126">The most likely explanation is that the application had been granted the *User.ReadBasic.All* permission.</span></span> <span data-ttu-id="1c4a1-127">Tas ļauj lietojumprogrammai lasīt ierobežotu lietotāja rekvizītu kopu, atgriežot visus pārējos rekvizītus kā Null pat tad, ja tie ir iepriekš iestatīti.</span><span class="sxs-lookup"><span data-stu-id="1c4a1-127">This allows the application to read a limited set of user properties, returning all other properties as null even if they have been previously set.</span></span> <span data-ttu-id="1c4a1-128">Mēģiniet piešķirt lietojumprogrammas *lietotāju. Read. All* Permission tā vietā.</span><span class="sxs-lookup"><span data-stu-id="1c4a1-128">Try granting the application *User.Read.All* permission instead.</span></span>

<span data-ttu-id="1c4a1-129">Lai iegūtu papildinformāciju, skatiet rakstu [Microsoft Graph lietotāju atļaujas](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span><span class="sxs-lookup"><span data-stu-id="1c4a1-129">For more information, see [Microsoft Graph user permissions](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span></span>

<span data-ttu-id="1c4a1-130">**Man rodas problēmas, izmantojot OData vaicājuma parametrus, lai filtrētu datus manos pieprasījumos**</span><span class="sxs-lookup"><span data-stu-id="1c4a1-130">**I'm having trouble using OData query parameters to filter data in my requests**</span></span>

<span data-ttu-id="1c4a1-131">Kamēr Microsoft Graph atbalsta plašu OData vaicājuma parametru diapazonu, daudzus no šiem parametriem pilnībā neatbalsta direktoriju pakalpojumi (resursi, kas pārmanto no *directoryObject*) programmā Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1c4a1-131">While Microsoft Graph supports a wide range of the OData query parameters, many of those parameters are not fully supported by directory services (resources that inherit from *directoryObject*) in Microsoft Graph.</span></span> <span data-ttu-id="1c4a1-132">Tie paši ierobežojumi, kas bija atrodami Azure AD Graph programmā Microsoft Graph, joprojām ir iespējami lielākoties:</span><span class="sxs-lookup"><span data-stu-id="1c4a1-132">The same limitations that were present in Azure AD Graph persist for the most part in Microsoft Graph:</span></span>

1. <span data-ttu-id="1c4a1-133">**Netiek atbalstīts**: $count, $search un $Filter vērtību *Null* vai *Not Null*</span><span class="sxs-lookup"><span data-stu-id="1c4a1-133">**Not supported**: $count, $search, and $filter on *null* or *not null* values</span></span>
2. <span data-ttu-id="1c4a1-134">**Netiek atbalstīts**: $Filter noteiktos rekvizītos (skatīt resursu tēmas, kuru rekvizītus var filtrēt)</span><span class="sxs-lookup"><span data-stu-id="1c4a1-134">**Not supported**: $filter on certain properties (see resource topics on which properties are filterable)</span></span>
3. <span data-ttu-id="1c4a1-135">**Netiek atbalstīts**: lapošana, filtrēšana un kārtošana vienlaikus</span><span class="sxs-lookup"><span data-stu-id="1c4a1-135">**Not supported**: paging, filtering, and sorting at the same time</span></span>
4. <span data-ttu-id="1c4a1-136">**Netiek atbalstīts**: relācijas filtrēšana.</span><span class="sxs-lookup"><span data-stu-id="1c4a1-136">**Not supported**: filtering on a relationship.</span></span> <span data-ttu-id="1c4a1-137">Piemēram, atrodiet visus tās tehniskās grupas dalībniekus, kas ir Apvienotajā Karalistē.</span><span class="sxs-lookup"><span data-stu-id="1c4a1-137">For example - find all members of the engineering group that are in the UK.</span></span>
5. <span data-ttu-id="1c4a1-138">**Daļējs atbalsts**: $orderby *lietotājam* (tikai displayName un userPrincipalName) un *grupu*</span><span class="sxs-lookup"><span data-stu-id="1c4a1-138">**Partial support**: $orderby on *user* (displayName and userPrincipalName only) and *group*</span></span>
6. <span data-ttu-id="1c4a1-139">**Daļējs atbalsts**: $Filter (atbalsta tikai *EQ*, startswith *,* *kā arī* *un ierobežots)* atbalstu, $Expand (viena objekta relāciju izvēršana atgriež visas relācijas, taču objektu kopuma paplašināšana ir ierobežota) </span><span class="sxs-lookup"><span data-stu-id="1c4a1-139">**Partial support**: $filter (supports only *eq*, *startswith*, *or*, *and*, and limited *any*) support, $expand (expanding a single object's relationships returns all relationships, but expanding a collection of objects' relationships is limited)</span></span>

<span data-ttu-id="1c4a1-140">Lai iegūtu papildinformāciju, skatiet rakstu [atbilžu pielāgošana ar vaicājuma parametriem](https://docs.microsoft.com/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1c4a1-140">For more information, see [Customize responses with query parameters](https://docs.microsoft.com/graph/query-parameters).</span></span>

<span data-ttu-id="1c4a1-141">**API, ko es saukšu, nedarbojas — kur varu veikt papildu testēšanu?**</span><span class="sxs-lookup"><span data-stu-id="1c4a1-141">**The API I'm calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="1c4a1-142">**Microsoft Graph Explorer** — testējiet Microsoft Graph API savā nomniekā vai demonstrācijas nomniekā, kā arī skatiet **vaicājumu piemērus** programmā Microsoft Graph Explorer.</span><span class="sxs-lookup"><span data-stu-id="1c4a1-142">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="1c4a1-143">**Veicot vaicājumu, lai iegūtu datus, šķiet, ka tiek atgriezta nepilnīga datu kopa**</span><span class="sxs-lookup"><span data-stu-id="1c4a1-143">**When I query for data it seems like I get an incomplete data set back**</span></span>

<span data-ttu-id="1c4a1-144">Ja veicat vaicājumu par kolekciju (piemēram, *lietotāji*), Microsoft Graph izmanto servera puses lappušu ierobežojumus, tāpēc rezultāti vienmēr tiek atgriezti, izmantojot noklusējuma lappuses izmērus.</span><span class="sxs-lookup"><span data-stu-id="1c4a1-144">If you are querying a collection (like *users*), Microsoft Graph uses server-side page limits so results are always returned with a default page-size.</span></span> <span data-ttu-id="1c4a1-145">Jūsu programmai vienmēr būtu jāgaida no pakalpojuma atdots kolekcijas.</span><span class="sxs-lookup"><span data-stu-id="1c4a1-145">Your app should always expect to page through collections returned from the service.</span></span>

<span data-ttu-id="1c4a1-146">Papildinformāciju skatiet rakstā:</span><span class="sxs-lookup"><span data-stu-id="1c4a1-146">For more information, see:</span></span>

- [<span data-ttu-id="1c4a1-147">Microsoft Graph paraugprakse</span><span class="sxs-lookup"><span data-stu-id="1c4a1-147">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="1c4a1-148">Microsoft Graph datu lapošana jūsu lietojumprogrammā</span><span class="sxs-lookup"><span data-stu-id="1c4a1-148">Paging Microsoft Graph data in your app</span></span>](https://docs.microsoft.com/graph/paging)

<span data-ttu-id="1c4a1-149">**Mana programma ir pārāk lēna, un tiek arī panākta ierobežošana. Kādus uzlabojumus varu veikt?**</span><span class="sxs-lookup"><span data-stu-id="1c4a1-149">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="1c4a1-150">Atkarībā no tā jūsu rīcībā ir dažādi varianti, kā jūsu lietojumprogrammā veikt papildu darbības, un dažos gadījumos mazāk noslieces uz darbu, izmantojot pakalpojumu (kad veicat pārāk daudz zvanu).</span><span class="sxs-lookup"><span data-stu-id="1c4a1-150">Depending on your scenario, there are a variety of different options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

<span data-ttu-id="1c4a1-151">Lai uzzinātu vairāk, skatiet:</span><span class="sxs-lookup"><span data-stu-id="1c4a1-151">To learn more, see:</span></span>

- [<span data-ttu-id="1c4a1-152">Microsoft Graph paraugprakse</span><span class="sxs-lookup"><span data-stu-id="1c4a1-152">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="1c4a1-153">Pakešapstrādes pieprasījumi</span><span class="sxs-lookup"><span data-stu-id="1c4a1-153">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="1c4a1-154">Izmaiņu reģistrēšana, izmantojot Delta vaicājumu</span><span class="sxs-lookup"><span data-stu-id="1c4a1-154">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="1c4a1-155">Saņemiet paziņojumus par izmaiņām, izmantojot āķus</span><span class="sxs-lookup"><span data-stu-id="1c4a1-155">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="1c4a1-156">Ierobežošanas norādījumi</span><span class="sxs-lookup"><span data-stu-id="1c4a1-156">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="1c4a1-157">**Kur var iegūt papildinformāciju par kļūdām un zināmajām problēmām?**</span><span class="sxs-lookup"><span data-stu-id="1c4a1-157">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="1c4a1-158">Microsoft Graph kļūdas atbilžu informācija</span><span class="sxs-lookup"><span data-stu-id="1c4a1-158">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="1c4a1-159">Zināmās problēmas ar Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1c4a1-159">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="1c4a1-160">**Kur varu pārbaudīt pakalpojumu pieejamības un savienojamības statusu?**</span><span class="sxs-lookup"><span data-stu-id="1c4a1-160">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="1c4a1-161">Pamata pakalpojumu pieejamība un savienojamība, kam var piekļūt, izmantojot Microsoft Graph, var ietekmēt Microsoft Graph vispārējo pieejamību un veiktspēju.</span><span class="sxs-lookup"><span data-stu-id="1c4a1-161">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="1c4a1-162">Azure Active Directory pakalpojuma darbspējas pārbaudei pārbaudiet statusu **drošības + identitātes** pakalpojumi, kas norādīti [Azure statusa lapā](https://azure.microsoft.com/status/).</span><span class="sxs-lookup"><span data-stu-id="1c4a1-162">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="1c4a1-163">Office pakalpojumiem, kas sniedz ieguldījumu programmā Microsoft Graph, pārbaudiet pakalpojumu statusu, kas norādīti [Office pakalpojumu darbspējas informācijas panelī](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="1c4a1-163">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
