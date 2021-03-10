---
title: Problēmas atiestatot paroli
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694379"
---
# <a name="problems-resetting-password"></a><span data-ttu-id="750de-102">Problēmas atiestatot paroli</span><span class="sxs-lookup"><span data-stu-id="750de-102">Problems resetting password</span></span>

<span data-ttu-id="750de-103">Tālāk norādītas dažas problēmas, kas var rasties, atiestatot paroli un iespējamos risinājumus:</span><span class="sxs-lookup"><span data-stu-id="750de-103">Following are some of the issues that you might face when resetting password and the possible solutions:</span></span>

<span data-ttu-id="750de-104">**Man ir problēma ar paroles atiestatīšanu, kas nav iekļauta citās kategorijās**</span><span class="sxs-lookup"><span data-stu-id="750de-104">**I'm having an issue with password reset not covered in the other categories**</span></span>

- <span data-ttu-id="750de-105">Pārliecinieties, vai jums ir atļauts Atiestatīt paroles.</span><span class="sxs-lookup"><span data-stu-id="750de-105">Ensure you are authorized to reset passwords.</span></span> <span data-ttu-id="750de-106">Tikai globālie, paroļu un lietotāju administratori var atiestatīt lietotāju paroles.</span><span class="sxs-lookup"><span data-stu-id="750de-106">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="750de-107">Globālie administratori var arī atiestatīt citas privilēģijas administratora paroles.</span><span class="sxs-lookup"><span data-stu-id="750de-107">Global administrators can also reset other privileged administrator's passwords.</span></span>
- <span data-ttu-id="750de-108">Pārliecinieties, vai jums ir izpratne par licencēšanas prasībām:</span><span class="sxs-lookup"><span data-stu-id="750de-108">Ensure that you understand the licensing requirements:</span></span>
    - <span data-ttu-id="750de-109">Jums ir nepieciešama vismaz viena licence, kas piešķirta jūsu organizācijā</span><span class="sxs-lookup"><span data-stu-id="750de-109">You must have at least one license assigned in your organization</span></span>
        - <span data-ttu-id="750de-110">Tikai mākoņi — visi Office 365 (O365) apmaksātie SKU vai Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="750de-110">Cloud only users - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
        - <span data-ttu-id="750de-111">Mākoņa un/vai Lokālie lietotāji — Azure AD Premium P1 vai P2, Enterprise Mobility + Security (EMS) vai Secure ražīgs uzņēmums (SPE)</span><span class="sxs-lookup"><span data-stu-id="750de-111">Cloud and/or on-premises users - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
        - <span data-ttu-id="750de-112">Papildinformāciju par licencēšanas prasībām skatiet rakstā Azure AD pašapkalpošanās [paroles atiestatīšanas licencēšanas prasības](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="750de-112">To read more about licensing requirements see the article [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="750de-113">**Man ir problēmas ar iestatītās paroles atiestatīšanas politikas testēšanu**</span><span class="sxs-lookup"><span data-stu-id="750de-113">**I'm having problems testing the password reset policy I set**</span></span>

- <span data-ttu-id="750de-114">Nesen lietotās politikas var ilgt vairākas minūtes, lai tās atdarinātu visos datu centros un galapunktos.</span><span class="sxs-lookup"><span data-stu-id="750de-114">Recently applied policies can take several minutes to replicate across all data centers and end-points.</span></span> <span data-ttu-id="750de-115">Arī fiziskais attālums no datu centra ietekmēs, cik ātri izmaiņas tiek lietotas.</span><span class="sxs-lookup"><span data-stu-id="750de-115">Physical distance from the data center will also affect how quickly changes are applied.</span></span>
- <span data-ttu-id="750de-116">Testējiet ar lietotāju, nevis administratoru un pilots ar nelielu lietotāju kopu.</span><span class="sxs-lookup"><span data-stu-id="750de-116">Test with an end user, not an administrator, and pilot with a small set of users.</span></span> <span data-ttu-id="750de-117">Azure portālā konfigurētās politikas attiecas tikai uz lietotājiem, nevis administratoriem.</span><span class="sxs-lookup"><span data-stu-id="750de-117">The policies configured in the Azure portal ONLY apply to end-users, not administrators.</span></span> <span data-ttu-id="750de-118">Microsoft ievieš spēcīgu noklusējuma divu vārtu paroles atiestatīšanas politiku jebkurai Azure administratora lomai (piemēram: globālā administratora, palīdzības dienesta administrators, paroļu administrators utt.)</span><span class="sxs-lookup"><span data-stu-id="750de-118">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role (Example: Global Administrator, Helpdesk Administrator, Password Administrator, etc.)</span></span>
    - <span data-ttu-id="750de-119">Uzziniet vairāk par [administratoru politikām](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span><span class="sxs-lookup"><span data-stu-id="750de-119">Learn more about [policies for administrators](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span></span>

<span data-ttu-id="750de-120">**Es vēlos izvietot paroles atiestatīšanu, bet nevēlos, lai lietotāji reģistrētu papildu drošības informāciju**</span><span class="sxs-lookup"><span data-stu-id="750de-120">**I want to deploy password reset but I don't want to make my users register additional security info**</span></span>

<span data-ttu-id="750de-121">Iepriekš aizpildiet datus saviem lietotājiem, lai tiem nebūtu!</span><span class="sxs-lookup"><span data-stu-id="750de-121">Pre-populate data for your users so they don't have to!</span></span> <span data-ttu-id="750de-122">-Kā administrators varat iestatīt tālruņa un e-pasta rekvizītus saviem lietotājiem, pirms izlaižat paroles atiestatīšanu savai organizācijai.</span><span class="sxs-lookup"><span data-stu-id="750de-122">- As an administrator you can set phone and email properties for your users before rolling out password reset to your organization.</span></span> <span data-ttu-id="750de-123">To var izdarīt, izmantojot API, PowerShell vai Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="750de-123">You can do this using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="750de-124">Papildinformācija šeit:</span><span class="sxs-lookup"><span data-stu-id="750de-124">More information here:</span></span>
- [<span data-ttu-id="750de-125">Paroles atiestatīšanas izvietošana bez nepieciešamības lietotājiem reģistrēties</span><span class="sxs-lookup"><span data-stu-id="750de-125">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [<span data-ttu-id="750de-126">Kādus datus izmanto paroles atiestatīšana</span><span class="sxs-lookup"><span data-stu-id="750de-126">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="750de-127">**Paroles atiestatīšanas poga ir pelēkota**</span><span class="sxs-lookup"><span data-stu-id="750de-127">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="750de-128">Jūs neesat autorizēts šī lietotāja paroļu atiestatīšanai.</span><span class="sxs-lookup"><span data-stu-id="750de-128">You are not authorized to reset this user's passwords.</span></span> <span data-ttu-id="750de-129">Tikai globālie, paroļu un lietotāju administratori var atiestatīt lietotāju paroles.</span><span class="sxs-lookup"><span data-stu-id="750de-129">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="750de-130">Globālie administratori var arī atiestatīt citas privilēģijas administratora paroles.</span><span class="sxs-lookup"><span data-stu-id="750de-130">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="750de-131">**Nav redzams paroles atiestatīšanas asmens**</span><span class="sxs-lookup"><span data-stu-id="750de-131">**I don't see the password reset blade**</span></span>

<span data-ttu-id="750de-132">Jūs neesat autorizēts, lai atiestatītu paroles.</span><span class="sxs-lookup"><span data-stu-id="750de-132">You are not authorized to reset passwords.</span></span> <span data-ttu-id="750de-133">Tikai globālie, paroļu un lietotāju administratori var atiestatīt lietotāju paroles.</span><span class="sxs-lookup"><span data-stu-id="750de-133">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="750de-134">Globālie administratori var arī atiestatīt citas privilēģijas administratora paroles.</span><span class="sxs-lookup"><span data-stu-id="750de-134">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="750de-135">**Paroles atiestatīšana nav redzama lokālā integrācijas asmens**</span><span class="sxs-lookup"><span data-stu-id="750de-135">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="750de-136">Lokālā integrācijas asmens tiek rādīts tikai hibrīdās vidēs — tas nozīmē, ka izmantojat paroļu arī atpakaļrakstīšanas, lai manipulētu ar lokālo lietotāju parolēm.</span><span class="sxs-lookup"><span data-stu-id="750de-136">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>
- <span data-ttu-id="750de-137">Šis asmens nav redzams, ja:</span><span class="sxs-lookup"><span data-stu-id="750de-137">You do not see this blade if:</span></span>
    - <span data-ttu-id="750de-138">Jūs neizmantojat paroļu arī atpakaļrakstīšanas</span><span class="sxs-lookup"><span data-stu-id="750de-138">You are not using password writeback</span></span>
    - <span data-ttu-id="750de-139">Ir radusies problēma ar jūsu paroļu arī atpakaļrakstīšanas instalāciju/savienojamību</span><span class="sxs-lookup"><span data-stu-id="750de-139">There is a problem with your installation/connectivity of password writeback</span></span>
    - <span data-ttu-id="750de-140">Ir radusies problēma ar Azure AD Connect instalēšanu/savienojamību</span><span class="sxs-lookup"><span data-stu-id="750de-140">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
    - <span data-ttu-id="750de-141">Papildinformāciju par problēmu novēršanu saistībā ar paroļu arī atpakaļrakstīšanas skatiet sadaļā [problēmu novēršana paroļu arī atpakaļrakstīšanas](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="750de-141">For more troubleshooting steps for issues with password writeback, see the section [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="750de-142">**Es nezinu, kā atiestatīt lietotāja paroli**</span><span class="sxs-lookup"><span data-stu-id="750de-142">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="750de-143">Pierakstieties Azure portālā kā atbilstošs administrators.</span><span class="sxs-lookup"><span data-stu-id="750de-143">Sign in to the Azure portal as an appropriate admin.</span></span>
1. <span data-ttu-id="750de-144">Dodieties uz lapu lietotāji un grupas, atlasiet **Visi lietotāji**.</span><span class="sxs-lookup"><span data-stu-id="750de-144">Go to the Users and groups blade, select **All Users**.</span></span>
1. <span data-ttu-id="750de-145">Sarakstā atlasiet lietotāju.</span><span class="sxs-lookup"><span data-stu-id="750de-145">Select a user from the list.</span></span>
1. <span data-ttu-id="750de-146">Atlasītajam lietotājam atlasiet **pārskats** un pēc tam komandjoslā noklikšķiniet uz **Atiestatīt paroli**.</span><span class="sxs-lookup"><span data-stu-id="750de-146">For the selected user, select **Overview**, and then in the command bar, click **Reset password**.</span></span>
1. <span data-ttu-id="750de-147">Izpildiet ekrānā redzamos norādījumus.</span><span class="sxs-lookup"><span data-stu-id="750de-147">Follow the instructions on the screen.</span></span>
    - <span data-ttu-id="750de-148">Tiek atiestatīta tikai Azure portāla atbalsta paroles arī atpakaļrakstīšanas.</span><span class="sxs-lookup"><span data-stu-id="750de-148">Only resets performed through the Azure portal support password writeback.</span></span>

<span data-ttu-id="750de-149">**Atjaunoju lokālā lietotāja paroli no Office 365 administrēšanas portāla vai Office 365 mobilās lietojumprogrammas, taču lietotājs joprojām nevar pierakstīties**</span><span class="sxs-lookup"><span data-stu-id="750de-149">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="750de-150">Paroļu arī atpakaļrakstīšanas šajā portālā netiek atbalstīts.</span><span class="sxs-lookup"><span data-stu-id="750de-150">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="750de-151">Vēlreiz atiestatiet lietotāja paroli Azure portālā-portal.azure.com</span><span class="sxs-lookup"><span data-stu-id="750de-151">Reset the user's password again in the Azure portal - portal.azure.com</span></span>

