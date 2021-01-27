---
title: Lietotāju problēmu novēršana
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7813"
- "9004358"
ms.openlocfilehash: d9964e50bdea0c41ac14ab3783b579034b5f2c8c
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901041"
---
# <a name="announcements"></a><span data-ttu-id="492ad-102">Paziņojumi</span><span class="sxs-lookup"><span data-stu-id="492ad-102">Announcements</span></span>

<span data-ttu-id="492ad-103">Sekojiet Google norādījumiem par saderību ar testēšanu, lai pārbaudītu, vai jūsu lietojumprogrammas ir ietekmētas.</span><span class="sxs-lookup"><span data-stu-id="492ad-103">Follow Google's guidance on testing compatibility to test whether your apps are affected.</span></span> <span data-ttu-id="492ad-104">Google norādījumi ir pieejami https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support .</span><span class="sxs-lookup"><span data-stu-id="492ad-104">Google's guidance is available in https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support.</span></span>

<span data-ttu-id="492ad-105">Pārliecinieties, vai, pierakstoties lietotājiem ar patērētāju Google kontiem, izmantojat sistēmas tīmekļa skatu vai sistēmas pārlūkprogrammu.</span><span class="sxs-lookup"><span data-stu-id="492ad-105">Ensure you use the system webview or system browser when signing in your users with consumer Google accounts.</span></span> <span data-ttu-id="492ad-106">Papildinformāciju skatiet rakstā problēmas, [pierakstoties lietojumprogrammā (-as), izmantojot tikai Chrome pārlūkprogrammu](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).</span><span class="sxs-lookup"><span data-stu-id="492ad-106">For more information, see [Issues signing in to application(s) using Chrome browser only](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).</span></span>


<span data-ttu-id="492ad-107">**Nevaru izveidot jaunu lietotāju savā Azure AD direktorijā**</span><span class="sxs-lookup"><span data-stu-id="492ad-107">**I can't create a new user in my Azure AD directory**</span></span>

<span data-ttu-id="492ad-108">Lai novērstu problēmu, ka Azure AD nav iespējams izveidot jaunu lietotāju, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="492ad-108">To troubleshoot the issue of not being able to create a new user in Azure AD, perform the following steps:</span></span>

1. <span data-ttu-id="492ad-109">Pārliecinieties, vai esat autorizēts izveidot jaunu standarta lietotāju.</span><span class="sxs-lookup"><span data-stu-id="492ad-109">Ensure that you are authorized to create a new standard user.</span></span> <span data-ttu-id="492ad-110">Azure Active Directory (AD) tikai globālā administratora vai lietotāja administratora loma var izveidot jaunu standarta lietotāju.</span><span class="sxs-lookup"><span data-stu-id="492ad-110">Only the global administrator or user administrator role in Azure Active Directory (AD) can create a new standard user.</span></span> <span data-ttu-id="492ad-111">Ja neesat kādā no šīm lomām, lūdziet administratoram pievienot jūs kādai no šīm lomām vai izveidot jaunu lietotāja kontu.</span><span class="sxs-lookup"><span data-stu-id="492ad-111">If you're not in one of these roles, ask an administrator to add you to one of these roles or to create the new user account for you.</span></span>
2. <span data-ttu-id="492ad-112">Pārliecinieties, vai lietotājvārds ir domēnā, kas ir verificēts Azure AD.</span><span class="sxs-lookup"><span data-stu-id="492ad-112">Ensure that the user name is in a domain that is verified in your Azure AD.</span></span> <span data-ttu-id="492ad-113">Ja Azure AD nav pārbaudīti pielāgoti domēnu nosaukumi, varat izmantot Azure AD sākotnējo domēnu, kas beidzas ar \*. onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="492ad-113">If you do not have any verified custom domain names in your Azure AD, you can use your Azure AD initial domain, which ends with \*.onmicrosoft.com.</span></span>
3. <span data-ttu-id="492ad-114">Pārliecinieties, vai lietotājvārds ir domēnā, kas nav Azure AD integrētās reklāmas no lokālās reklāmas.</span><span class="sxs-lookup"><span data-stu-id="492ad-114">Ensure that the user name is in a domain that is not federated to Azure AD from your on-premises AD.</span></span> <span data-ttu-id="492ad-115">Lietotāji nevar pievienot mākonī ar domēnu nosaukumiem, kas tiek apvienoti no lokālās atrašanās vietas.</span><span class="sxs-lookup"><span data-stu-id="492ad-115">Users cannot be added in the cloud with domain names that are federated from on-premises.</span></span>
4. <span data-ttu-id="492ad-116">Pārliecinieties, vai nevienam lietotājam vai kontaktpersonai jau ir lietotājvārds, ko vēlaties piešķirt jaunajam lietotājam.</span><span class="sxs-lookup"><span data-stu-id="492ad-116">Ensure that no other user or contact already has the user name that you want to assign to the new user.</span></span> <span data-ttu-id="492ad-117">Lietotāju nosaukumiem ir jābūt unikāliem visā Azure AD.</span><span class="sxs-lookup"><span data-stu-id="492ad-117">User names must be unique across Azure AD.</span></span>
5. <span data-ttu-id="492ad-118">Skatiet [Azure AD lomas un administratorus](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) par savu Azure AD.</span><span class="sxs-lookup"><span data-stu-id="492ad-118">See [Azure AD roles and administrators](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
6. <span data-ttu-id="492ad-119">Skatiet Azure AD [domēnu nosaukumus](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Domains) .</span><span class="sxs-lookup"><span data-stu-id="492ad-119">See the [domain names](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Domains) for your Azure AD.</span></span>
7. <span data-ttu-id="492ad-120">Pārskatiet [audita žurnālus](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Audit) , lai skatītu detalizētāku informāciju par nesen izveidotu vai izdzēstu lietotāju, piemēram, kurš veica darbību, un kad.</span><span class="sxs-lookup"><span data-stu-id="492ad-120">Review [Audit logs](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Audit) to see more detailed information about a recently created or deleted user like who performed the action and when.</span></span>
8. <span data-ttu-id="492ad-121">Lai iegūtu papildinformāciju par jaunu lietotāju pievienošanu, skatiet sadaļu [debeszils portāla izmantošana, lai izveidotu jaunu lietotāju AZURE ad](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory) .</span><span class="sxs-lookup"><span data-stu-id="492ad-121">For more information on adding new users, see [Use the Azure portal to create a new user in your Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory) .</span></span>
9. <span data-ttu-id="492ad-122">Lai iegūtu papildinformāciju par administratora lomu atļaujām Azure AD, skatiet rakstu [AZURE ad administratīvās lomas](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="492ad-122">For more information on administrator role permissions in Azure AD, see [Azure AD administrative roles](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference).</span></span>
10. <span data-ttu-id="492ad-123">Detalizētu informāciju par to, kā izveidot lietotāju, izmantojot Azure AD PowerShell, skatiet sadaļā [AZURE ad PowerShell, lai izveidotu jaunu lietotāju](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser).</span><span class="sxs-lookup"><span data-stu-id="492ad-123">For details on creating a user using Azure AD Powershell, see [Azure AD PowerShell to create a new user](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser).</span></span>

<span data-ttu-id="492ad-124">**Problēma ar pašapkalpošanās reģistrēšanu**</span><span class="sxs-lookup"><span data-stu-id="492ad-124">**Problem with self-service sign up**</span></span>

<span data-ttu-id="492ad-125">Lai novērstu problēmas saistībā ar pašapkalpošanās reģistrēšanu, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="492ad-125">To troubleshoot issues regarding self-service sign up, perform the following steps:</span></span>

1. <span data-ttu-id="492ad-126">Lai izmantotu patstāvīgi izmantojamas reģistrācijas lietojumprogrammas, vispirms ir jāiespējo patstāvīgi reģistrēties savam nomniekam.</span><span class="sxs-lookup"><span data-stu-id="492ad-126">To use self-service sign-up with your applications, first enable self-service sign-up for your tenant.</span></span> 
2. <span data-ttu-id="492ad-127">Lai iespējotu lietojumprogrammas atbalstu pašapkalpošanās reģistrēšanās, pievienojiet to lietotāja plūsmai.</span><span class="sxs-lookup"><span data-stu-id="492ad-127">To enable an application to support self-service sign up, add it to your user flow .</span></span> <span data-ttu-id="492ad-128">Nākamajā reizē, kad dosities uz šīs lietojumprogrammas pieteikšanās lapu, redzēsit opciju \**_nav konta? Izveidojiet to!_* _.</span><span class="sxs-lookup"><span data-stu-id="492ad-128">The next time you go to the login page for that application, you'll see an option \**_No account? Create one!_* _.</span></span> <span data-ttu-id="492ad-129">Tādējādi tiek sākts pašapkalpošanās reģistrācijas process.</span><span class="sxs-lookup"><span data-stu-id="492ad-129">This starts the self-service sign-up process.</span></span>
3. <span data-ttu-id="492ad-130">Lai iegūtu informāciju par to, kā izmantot pašapkalpošanās reģistrēšanos, lai aizpildītu organizāciju Azure AD, skatiet rakstu [pašapkalpošanās reģistrācija pakalpojumam AZURE ad](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-self-service-signup).</span><span class="sxs-lookup"><span data-stu-id="492ad-130">For information on how to use self-service sign up to populate an organization in Azure AD, see [Self-service sign up for Azure AD](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-self-service-signup).</span></span>
4. <span data-ttu-id="492ad-131">Pēc tam, kad esat saistījis lietotāju plūsmu ar vienu vai vairākām lietojumprogrammām, lietotāji, kuri apmeklē šo programmu, varēs reģistrēties un iegūt viesa kontu, izmantojot lietotāja plūsmā konfigurētās opcijas.</span><span class="sxs-lookup"><span data-stu-id="492ad-131">Once you associate the user flow with one or more applications, users who visit that app will be able to sign up and gain a guest account using the options configured in the user flow.</span></span> <span data-ttu-id="492ad-132">Lai iegūtu papildinformāciju par to, kā reģistrēt un iegūt viesa kontu, lietotāji var redzēt viesu lietotāju pašapkalpošanās [reģistrēšanu](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow).</span><span class="sxs-lookup"><span data-stu-id="492ad-132">For more information on signing up and gaining a guest account, the users can see [Self-service sign-up for guest users](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow).</span></span>

<span data-ttu-id="492ad-133">*Kļūda, uzaicinot ārēju lietotāju*\*</span><span class="sxs-lookup"><span data-stu-id="492ad-133">_ *Problem inviting an external user*\*</span></span>

<span data-ttu-id="492ad-134">Lai novērstu problēmas saistībā ar ārēja lietotāja uzaicināšanu, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="492ad-134">To troubleshoot issues regarding inviting an external user, perform the following step:</span></span>

<span data-ttu-id="492ad-135">Pārliecinieties, vai esat nosūtījis lietotāja uzaicinājumu uz e-pasta adresi, kas atbilst vārdam, ar kuru pierakstās lietotājs.</span><span class="sxs-lookup"><span data-stu-id="492ad-135">Ensure that you send a user's invitation to the email address that matches the name that the user signs in with.</span></span> <span data-ttu-id="492ad-136">Ja nosūtāt uzaicinājumu uz lietotāja starpniekservera e-pasta adresi, lietotājs to nevar izmantot.</span><span class="sxs-lookup"><span data-stu-id="492ad-136">If you send the invitation to a user's proxy email address, the user can't redeem it.</span></span> <span data-ttu-id="492ad-137">Papildinformāciju skatiet rakstā [AZURE ad B2B dokumentācija](https://docs.microsoft.com/azure/active-directory/external-identities/).</span><span class="sxs-lookup"><span data-stu-id="492ad-137">For more information, see [Azure AD B2B documentation](https://docs.microsoft.com/azure/active-directory/external-identities/).</span></span>

<span data-ttu-id="492ad-138">**Nevaru piešķirt licences lietotājam**</span><span class="sxs-lookup"><span data-stu-id="492ad-138">**I can't assign licenses to a user**</span></span>

<span data-ttu-id="492ad-139">Lai novērstu problēmas saistībā ar licenču piešķiršanu lietotājam, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="492ad-139">To troubleshoot issues regarding assigning licenses to a user, perform the following steps:</span></span>

1. <span data-ttu-id="492ad-140">Lai pārvaldītu lietotāju licences, pārliecinieties, vai izmantojat kontu ar vienu no nepieciešamajām administratora lomām: globālais administrators, licenču administrators vai lietotāja administrators.</span><span class="sxs-lookup"><span data-stu-id="492ad-140">To manage user licenses, ensure that you use an account with one of the required administrator roles: global administrator, license administrator, or user administrator.</span></span> <span data-ttu-id="492ad-141">Varat pārbaudīt lietotāja lomu lietotāja diska cilnē **direktorija loma** .</span><span class="sxs-lookup"><span data-stu-id="492ad-141">You can check the user’s role in the **Directory role** tab on the user blade.</span></span>
2. <span data-ttu-id="492ad-142">Ja izmantojat Azure portālu un licenču piešķiršana neizdodas, noklikšķiniet uz paziņojuma augšējā labajā stūrī.</span><span class="sxs-lookup"><span data-stu-id="492ad-142">If you are using the Azure portal and license assignment is failing, click the notification in the upper-right corner.</span></span> <span data-ttu-id="492ad-143">Tiks atvērts asmens ar detalizētu informāciju par to, kas notika nepareizi.</span><span class="sxs-lookup"><span data-stu-id="492ad-143">This opens a blade with details about what went wrong.</span></span> <span data-ttu-id="492ad-144">Lielākajā daļā gadījumu tas ir pietiekami, lai saprastu un atrisinātu problēmu.</span><span class="sxs-lookup"><span data-stu-id="492ad-144">In most cases that is enough to understand and resolve the problem.</span></span>
3. <span data-ttu-id="492ad-145">Lai lietotājam varētu piešķirt licenci, pārliecinieties, vai ir iestatīts lietotāja rekvizīts **lietojuma vieta** .</span><span class="sxs-lookup"><span data-stu-id="492ad-145">Before a license can be assigned to a user, ensure that the **Usage Location** property is set for the user.</span></span> <span data-ttu-id="492ad-146">Pārbaudiet, vai lietotājam ir šī rekvizīta kopa, skatot lietotāja asmens cilni **profils** .</span><span class="sxs-lookup"><span data-stu-id="492ad-146">Verify the user has that property set by viewing the **Profile** tab on the user blade.</span></span>
4. <span data-ttu-id="492ad-147">Pārliecinieties, vai ir pieejamas pietiekamas licences produktam, kuru mēģināt piešķirt.</span><span class="sxs-lookup"><span data-stu-id="492ad-147">Ensure there are enough available licenses for the product you are trying to assign.</span></span> <span data-ttu-id="492ad-148">Pieejamo licenču skaitu Azure portālā varat skatīt Azure [Active Directory-> licences-> visiem produktiem](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/LicensesMenuBlade/Products).</span><span class="sxs-lookup"><span data-stu-id="492ad-148">You can see the number of available licenses in the Azure portal, at [Azure Active Directory -> Licenses -> All products](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/LicensesMenuBlade/Products).</span></span>
5. <span data-ttu-id="492ad-149">Lietotājam, iespējams, jau ir cita licence, kuras pakalpojumi konfliktē ar jaunajām licencēm, ko mēģināt piešķirt.</span><span class="sxs-lookup"><span data-stu-id="492ad-149">The user may already have another license whose services conflict with those in the new license you are trying to assign.</span></span> <span data-ttu-id="492ad-150">Piemēram, ja lietotājam ir iespējots pakalpojums Exchange Online (1. plāns), jūs nevarēsit piešķirt licenci pakalpojumam Exchange Online (2. plāns).</span><span class="sxs-lookup"><span data-stu-id="492ad-150">For example, if the user has the Exchange Online (Plan 1) service enabled, you won’t be able to assign a license with the Exchange Online (Plan 2).</span></span> <span data-ttu-id="492ad-151">Atspējojiet kādu no pakalpojumiem, lai atļautu jauno licenču piešķiršanu.</span><span class="sxs-lookup"><span data-stu-id="492ad-151">Disable one of the services to allow the new license assignment.</span></span> <span data-ttu-id="492ad-152">Ja izmantojat Azure Portal vai PowerShell cmdlet, **detalizētās informācijas** lapā ir uzskaitīti īpašie pakalpojumi, kas izraisa konfliktu.</span><span class="sxs-lookup"><span data-stu-id="492ad-152">If you are using the Azure portal or PowerShell cmdlets, the **problem details** page lists the specific services that are causing the conflict.</span></span>
6. <span data-ttu-id="492ad-153">Ja mēģināt noņemt licenci un tas neizdodas, lietotājam var būt citas licences ar pakalpojumiem, kas ir atkarīgi no pakalpojumiem, kurus cenšaties noņemt.</span><span class="sxs-lookup"><span data-stu-id="492ad-153">If you are trying to remove a license and that is failing, the user might have other licenses with services that depend on the services you are trying to remove.</span></span> <span data-ttu-id="492ad-154">Ja izmantojat Azure Portal vai PowerShell cmdlet, kļūdas ziņojumā tiek uzskaitīti konkrēti pakalpojumi, kuriem ir atkarības.</span><span class="sxs-lookup"><span data-stu-id="492ad-154">If you are using the Azure portal or PowerShell cmdlets, the error message will list the specific services that have dependencies.</span></span>
7. <span data-ttu-id="492ad-155">Ja vēlaties saprast, kāpēc no lietotāja ir pievienota vai noņemta licence (piemēram, kurš vēl jūsu organizācijā ir veicis izmaiņas), pārbaudiet audita žurnālus.</span><span class="sxs-lookup"><span data-stu-id="492ad-155">If you want to understand why a license was added/removed from a user (for example, who else in your organization may have made changes), check the audit logs.</span></span> <span data-ttu-id="492ad-156">Iestatiet filtru, lai tiktu rādītas visas modifikācijas, ieskaitot tās **, kas tās** ir veikušas.</span><span class="sxs-lookup"><span data-stu-id="492ad-156">Set the filter to **license activities** to show all modifications, including the "actor" that performed them.</span></span>
8. <span data-ttu-id="492ad-157">Ja izmantojat Exchange Online, daži nomnieka lietotāji, iespējams, ir nepareizi konfigurēti ar to pašu starpniekservera adreses vērtību.</span><span class="sxs-lookup"><span data-stu-id="492ad-157">If you are using Exchange Online, some users in your tenant may be incorrectly configured with the same proxy address value.</span></span> <span data-ttu-id="492ad-158">Šādos gadījumos, iespējams, redzēsit vispārējus kļūdu ziņojumus, ja licences operācija bankrotē.</span><span class="sxs-lookup"><span data-stu-id="492ad-158">In such cases, you may see generic error messages when a license operation fails.</span></span> <span data-ttu-id="492ad-159">[Šajā rakstā](https://docs.microsoft.com/exchange/troubleshoot/administration/proxy-address-being-used) ir sniegta papildinformācija par šo problēmu, tostarp informācija par to, [kā izveidot savienojumu ar Exchange Online, izmantojot Remote PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell). Lai noteiktu, kuri lietotāji jūsu nomniekā satur to pašu starpniekservera adresi, izpildīs šo Exchange Online cmdlet:</span><span class="sxs-lookup"><span data-stu-id="492ad-159">[This article](https://docs.microsoft.com/exchange/troubleshoot/administration/proxy-address-being-used) contains more information about this problem, including information on [how to connect to Exchange Online using remote PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).To identify which users in your tenant, contain the same proxy address, execute this Exchange Online cmdlet:</span></span>

<span data-ttu-id="492ad-160">Palaist</span><span class="sxs-lookup"><span data-stu-id="492ad-160">Run</span></span>

<span data-ttu-id="492ad-161">Get-Recipient | kur {$ _. Parametrā EmailAddresses norādītā-Match <user principal name> } | fL nosaukums, RecipientType, parametrā EmailAddresses norādītā</span><span class="sxs-lookup"><span data-stu-id="492ad-161">Get-Recipient | where {$_.EmailAddresses -match <user principal name>} | fL Name, RecipientType,emailaddresses</span></span>




