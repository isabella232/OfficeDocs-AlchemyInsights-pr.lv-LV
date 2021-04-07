---
title: Atrodiet trūkstošās lietojumprogrammas programmas reģistrācijas asmenī
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
- "9004352"
- "9654"
ms.openlocfilehash: 00b5821e2edad8b60ff60b1f85264d81c72277e4
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404697"
---
# <a name="find-missing-applications-on-app-registration-blade"></a><span data-ttu-id="c1bb7-102">Atrodiet trūkstošās lietojumprogrammas programmas reģistrācijas asmenī</span><span class="sxs-lookup"><span data-stu-id="c1bb7-102">Find missing applications on App Registration blade</span></span>

1. <span data-ttu-id="c1bb7-103">Nevar atrast lietojumprogrammas lietojumprogrammu reģistrācijas portālā.</span><span class="sxs-lookup"><span data-stu-id="c1bb7-103">Cannot find applications on App Registration portal.</span></span>

    <span data-ttu-id="c1bb7-104">Ja programma ir vairāku nomnieku programma un tā ir reģistrēta citā nomniekā, tā netiks rādīta zem programmas reģistrācijas asmens stūra.</span><span class="sxs-lookup"><span data-stu-id="c1bb7-104">If an application is a multi-tenant application and it was registered in another tenant, it will not be displayed under App Registration blade.</span></span> <span data-ttu-id="c1bb7-105">Tomēr pēc piekļuves (pēc piekrišanas) un jūsu nomniekā ir izveidota pakalpojuma pamatsumma, iespējams, to atradīsit Enterprise Applications asmens slāpī.</span><span class="sxs-lookup"><span data-stu-id="c1bb7-105">However, you may find it under Enterprise Applications blade once it has been accessed (after being consented) and service principal has been created in your tenant.</span></span> <span data-ttu-id="c1bb7-106">Papildinformāciju skatiet rakstā [& identitātes platformas Azure AD — Microsoft identitātes platforma.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)</span><span class="sxs-lookup"><span data-stu-id="c1bb7-106">For more information, see [Apps & service principals in Azure AD - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).</span></span>
2. <span data-ttu-id="c1bb7-107">Nevar skatīt programmas programmu reģistrācijas asmens slāpē, pat ja esat administrators.</span><span class="sxs-lookup"><span data-stu-id="c1bb7-107">Unable to view apps in App Registration blade even though you are an admin.</span></span>

    <span data-ttu-id="c1bb7-108">Pārliecinieties, vai esat pareizajā direktorijā Azure portālā.</span><span class="sxs-lookup"><span data-stu-id="c1bb7-108">Please ensure you are in the right directory on the Azure portal.</span></span>
3. <span data-ttu-id="c1bb7-109">Mana programma nav norādīta sadaļā Enterprise Applications asmens saraksts, bet tā tiek parādīta, kad es izveidoju vaicājumu PowerShell komandai.</span><span class="sxs-lookup"><span data-stu-id="c1bb7-109">My application is not listed under Enterprise Applications blade but it shows up when I query PowerShell command.</span></span>

    <span data-ttu-id="c1bb7-110">Dažreiz, kad lietojumprogrammu izdzēšat no Azure portāla, tā netiek rādīta portālā, bet, iespējams, nav pilnībā izdzēsta.</span><span class="sxs-lookup"><span data-stu-id="c1bb7-110">Sometimes, after you delete the application from the Azure portal it does not show up in the portal but it may not have been deleted completely.</span></span> <span data-ttu-id="c1bb7-111">Papildinformāciju skatiet šeit:</span><span class="sxs-lookup"><span data-stu-id="c1bb7-111">For more information, see:</span></span>
    - <span data-ttu-id="c1bb7-112">Varat izgūt iepriekš izdzēsto lietojumprogrammu sarakstu un redzēt, vai lietojumprogramma sarakstā tiek parādīta, izmantojot Powershell komandu: **Get-AzureADDeletedApplication**.</span><span class="sxs-lookup"><span data-stu-id="c1bb7-112">You can retrieve the list of previously deleted applications and see if the application shows up in the list by using the Powershell command: **Get-AzureADDeletedApplication**.</span></span> <span data-ttu-id="c1bb7-113">Papildinformāciju skatiet rakstā [Get-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication)</span><span class="sxs-lookup"><span data-stu-id="c1bb7-113">To learn more, see [Get-AzureADDeletedApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication).</span></span>
    - <span data-ttu-id="c1bb7-114">Ja vēlaties pilnībā noņemt lietojumprogrammu, varat izmēģināt tālāk norādītos mēģinājumus programmā PowerShell: **Remove-AzureADApplication -ObjectId**.</span><span class="sxs-lookup"><span data-stu-id="c1bb7-114">If you want to remove the application completely, you can try the following in PowerShell: **Remove-AzureADApplication -ObjectId**.</span></span> <span data-ttu-id="c1bb7-115">Papildinformāciju skatiet rakstā [AzureADApplication (AzureAD) noņemšana.](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication)</span><span class="sxs-lookup"><span data-stu-id="c1bb7-115">To learn more, see [Remove-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication).</span></span>
    - <span data-ttu-id="c1bb7-116">Vai arī varat mēģināt atjaunot izdzēsto lietojumprogrammu, izmantojot šādu Powershell komandu: **AzureADDeletedApplication -ObjectId** atjaunošana.</span><span class="sxs-lookup"><span data-stu-id="c1bb7-116">Alternatively, you can try restoring the deleted application using the following Powershell command: **Restore AzureADDeletedApplication -ObjectId**.</span></span> <span data-ttu-id="c1bb7-117">Papildinformāciju skatiet rakstā [Restore-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)</span><span class="sxs-lookup"><span data-stu-id="c1bb7-117">To learn more, see [Restore-AzureADDeletedApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span></span>
4. <span data-ttu-id="c1bb7-118">Savā jaunajā Azure nomniekā nevar atrast visu sākotnēji instalēto uzņēmuma lietojumprogrammu sarakstu.</span><span class="sxs-lookup"><span data-stu-id="c1bb7-118">Can’t find list of all pre-installed enterprise applications in my new Azure tenant.</span></span>

    <span data-ttu-id="c1bb7-119">Pēc noklusējuma azure AD nav sākotnēji instalētas uzņēmuma lietojumprogrammas.</span><span class="sxs-lookup"><span data-stu-id="c1bb7-119">There are no pre-installed enterprise applications in Azure AD by default.</span></span> <span data-ttu-id="c1bb7-120">Tā ir manuāli jāpievieno no opcijas "Jauna lietojumprogramma", pārlūkojot to no Azure AD galerijas vai pievienojot lietojumprogrammu, kas nav galerija.</span><span class="sxs-lookup"><span data-stu-id="c1bb7-120">You need to add it manually from the ‘New application’ option by browsing it from Azure AD gallery or add a non-gallery application.</span></span> <span data-ttu-id="c1bb7-121">Papildinformāciju skatiet rakstā [Īsā pamācība: programmas pievienošana Azure Active Directory (Azure AD) nomniekam.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)</span><span class="sxs-lookup"><span data-stu-id="c1bb7-121">To learn more, see [Quickstart: Add an application to your Azure Active Directory (Azure AD) tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal).</span></span>
    <span data-ttu-id="c1bb7-122">Ja esat globālais administrators, varat viegli piekļūt savām programmām, izmantojot [Microsoft 365 lietojumprogrammu palaidēju](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher).</span><span class="sxs-lookup"><span data-stu-id="c1bb7-122">If you are a global administrator, you can easily access your apps using the [Microsoft 365 App Launcher](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher).</span></span>
5. <span data-ttu-id="c1bb7-123">Nevar atrast manas lietojumprogrammas no portāla Manas lietojumprogrammas.</span><span class="sxs-lookup"><span data-stu-id="c1bb7-123">Unable to find my apps from My Apps portal.</span></span>

    <span data-ttu-id="c1bb7-124">Pārliecinieties, vai lietojumprogrammas nav paslēptas kolekcijas Mana lietojumprogramma lapā.</span><span class="sxs-lookup"><span data-stu-id="c1bb7-124">Make sure that apps are not hidden in My Apps collection page.</span></span> <span data-ttu-id="c1bb7-125">Papildinformāciju skatiet rakstā [Kolekcijas (priekšskatījums) portālā Manas programmas — Azure AD.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections)</span><span class="sxs-lookup"><span data-stu-id="c1bb7-125">To learn more, see [Collections (preview) in the My Apps portal - Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections).</span></span>
6. <span data-ttu-id="c1bb7-126">Lai startētu lietojumprogrammas no portāla Manas programmas, skatiet & programmu atrašana manu [lietojumprogrammu portālā — Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access).</span><span class="sxs-lookup"><span data-stu-id="c1bb7-126">To start apps from the My Apps portal, see [Locate & use apps on the My Apps portal - Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access).</span></span>
7. <span data-ttu-id="c1bb7-127">Pēc instalēšanas Office 365 Mover programma netiek rādīta Enterprise Applications asmens slāpī.</span><span class="sxs-lookup"><span data-stu-id="c1bb7-127">Office 365 Mover app is not showing up on Enterprise Applications blade after installation.</span></span>

    <span data-ttu-id="c1bb7-128">Lietojumprogramma "Office 365 Mover" ir vairāku nomnieku programma, kas nav jāpievieno AAD, izmantojot sadaļas Galerijas lietojumprogrammas sadaļā Enterprise Programmu reģistrācija.</span><span class="sxs-lookup"><span data-stu-id="c1bb7-128">The "Office 365 Mover" application is a multitenant app that doesn’t need to be added to AAD using the Gallery Applications section under Enterprise App Registration.</span></span> <span data-ttu-id="c1bb7-129">Lai piekļūtu Office 365 pārvietošanas programmai, vienkārši pierakstieties lietojumprogrammā un pieprasiet lietotāja piekrišanu atļaujām.</span><span class="sxs-lookup"><span data-stu-id="c1bb7-129">To access Office 365 Mover app, simply sign-in to the app and it would ask for user's consent for the permissions.</span></span> <span data-ttu-id="c1bb7-130">Kad lietotājs būs sniedzis piekrišanu, šī lietojumprogramma tiks automātiski pievienota nomniekam ar e-pasta ID, kuru esat pieteicies.</span><span class="sxs-lookup"><span data-stu-id="c1bb7-130">Once the user provides the consent, this app would automatically get added to the tenant with the email id you have logged in.</span></span>

    <span data-ttu-id="c1bb7-131">Pēc pierakstīšanās lietojumprogrammā jums jāspēj atrast šīs lietojumprogrammas ierakstu AAD sadaļā Enterprise Applications asmens lietojumprogrammu asmens.</span><span class="sxs-lookup"><span data-stu-id="c1bb7-131">After signing into the application, you should be able to find this application's entry under the Enterprise Applications' blade in AAD.</span></span> <span data-ttu-id="c1bb7-132">Lietojumprogramma ir jāmeklē, ierakstot vārdu un uzvārdu, piemēram, "Office 365 Mover" vai vienkārši meklējiet "office", un tajā jābūt uzskaitītai programmai.</span><span class="sxs-lookup"><span data-stu-id="c1bb7-132">You need to search for that application by either typing the full name, i.e., "Office 365 Mover" or simply search "office" and it should list the app.</span></span> <span data-ttu-id="c1bb7-133">Lai uzzinātu vairāk, skatiet [rakstu Office 365 Mover](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)norāda, ka tas jau ir instalēts, bet nav norādīts Enterprise lietojumprogrammu galerijā.</span><span class="sxs-lookup"><span data-stu-id="c1bb7-133">To learn more, see [Office 365 Mover says it's already installed but it's not listed in the Enterprise Application gallery](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html).</span></span>
8. <span data-ttu-id="c1bb7-134">Īsā pamācība: skatiet to lietojumprogrammu sarakstu, kuras izmanto jūsu [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) nomnieku identitātes pārvaldībai, parāda, kā skatīt lietojumprogrammas, kuras tiek dēvētas arī par lietojumprogrammām, kuras jau ir iestatītas izmantot jūsu Azure AD nomnieku kā identitātes nodrošinātāju (IdP).</span><span class="sxs-lookup"><span data-stu-id="c1bb7-134">[Quickstart: View the list of applications that are using your Azure Active Directory (Azure AD) tenant for identity management](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) shows you how to view the applications, also known as apps, that are already set up to use your Azure AD tenant as their Identity Provider (IdP).</span></span>
9. <span data-ttu-id="c1bb7-135">[Novērsiet bieži sastopamās](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) problēmas, pievienojot vai noņemot lietojumprogrammu pakalpojumā Azure Active Directory, varat izprast biežāk sastopamās problēmas, ar kurām lietotāji saskaras ar lietojumprogrammu skatīšanu pakalpojumā Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c1bb7-135">[Troubleshoot common problem adding or removing an application to Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) helps you understand the common problems people face viewing apps in Azure Active Directory.</span></span>