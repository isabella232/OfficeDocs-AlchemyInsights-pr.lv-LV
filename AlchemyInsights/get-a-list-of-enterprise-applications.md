---
title: Enterprise lietojumprogrammu saraksta izveide
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "9837"
ms.openlocfilehash: f5c1a77e415d4bbaa5718a6668af95934db7e5ae
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/26/2021
ms.locfileid: "51404928"
---
# <a name="get-a-list-of-enterprise-applications"></a><span data-ttu-id="58381-102">Enterprise lietojumprogrammu saraksta izveide</span><span class="sxs-lookup"><span data-stu-id="58381-102">Get a list of Enterprise Applications</span></span>

1. <span data-ttu-id="58381-103">Lai **iegūtu** sarakstu ar uzņēmuma lietojumprogrammām (visas lietojumprogrammas vai filtrētas pēc parādāmā vārda, ID, identifikatoru URI u.c.), izmantojot Powershell komandu, skatiet rakstu [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span><span class="sxs-lookup"><span data-stu-id="58381-103">To **get a list of enterprise applications** (all applications or filtered by Display name, ID, Identifier URIs, etc.) through Powershell command, see [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span></span>
2. <span data-ttu-id="58381-104">Lai iegūtu pakalpojuma pamatobjektu sarakstu (visus objektus vai atfiltrējot pēc ID), izmantojot Powershell komandu, skatiet rakstu [Get-AzureADServicePrincipal (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal)</span><span class="sxs-lookup"><span data-stu-id="58381-104">To get a list of service principal objects (all objects or filtered by ID) through Powershell command, see [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span></span>
3. <span data-ttu-id="58381-105">Ja vēlaties iegūt **SAML konfigurēto programmu sarakstu,** tālāk norādītās PowerShell skripti var palīdzēt:</span><span class="sxs-lookup"><span data-stu-id="58381-105">If you want to **get a list of SAML configured apps, following PowerShell scripts** may help you:</span></span>

    <span data-ttu-id="58381-106">Katrā lietojumprogrammā (OAuth programmā vai SAML programmā (gan galerijā, gan programmās, kas nav galerijas) būtu divi objekti, kas tiek izveidoti AAD, kad notiek to reģistrācija.</span><span class="sxs-lookup"><span data-stu-id="58381-106">Every Application be it an OAuth app or SAML app (both gallery and non-gallery apps) would have two objects created in AAD when their registration happens.</span></span> <span data-ttu-id="58381-107">Viens tiek dēvēts par lietojumprogrammas objektu, bet otra — objekts Service Principal.</span><span class="sxs-lookup"><span data-stu-id="58381-107">One is called the Application Object and the other is the Service Principal object.</span></span> <span data-ttu-id="58381-108">Kad, izmantojot PowerShell, izmantojat pakalpojuma pamat objekta rekvizītus, katrai lietojumprogrammai ir piesaistīts noteikts skaits ar to saistīto atzīmju:</span><span class="sxs-lookup"><span data-stu-id="58381-108">When you dump the properties of a Service Principal Object using PowerShell, you would find that every application has a certain number of Tags associated with it like:</span></span>

    - <span data-ttu-id="58381-109">OAuth programmām būtu atzīme "**WindowsAzureActiveDirectoryIntegratedApp**"</span><span class="sxs-lookup"><span data-stu-id="58381-109">OAuth apps would have a tag called "**WindowsAzureActiveDirectoryIntegratedApp**"</span></span>
    - <span data-ttu-id="58381-110">Galerija SAML lietojumprogrammām būtu atzīme **"WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span><span class="sxs-lookup"><span data-stu-id="58381-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span></span>
    - <span data-ttu-id="58381-111">Bez galerijas SAML lietojumprogrammām būtu atzīme **"WindowsAzureActiveDirectoryCustomSingleSignOnApplication"**</span><span class="sxs-lookup"><span data-stu-id="58381-111">Non-Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span></span>

    <span data-ttu-id="58381-112">Tādējādi varat izmantot šīs atzīmes un uzzināt, kāda programma tā ir.</span><span class="sxs-lookup"><span data-stu-id="58381-112">Hence, you can use these tags and find out what kind of app it is.</span></span> <span data-ttu-id="58381-113">Atzīme "**WindowsAzureActiveDirectoryIntegratedApp**" tiek bieži lietots visu veidu programmām.</span><span class="sxs-lookup"><span data-stu-id="58381-113">The tag "**WindowsAzureActiveDirectoryIntegratedApp**" is common to all types of apps.</span></span> <span data-ttu-id="58381-114">Lai uzskaitītu visas SAML programmas (gan galerijā, gan ārpus galerijas), varat izmantot tālāk norādīto fragmentu.</span><span class="sxs-lookup"><span data-stu-id="58381-114">You can use following snippet to list all the SAML apps (both gallery and non-gallery):</span></span>

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    <span data-ttu-id="58381-115">Papildinformāciju skatiet rakstā [SamL iespējoto programmu identificēšana pakalpojumā Azure AD.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)</span><span class="sxs-lookup"><span data-stu-id="58381-115">For more information, see [Identify SAML-enabled apps in Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span></span>

4. <span data-ttu-id="58381-116">**Tikai tīmekļa lietojumprogrammu atrašana** un saraksts: izmantojiet tālāk norādīto komandu, lai iegūtu visas Azure AD lietojumprogrammas ar lietojumprogrammas tipu "Tīmekļa lietojumprogramma/API"</span><span class="sxs-lookup"><span data-stu-id="58381-116">**Find and list only Web applications**: Use the below command to get all Azure AD applications with the application type "Web app/API"</span></span>

    <span data-ttu-id="58381-117">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT</span><span class="sxs-lookup"><span data-stu-id="58381-117">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -ne $true } | FT</span></span>
5. <span data-ttu-id="58381-118">**Atrodiet un uzziniet tikai vietējās lietojumprogrammas:** izpildiet tālāk norādīto komandu, lai iegūtu visas vietējās klienta (darbvirsmas/mobilās ierīces) lietojumprogrammas.</span><span class="sxs-lookup"><span data-stu-id="58381-118">**Find and list Native applications alone**: Run the following command to get all the native client (desktop/mobile device) applications.</span></span>

    <span data-ttu-id="58381-119">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT</span><span class="sxs-lookup"><span data-stu-id="58381-119">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -eq $true } | FT</span></span>
6. <span data-ttu-id="58381-120">**Eksportēt visu reģistrēto Azure AD lietojumprogrammas informāciju CSV** failā: tālāk redzama komanda eksportē visas Azure AD programmas ar nepieciešamo informāciju csv failā:</span><span class="sxs-lookup"><span data-stu-id="58381-120">**Export All Registered Azure AD Application Details to CSV**: The below command exports all the Azure AD apps with required details to csv file:</span></span>

    - <span data-ttu-id="58381-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span><span class="sxs-lookup"><span data-stu-id="58381-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span></span>
    - <span data-ttu-id="58381-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span><span class="sxs-lookup"><span data-stu-id="58381-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span></span>

7. <span data-ttu-id="58381-123">**Nepieciešams eksportēt neizmantoto Azure programmu sarakstu** — audita atskaite</span><span class="sxs-lookup"><span data-stu-id="58381-123">**Need to export a list of unused Azure apps** – Audit report</span></span>

    <span data-ttu-id="58381-124">Azure AD var parādīt programmu žurnālus tikai līdz 30 dienām, ja jums ir Azure AD Premium licence.</span><span class="sxs-lookup"><span data-stu-id="58381-124">Azure AD can show application logs for only up to 30 days provided you have Azure AD Premium license.</span></span>
    <span data-ttu-id="58381-125">Ir divas iespējas saglabāt datus ilgāk par 30 dienām.</span><span class="sxs-lookup"><span data-stu-id="58381-125">You have two options to retain the data for longer than 30 days.</span></span> <span data-ttu-id="58381-126">Varat izmantot [Azure AD atskaišu API, lai](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) programmiski izgūtu datus un glabātu tos datu bāzē.</span><span class="sxs-lookup"><span data-stu-id="58381-126">You can use the [Azure AD Reporting APIs](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) to retrieve the data programmatically and store it in a database.</span></span> <span data-ttu-id="58381-127">Varat arī integrēt audita žurnālus trešās puses SIEM sistēmā.</span><span class="sxs-lookup"><span data-stu-id="58381-127">Alternatively, you can integrate audit logs into a third party SIEM system.</span></span>

    <span data-ttu-id="58381-128">Varat arī lejupielādēt lietojumprogrammu sarakstu visām lietojumprogrammām un piederošām lietojumprogrammām Azure Active Directory>programmu reģistrācijas>lejupielādēt>visas lietojumprogrammas/piederošās lietojumprogrammas.</span><span class="sxs-lookup"><span data-stu-id="58381-128">You can also download the app list for all applications and owned applications under Azure Active directory>App Registrations>Download>All applications/Owned applications.</span></span>

    <span data-ttu-id="58381-129">Lai iegūtu lietojumprogrammu sarakstu, izmantojot MS Graph, skatiet rakstu Sarakstu [lietojumprogrammas — Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) un lietojumprogrammas resursu [tips — Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span><span class="sxs-lookup"><span data-stu-id="58381-129">To get a list of applications through MS Graph, see [List applications - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) and [application resource type - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span></span>
