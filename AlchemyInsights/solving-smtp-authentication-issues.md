---
title: SMTP autentifikācijas un problēmu novēršanas iespējošana
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077658"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a><span data-ttu-id="695aa-102">SMTP autentifikācijas un problēmu novēršanas iespējošana</span><span class="sxs-lookup"><span data-stu-id="695aa-102">Enable SMTP authentication and troubleshooting</span></span>

<span data-ttu-id="695aa-103">Ja vēlaties iespējot SMTP autentifikāciju pastkastei vai saņemat kļūdu "Klients nav autentificēts", "Autentifikācija nesekmīga" vai "SmtpClientAuthentication" ar kodu 5.7.57 vai 5.7.3 vai 5.7.139, kad mēģināt nosūtīt e-pasta ziņojumu, autentificējot ierīci vai lietojumprogrammu ar Microsoft 365, veiciet šīs trīs darbības, lai novērstu šo problēmu:</span><span class="sxs-lookup"><span data-stu-id="695aa-103">If you want to enable SMTP authentication for a mailbox or you're getting a "Client not authenticated", "Authentication unsuccessful", or "SmtpClientAuthentication" error with code 5.7.57 or 5.7.3 or 5.7.139 when you try to relay email by authenticating a device or application with Microsoft 365, perform these three actions to resolve the issue:</span></span>

1. <span data-ttu-id="695aa-104">Atspējojiet [Azure drošības noklusējumus,](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) izslēdzot opciju **Iespējot drošības noklusējumus** uz **Nē**.</span><span class="sxs-lookup"><span data-stu-id="695aa-104">Disable the [Azure security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) by toggling **Enable security defaults** to **No**.</span></span>

    <span data-ttu-id="695aa-105">a.</span><span class="sxs-lookup"><span data-stu-id="695aa-105">a.</span></span> <span data-ttu-id="695aa-106">Pierakstieties Azure portālā kā drošības administrators, nosacījum piekļuves administrators vai globālais administrators.</span><span class="sxs-lookup"><span data-stu-id="695aa-106">Sign in to the Azure portal as a Security administrator, Conditional Access administrator, or global administrator.</span></span><BR/>
    <span data-ttu-id="695aa-107">b.</span><span class="sxs-lookup"><span data-stu-id="695aa-107">b.</span></span> <span data-ttu-id="695aa-108">Pārlūkojot atrodiet Azure Active Directory > **rekvizīti.**</span><span class="sxs-lookup"><span data-stu-id="695aa-108">Browse to Azure Active Directory > **Properties**.</span></span><BR/>
    <span data-ttu-id="695aa-109">c.</span><span class="sxs-lookup"><span data-stu-id="695aa-109">c.</span></span> <span data-ttu-id="695aa-110">Atlasiet **Pārvaldīt drošības noklusējumus**.</span><span class="sxs-lookup"><span data-stu-id="695aa-110">Select **Manage security defaults**.</span></span><BR/>
    <span data-ttu-id="695aa-111">d.</span><span class="sxs-lookup"><span data-stu-id="695aa-111">d.</span></span> <span data-ttu-id="695aa-112">Iestatiet **Iespējot drošības noklusējumus** **uz Nē**.</span><span class="sxs-lookup"><span data-stu-id="695aa-112">Set **Enable security defaults** to **No**.</span></span><BR/>
    <span data-ttu-id="695aa-113">e.</span><span class="sxs-lookup"><span data-stu-id="695aa-113">e.</span></span> <span data-ttu-id="695aa-114">Atlasiet **Saglabāt**.</span><span class="sxs-lookup"><span data-stu-id="695aa-114">Select **Save**.</span></span>

2. <span data-ttu-id="695aa-115">[Licencētajā pastkastē iespējojiet](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) klienta SMTP iesniegšanu.</span><span class="sxs-lookup"><span data-stu-id="695aa-115">[Enable Client SMTP submission](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) on the licensed mailbox.</span></span>

    <span data-ttu-id="695aa-116">a.</span><span class="sxs-lookup"><span data-stu-id="695aa-116">a.</span></span> <span data-ttu-id="695aa-117">Izvēlnē Microsoft 365 administrēšanas centrs dodieties **uz Aktīvie** lietotāji un atlasiet lietotāju.</span><span class="sxs-lookup"><span data-stu-id="695aa-117">From the Microsoft 365 admin center, go to **Active Users**, and select the user.</span></span><BR/>
    <span data-ttu-id="695aa-118">b.</span><span class="sxs-lookup"><span data-stu-id="695aa-118">b.</span></span> <span data-ttu-id="695aa-119">Dodieties uz cilni Pasts un sadaļā **E-pasta programmas** atlasiet Pārvaldīt **e-pasta programmas**.</span><span class="sxs-lookup"><span data-stu-id="695aa-119">Go to Mail tab, and under **Email apps**, select **Manage email apps**.</span></span><BR/>
    <span data-ttu-id="695aa-120">d.</span><span class="sxs-lookup"><span data-stu-id="695aa-120">d.</span></span> <span data-ttu-id="695aa-121">**Pārliecinieties, vai ir atzīmēta** opcija Autentificēts SMTP (iespējots).</span><span class="sxs-lookup"><span data-stu-id="695aa-121">Make sure **Authenticated SMTP** is checked (enabled).</span></span><BR/>
    <span data-ttu-id="695aa-122">e.</span><span class="sxs-lookup"><span data-stu-id="695aa-122">e.</span></span> <span data-ttu-id="695aa-123">Atlasiet **Saglabāt izmaiņas**.</span><span class="sxs-lookup"><span data-stu-id="695aa-123">Select **Save changes**.</span></span><BR/>

3. <span data-ttu-id="695aa-124">[Atspējojiet daudzfaktors autentifikācijas (multi-Factor Authentication — MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) licencētajā pastkastē.</span><span class="sxs-lookup"><span data-stu-id="695aa-124">[Disable Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) on the licensed mailbox.</span></span>

    <span data-ttu-id="695aa-125">a.</span><span class="sxs-lookup"><span data-stu-id="695aa-125">a.</span></span> <span data-ttu-id="695aa-126">Dodieties uz Microsoft 365 administrēšanas centrs un kreisajā navigācijas izvēlnē **atlasiet** Lietotāji  >  **Aktīvie lietotāji**.</span><span class="sxs-lookup"><span data-stu-id="695aa-126">Go to the Microsoft 365 admin center, and in the left navigation menu select **Users** > **Active users**.</span></span><BR/>
    <span data-ttu-id="695aa-127">b.</span><span class="sxs-lookup"><span data-stu-id="695aa-127">b.</span></span> <span data-ttu-id="695aa-128">Atlasiet **Daudzfaktors autentifikācija**.</span><span class="sxs-lookup"><span data-stu-id="695aa-128">Select **Multi-factor authentication**.</span></span><BR/>
    <span data-ttu-id="695aa-129">c.</span><span class="sxs-lookup"><span data-stu-id="695aa-129">c.</span></span> <span data-ttu-id="695aa-130">Atlasiet lietotāju un atspējojiet **Daudzfaktors autentifikāciju**.</span><span class="sxs-lookup"><span data-stu-id="695aa-130">Select the user and disable **Multi-Factor auth**.</span></span><BR/>
