---
title: Problēmas ar akreditācijas datiem
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
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063680"
---
# <a name="issues-with-credentials"></a><span data-ttu-id="407fb-102">Problēmas ar akreditācijas datiem</span><span class="sxs-lookup"><span data-stu-id="407fb-102">Issues with credentials</span></span>

<span data-ttu-id="407fb-103">[Microsoft identitātes platformā un oauth 2,0 klienta akreditācijas datu plūsmā](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) ir paskaidrots, kā programmēt tieši atbilstoši OAuth 2,0 klienta akreditācijas datu plūsmai.</span><span class="sxs-lookup"><span data-stu-id="407fb-103">[Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) describes how to program directly against the OAuth 2.0 client credentials grant flow.</span></span>

<span data-ttu-id="407fb-104">**Kā pārvaldīt lietojumprogrammas paroles vai sertifikāta akreditācijas datus?**</span><span class="sxs-lookup"><span data-stu-id="407fb-104">**How do I manage an application's password or certificate credentials?**</span></span>

<span data-ttu-id="407fb-105">Azure CLI varat izmantot [AZ ad lietojumprogrammas akreditācijas](https://docs.microsoft.com/cli/azure/ad/app/credential) datus, lai izdzēstu, sarakstu vai atiestatītu lietojumprogrammas paroles vai sertifikāta akreditācijas datus.</span><span class="sxs-lookup"><span data-stu-id="407fb-105">In the Azure CLI, you can use [az ad app credential](https://docs.microsoft.com/cli/azure/ad/app/credential) to delete, list, or reset an application's password or certificate credentials.</span></span>

<span data-ttu-id="407fb-106">**Kā mani lietotāji var atiestatīt savas paroles?**</span><span class="sxs-lookup"><span data-stu-id="407fb-106">**How do my users reset their passwords?**</span></span>

<span data-ttu-id="407fb-107">Lai varētu atiestatīt savas paroles, lietotājiem ir [jāreģistrējas pašapkalpošanās paroles atiestatīšanai](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) .</span><span class="sxs-lookup"><span data-stu-id="407fb-107">Users need to [register for self-service password reset](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) before they can reset their passwords.</span></span> <span data-ttu-id="407fb-108">Pēc tam, kad lietotājs ir reģistrējies, viņš var izpildīt šajā rakstā sniegtos norādījumus, lai atiestatītu paroli: [darba vai skolas paroles](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)atiestatīšana.</span><span class="sxs-lookup"><span data-stu-id="407fb-108">Once a user has registered, they can follow the instructions in this article to reset their password: [Reset your work or school password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span></span>

<span data-ttu-id="407fb-109">**Kā mani lietotāji var mainīt savas paroles?**</span><span class="sxs-lookup"><span data-stu-id="407fb-109">**How do my users change their passwords?**</span></span>

<span data-ttu-id="407fb-110">Lietotāji var veikt šajā rakstā norādītās darbības, lai mainītu paroles: [kā mainīt paroli](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span><span class="sxs-lookup"><span data-stu-id="407fb-110">Users can follow the steps in this article to change their passwords: [How to change your password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span></span>
<span data-ttu-id="407fb-111">Tās var arī [pārvaldīt programmu paroles divsoļu pārbaudei](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span><span class="sxs-lookup"><span data-stu-id="407fb-111">They can also [Manage app passwords for two-step verification](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span></span>

<span data-ttu-id="407fb-112">**Mainot vai atiestatot paroli, mans lietotājs saņem kļūdas ziņojumu**</span><span class="sxs-lookup"><span data-stu-id="407fb-112">**My user is getting an error when changing or resetting their password**</span></span>

<span data-ttu-id="407fb-113">Šajā saitē būs sniegta informācija par bieži sastopamām problēmām, kas var rasties, ja lietotājs mēģina atiestatīt paroli: [biežāk sastopamās problēmas un to risinājumi](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span><span class="sxs-lookup"><span data-stu-id="407fb-113">This link will provide information on common problems that can arise when a user is trying to reset their password: [Common problems and their solutions](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span></span>

<span data-ttu-id="407fb-114">**Man radās problēma, atiestatot lietotāja paroli**</span><span class="sxs-lookup"><span data-stu-id="407fb-114">**I'm having a problem resetting a user's password**</span></span>

- <span data-ttu-id="407fb-115">Pārliecinieties, vai jums ir atļauts Atiestatīt paroles.</span><span class="sxs-lookup"><span data-stu-id="407fb-115">Make sure you are authorized to reset passwords.</span></span> <span data-ttu-id="407fb-116">*Tikai globālie, paroļu un lietotāju administratori var atiestatīt lietotāju paroles.*</span><span class="sxs-lookup"><span data-stu-id="407fb-116">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="407fb-117">Globālie administratori var arī atiestatīt citas privilēģijas administratora paroles.</span><span class="sxs-lookup"><span data-stu-id="407fb-117">Global administrators can also reset other privileged administrator's passwords.</span></span>

- <span data-ttu-id="407fb-118">Pārliecinieties, vai jums ir izpratne par licencēšanas prasībām:</span><span class="sxs-lookup"><span data-stu-id="407fb-118">Make sure you understand the licensing requirements:</span></span>

  - <span data-ttu-id="407fb-119">Jums ir jābūt vismaz vienai jūsu organizācijā piešķirtai licencei:</span><span class="sxs-lookup"><span data-stu-id="407fb-119">You must have at least one license assigned in your organization:</span></span>
    - <span data-ttu-id="407fb-120">**Tikai mākoņi** — visi Office 365 (O365) apmaksātie SKU vai Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="407fb-120">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="407fb-121">**Mākoņa un/vai Lokālie lietotāji** — Azure AD Premium P1 vai P2, Enterprise Mobility + Security (EMS) vai Secure ražīgs uzņēmums (SPE)</span><span class="sxs-lookup"><span data-stu-id="407fb-121">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="407fb-122">Papildinformāciju par licencēšanas prasībām skatiet rakstā Azure AD pašapkalpošanās [paroles atiestatīšanas licencēšanas prasības](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span><span class="sxs-lookup"><span data-stu-id="407fb-122">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span></span>
- <span data-ttu-id="407fb-123">Lai atiestatītu lietotāja paroli, atrodiet lietotāju Azure AD.</span><span class="sxs-lookup"><span data-stu-id="407fb-123">To reset a user's password, find the user in Azure AD.</span></span> <span data-ttu-id="407fb-124">Pēc tam šī lietotāja apskata asmenī noklikšķiniet uz pogas "Atiestatīt paroli".</span><span class="sxs-lookup"><span data-stu-id="407fb-124">Then, on the overview blade for that user, click the "reset password" button.</span></span>

<span data-ttu-id="407fb-125">**Paroles atiestatīšanas poga ir pelēkota**</span><span class="sxs-lookup"><span data-stu-id="407fb-125">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="407fb-126">Jūs neesat autorizēts **Šī** lietotāja paroļu atiestatīšanai.</span><span class="sxs-lookup"><span data-stu-id="407fb-126">You are not authorized to reset **this** user's passwords.</span></span> <span data-ttu-id="407fb-127">*Tikai globālie, paroļu un lietotāju administratori var atiestatīt lietotāju paroles.*</span><span class="sxs-lookup"><span data-stu-id="407fb-127">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="407fb-128">Globālie administratori var arī atiestatīt citas privilēģijas administratora paroles.</span><span class="sxs-lookup"><span data-stu-id="407fb-128">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="407fb-129">**Nav redzams paroles atiestatīšanas asmens**</span><span class="sxs-lookup"><span data-stu-id="407fb-129">**I don't see the password reset blade**</span></span>

<span data-ttu-id="407fb-130">Jūs neesat autorizēts, lai atiestatītu paroles.</span><span class="sxs-lookup"><span data-stu-id="407fb-130">You are not authorized to reset passwords.</span></span> <span data-ttu-id="407fb-131">*Tikai globālie, paroļu un lietotāju administratori var atiestatīt lietotāju paroles.*</span><span class="sxs-lookup"><span data-stu-id="407fb-131">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="407fb-132">Globālie administratori var arī atiestatīt citas privilēģijas administratora paroles.</span><span class="sxs-lookup"><span data-stu-id="407fb-132">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="407fb-133">**Paroles atiestatīšana nav redzama lokālā integrācijas asmens**</span><span class="sxs-lookup"><span data-stu-id="407fb-133">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="407fb-134">Lokālā integrācijas asmens tiek rādīts tikai hibrīdās vidēs — tas nozīmē, ka izmantojat paroļu arī atpakaļrakstīšanas, lai manipulētu ar lokālo lietotāju parolēm.</span><span class="sxs-lookup"><span data-stu-id="407fb-134">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>

- <span data-ttu-id="407fb-135">Šis asmens nav redzams, ja:</span><span class="sxs-lookup"><span data-stu-id="407fb-135">You do not see this blade if:</span></span>

  - <span data-ttu-id="407fb-136">Jūs neizmantojat paroļu arī atpakaļrakstīšanas</span><span class="sxs-lookup"><span data-stu-id="407fb-136">You are not using password writeback</span></span>
  - <span data-ttu-id="407fb-137">Ir radusies problēma ar jūsu paroļu arī atpakaļrakstīšanas instalāciju/savienojamību</span><span class="sxs-lookup"><span data-stu-id="407fb-137">There is a problem with your installation/connectivity of password writeback</span></span>
  - <span data-ttu-id="407fb-138">Ir radusies problēma ar Azure AD Connect instalēšanu/savienojamību</span><span class="sxs-lookup"><span data-stu-id="407fb-138">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
  - <span data-ttu-id="407fb-139">Papildinformāciju par problēmu novēršanu saistībā ar paroļu arī atpakaļrakstīšanas skatiet rakstā [paroļu arī atpakaļrakstīšanas problēmu novēršana](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="407fb-139">For more troubleshooting steps for issues with password writeback, see [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span></span>

<span data-ttu-id="407fb-140">**Es nezinu, kā atiestatīt lietotāja paroli**</span><span class="sxs-lookup"><span data-stu-id="407fb-140">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="407fb-141">Pierakstieties Azure portālā kā atbilstošs administrators.</span><span class="sxs-lookup"><span data-stu-id="407fb-141">Sign in to the Azure portal as an appropriate admin.</span></span>
2. <span data-ttu-id="407fb-142">Dodieties uz lapu **lietotāji un grupas** , atlasiet **Visi lietotāji**.</span><span class="sxs-lookup"><span data-stu-id="407fb-142">Go to the **Users and groups** blade, select **All Users**.</span></span>
3. <span data-ttu-id="407fb-143">Sarakstā atlasiet lietotāju.</span><span class="sxs-lookup"><span data-stu-id="407fb-143">Select a user from the list.</span></span>
4. <span data-ttu-id="407fb-144">Atlasītajam lietotājam atlasiet **pārskats** un pēc tam komandjoslā atlasiet **Atiestatīt paroli**.</span><span class="sxs-lookup"><span data-stu-id="407fb-144">For the selected user, select **Overview**, and then in the command bar, select **Reset password**.</span></span>
5. <span data-ttu-id="407fb-145">Atlasiet pogu **Atiestatīt paroli** un izpildiet ekrānā redzamos norādījumus.</span><span class="sxs-lookup"><span data-stu-id="407fb-145">Select the **Reset password** button and follow the instructions on the screen.</span></span>
    - <span data-ttu-id="407fb-146">Tiek atiestatīta tikai **Azure portāla** atbalsta paroles arī atpakaļrakstīšanas.</span><span class="sxs-lookup"><span data-stu-id="407fb-146">Only resets performed through the **Azure portal** support password writeback.</span></span>

<span data-ttu-id="407fb-147">**Atjaunoju lokālā lietotāja paroli no Office 365 administrēšanas portāla vai Office 365 mobilās lietojumprogrammas, taču lietotājs joprojām nevar pierakstīties**</span><span class="sxs-lookup"><span data-stu-id="407fb-147">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="407fb-148">Paroļu arī atpakaļrakstīšanas šajā portālā netiek atbalstīts.</span><span class="sxs-lookup"><span data-stu-id="407fb-148">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="407fb-149">Vēlreiz atiestatiet lietotāja paroli Azure portālā.</span><span class="sxs-lookup"><span data-stu-id="407fb-149">Reset the user's password again in the Azure portal.</span></span>
