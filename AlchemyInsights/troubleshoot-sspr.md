---
title: SSPR problēmu novēršana
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430222"
---
# <a name="troubleshoot-sspr"></a><span data-ttu-id="1eb2c-102">SSPR problēmu novēršana</span><span class="sxs-lookup"><span data-stu-id="1eb2c-102">Troubleshoot SSPR</span></span>

<span data-ttu-id="1eb2c-103">**Radās problēmas, konfigurējot paroles atiestatīšanu**</span><span class="sxs-lookup"><span data-stu-id="1eb2c-103">**I'm having trouble configuring password reset**</span></span>

- <span data-ttu-id="1eb2c-104">Ja esat administrators un meklējat, kā iespējot pašapkalpošanās paroles atiestatīšanu, skatiet rakstu [apmācība IESPĒJOT SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), lai konfigurētu paroles atiestatīšanu savai organizācijai.</span><span class="sxs-lookup"><span data-stu-id="1eb2c-104">If you are administrator and looking for how to enable self-service password reset, see [Tutorial enable SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), to configure password reset for your organization.</span></span> <span data-ttu-id="1eb2c-105">Jūs, iespējams, vēlēsities pārskatīt [licencēšanas prasības](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="1eb2c-105">You may also want to review the [licensing requirements](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span> <span data-ttu-id="1eb2c-106">Jūsu organizācijā jābūt piešķirtai vismaz vienai licencei.</span><span class="sxs-lookup"><span data-stu-id="1eb2c-106">You must have at least one license assigned in your organization.</span></span>
    - <span data-ttu-id="1eb2c-107">**Tikai mākoņi** — visi Office 365 (O365) apmaksātie SKU vai Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="1eb2c-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="1eb2c-108">**Mākoņa un/vai Lokālie lietotāji** — Azure AD Premium P1 vai P2, Enterprise Mobility + Security (EMS) vai Secure ražīgs uzņēmums (SPE)</span><span class="sxs-lookup"><span data-stu-id="1eb2c-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
- <span data-ttu-id="1eb2c-109">Lai saņemtu papildu jautājumus par pašapkalpošanās paroles atiestatīšanu, pārskatiet [mūsu bieži uzdotie jautājumi](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="1eb2c-109">For additional questions about self-service password reset, review [our FAQ](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="1eb2c-110">**Saņemu kļūdas ziņojumu**</span><span class="sxs-lookup"><span data-stu-id="1eb2c-110">**I'm getting an error message**</span></span>

<span data-ttu-id="1eb2c-111">Izlasiet šo rakstu, lai atrastu biežāk sastopamās kļūdas un to risinājumus: problēmu novēršana pašapkalpošanās [paroles atiestatīšanai](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="1eb2c-111">Review this article to find common errors and their solutions: [Troubleshoot self-service password reset](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="1eb2c-112">**Man radās problēma ar paroles atiestatīšanas politiku**</span><span class="sxs-lookup"><span data-stu-id="1eb2c-112">**I'm having a problem with my password reset policy**</span></span>

- <span data-ttu-id="1eb2c-113">Ja paroles atiestatīšanas politika nedarbojas, kā paredzēts, vai jums ir jautājumi par paroļu atiestatīšanas politikām, pārskatiet šo rakstu: [paroļu politikas un ierobežojumi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="1eb2c-113">If your password reset policy is not behaving as expected, or if you have questions about password reset policies, review this article: [Password policies and restrictions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="1eb2c-114">Paroļu atiestatīšanas politikas neattiecas uz administratoriem.</span><span class="sxs-lookup"><span data-stu-id="1eb2c-114">Password reset policies do not apply to administrators.</span></span> <span data-ttu-id="1eb2c-115">Microsoft ievieš spēcīgu noklusējuma divu vārtu paroles atiestatīšanas politiku jebkurai Azure administratora lomai.</span><span class="sxs-lookup"><span data-stu-id="1eb2c-115">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role.</span></span> <span data-ttu-id="1eb2c-116">Pārliecinieties, vai testējat lietotāju, kurš nav administrators.</span><span class="sxs-lookup"><span data-stu-id="1eb2c-116">Make sure that you are testing with a user who is not an administrator.</span></span> <span data-ttu-id="1eb2c-117">Papildinformāciju par administratoru atiestatīšanas politiku skatiet šajā rakstā: [administrators atiestatiet politikas atšķirības](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).</span><span class="sxs-lookup"><span data-stu-id="1eb2c-117">For more information on the administrator reset policy, see this article: [Administrator reset policy differences](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).</span></span>

<span data-ttu-id="1eb2c-118">**Nevēlos, lai lietotāji reģistrētu papildu drošības informāciju paroles atiestatīšanai**</span><span class="sxs-lookup"><span data-stu-id="1eb2c-118">**I don't want my users to register additional security info for password reset**</span></span>

<span data-ttu-id="1eb2c-119">Jūs varat iepriekš aizpildīt datus (e-pastu un tālruņa atribūtus) saviem lietotājiem, izmantojot API, PowerShell vai Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="1eb2c-119">You can pre-populate data (email and phone attributes) for your users using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="1eb2c-120">Lai uzzinātu, kā lasīt:</span><span class="sxs-lookup"><span data-stu-id="1eb2c-120">To learn how read:</span></span>

- [<span data-ttu-id="1eb2c-121">Paroles atiestatīšanas izvietošana bez nepieciešamības lietotājiem reģistrēties</span><span class="sxs-lookup"><span data-stu-id="1eb2c-121">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [<span data-ttu-id="1eb2c-122">Kādus datus izmanto paroles atiestatīšana</span><span class="sxs-lookup"><span data-stu-id="1eb2c-122">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="1eb2c-123">**Vēlos, lai lietotāji reģistrētu savu papildu drošības informāciju paroles atiestatīšanai**</span><span class="sxs-lookup"><span data-stu-id="1eb2c-123">**I want my users to register their additional security info for password reset**</span></span>

1. <span data-ttu-id="1eb2c-124">Lieciet lietotājiem reģistrēt savu drošības informāciju par pašapkalpošanās paroles atiestatīšanu, novirzot tos uz [aka.MS/ssprsetup](https://mysignins.microsoft.com/security-info).</span><span class="sxs-lookup"><span data-stu-id="1eb2c-124">Have your users register their security info for self service password reset by directing them to [aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info).</span></span>
1. <span data-ttu-id="1eb2c-125">Pēc tam, kad dati ir aizpildīti lietotājam (lietotājs vai administrators), virziet lietotāju uz [aka.MS/sspr](https://passwordreset.microsoftonline.com/) , lai jūsu lietotāji varētu būt pilnvaroti atiestatīt savas paroles.</span><span class="sxs-lookup"><span data-stu-id="1eb2c-125">After data is populated for the user (by the user or by the admin), direct your user to [aka.ms/sspr](https://passwordreset.microsoftonline.com/) so your users can be empowered to reset their own passwords.</span></span>
1. <span data-ttu-id="1eb2c-126">Ja lietotāji joprojām saskaras ar problēmām, kas var būt **izplatītākie** vai **paroļu hashi sinhronizētie** lietotāji.</span><span class="sxs-lookup"><span data-stu-id="1eb2c-126">If users are still experiencing problems they are most likely **federated** or **password hash synched** users.</span></span> <span data-ttu-id="1eb2c-127">Tas nozīmē, ka ir iespējamas problēmas ar paroļu arī atpakaļrakstīšanas pakalpojumu.</span><span class="sxs-lookup"><span data-stu-id="1eb2c-127">This means there is likely a problem with the Password Writeback service.</span></span>