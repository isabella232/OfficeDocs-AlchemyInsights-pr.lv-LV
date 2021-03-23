---
title: Es saņemu bloķētu piekļuvi, izmantojot domēna pieslēgto ierīci
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/20/2021
ms.locfileid: "51036701"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a><span data-ttu-id="2404d-102">Es saņemu bloķētu piekļuvi, izmantojot domēna pieslēgto ierīci</span><span class="sxs-lookup"><span data-stu-id="2404d-102">I’m getting blocked by Conditional Access with domain joined device</span></span>

<span data-ttu-id="2404d-103">**Ļoti Ieteicamie rīki**</span><span class="sxs-lookup"><span data-stu-id="2404d-103">**Highly Recommended Tools**</span></span>

<span data-ttu-id="2404d-104">[Ierīču reģistrācijas problēmu risinātāja rīks](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) — rīks, kas palīdz novērst izplatītākās ierīču reģistrācijas problēmas.</span><span class="sxs-lookup"><span data-stu-id="2404d-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - The tool that helps in troubleshooting the most common device registration issues.</span></span>

<span data-ttu-id="2404d-105">[Testa ierīces reģistrācijas savienojamības skripts](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) — skripts, kas nodrošina, ka ierīce var piekļūt ierīces reģistrācijas galapunktiem sistēmas kontā.</span><span class="sxs-lookup"><span data-stu-id="2404d-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - The script that helps ensuring that a device can access Device Registration endpoints under the system account.</span></span>

<span data-ttu-id="2404d-106">[AZURE ad Device cleanup skripts](https://github.com/mzmaili/AzureADDeviceCleanup) — skripts, kas sniedz iespēju meklēt un pārvaldīt novecojušas ierīces savā vidē.</span><span class="sxs-lookup"><span data-stu-id="2404d-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - The script that enables you to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="2404d-107">Tālāk ir norādīti daži raksturīgākie iemesli, kāpēc Nosacījumformatēšana var bojāt ierīci, kas ir savienota ar domēnu (hibrīdais Azure AD).</span><span class="sxs-lookup"><span data-stu-id="2404d-107">Here are some common reasons why conditional access may be failing a device that has joined a domain (Hybrid Azure AD).</span></span>

1. <span data-ttu-id="2404d-108">**Ierīcē nav AZURE ad PRT** , ir jāpārliecinās, vai ierīcei ir Azure AD primārās atsvaidzināšanas pilnvara (PRT).</span><span class="sxs-lookup"><span data-stu-id="2404d-108">**There’s no Azure AD PRT on the device** - You need to ensure that the device has Azure AD Primary Refresh Token (PRT).</span></span> <span data-ttu-id="2404d-109">Papildinformāciju par PRT skatiet šajā [dokumentā](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="2404d-109">For more information about PRT, see this [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="2404d-110">Lai pārbaudītu, vai jums ir Azure AD PRT, varat izpildīt `dsregcmd/status` ierīces komandu un pārbaudīt, vai "AzureAdPrt" ir vienāds ar "Jā".</span><span class="sxs-lookup"><span data-stu-id="2404d-110">To verify if you have Azure AD PRT, you can run `dsregcmd/status` command on the device and verify if “AzureAdPrt” equals “YES”.</span></span>

<span data-ttu-id="2404d-111">Ja "AzureAdPrt" ir "nē", pārbaudiet tālāk norādīto informāciju.</span><span class="sxs-lookup"><span data-stu-id="2404d-111">If "AzureAdPrt" is "NO", check the following:</span></span>

- <span data-ttu-id="2404d-112">**Neatkarīgi no tā, vai jums ir ārēja vide ar AD FS, un tas nav sasniedzams no lietotāju mājas tīkliem**: šajā gadījumā pārliecinieties, vai jūsu "usernamemixed" galapunkti ir pieejami no ārtīkla.</span><span class="sxs-lookup"><span data-stu-id="2404d-112">**Whether you have a federated environment with AD FS, and it’s unreachable from your users’ home networks**: In this case, ensure that your "usernamemixed" endpoints are accessible from the extranet.</span></span> <span data-ttu-id="2404d-113">Ja jūsu AD FS ir fonā, pārliecinieties, vai lietotāji izveido savienojumu ar VPN un atkārtoti pieteicies ierīcē.</span><span class="sxs-lookup"><span data-stu-id="2404d-113">If your AD FS is behind a VPN, ensure that the users connect to the VPN and re-login to the device.</span></span> <span data-ttu-id="2404d-114">Lai iegūtu papildinformāciju, skatiet šo [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span><span class="sxs-lookup"><span data-stu-id="2404d-114">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span></span>

- <span data-ttu-id="2404d-115">Neatkarīgi no tā, **vai ierīces TPM ir kļūdains, tāpēc nevar autentificēt ierīci**: Check "TPM. msc", lai noskaidrotu, vai TPM statuss ir gatavs.</span><span class="sxs-lookup"><span data-stu-id="2404d-115">**Whether the device’s TPM is faulty and thus cannot authenticate the device**: Check "tpm.msc" to see if the state of TPM is "Ready".</span></span> <span data-ttu-id="2404d-116">Ja nav, palaidiet `dsregcmd/leave` un ļaujiet ierīcei atkārtoti pievienoties pakalpojumam AZURE ad.</span><span class="sxs-lookup"><span data-stu-id="2404d-116">If not, run `dsregcmd/leave` and let the device re-join to Azure AD.</span></span> <span data-ttu-id="2404d-117">Pēc tam mēģiniet vēlreiz.</span><span class="sxs-lookup"><span data-stu-id="2404d-117">Then, try again.</span></span> <span data-ttu-id="2404d-118">Lai iegūtu papildinformāciju, skatiet šo [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span><span class="sxs-lookup"><span data-stu-id="2404d-118">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>

- <span data-ttu-id="2404d-119">**Jūs izmantojat trešo personu identitātes pakalpojumu sniedzēju, kas neatbalsta WS-Trust protokolu**.</span><span class="sxs-lookup"><span data-stu-id="2404d-119">**You’re using a 3rd party identity provider, which does not support WS-Trust protocol**.</span></span> <span data-ttu-id="2404d-120">Kā aprakstīts mūsu dokumentos, hibrīdās Azure AD-Savienotās ierīces nevar darboties šajā gadījumā.</span><span class="sxs-lookup"><span data-stu-id="2404d-120">As described in our docs, hybrid Azure AD-joined devices cannot work in this case.</span></span> <span data-ttu-id="2404d-121">Lai saņemtu atbalstu, lūdzu, sazinieties ar savu identitātes nodrošinātāju.</span><span class="sxs-lookup"><span data-stu-id="2404d-121">Please work with your Identity provider for support.</span></span>

2. <span data-ttu-id="2404d-122">**Lietotāji izmanto Chrome pārlūkprogrammu bez Windows 10 kontiem** vai **Office Extension Chrome automātiski neizmanto PRT ar AAD-savienotām vai hibrīdām ierīcēm**: tas rada jebkādas ierīces, kuru pamatā ir ierobežotas piekļuves politikas, tiek parādīts kļūdas ziņojums "nereģistrēta ierīce".</span><span class="sxs-lookup"><span data-stu-id="2404d-122">**Users are using Chrome browser without the Windows 10 Accounts** or **Office extension Chrome does not automatically use the PRT on AAD-joined or hybrid-AAD-joined devices**: This leads to failure of any device-based Conditional Access policies, with “Unregistered device” error message displayed.</span></span> <span data-ttu-id="2404d-123">Lai pareizi izmantotu Chrome pārlūkprogrammu, ir jāinstalē Windows 10 konti vai Office paplašinājums lietotāju Chrome pārlūkprogrammā, izmantojot SCCM vai Intune.</span><span class="sxs-lookup"><span data-stu-id="2404d-123">To use Chrome browser correctly, you must install the “Windows 10 Accounts” or "Office extension to the users’ Chrome browser" via SCCM or Intune.</span></span> <span data-ttu-id="2404d-124">Lai iegūtu papildinformāciju, skatiet šo [dokumentu](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span><span class="sxs-lookup"><span data-stu-id="2404d-124">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

<span data-ttu-id="2404d-125">Ja nav iespējams veikt pagarinājumu attālināti, informējiet lietotājus par to, ka manuāli jāinstalē kāds no iepriekš norādītajiem paplašinājumiem, lai piekļūtu lietojumprogrammas, kuru pamatā ir ierīces piekļuve.</span><span class="sxs-lookup"><span data-stu-id="2404d-125">If it’s not possible to push the extension remotely, notify users to manually install one of the above extensions to access applications behind device-based Conditional Access.</span></span> <span data-ttu-id="2404d-126">Lai iegūtu papildinformāciju, skatiet šo [dokumentu](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span><span class="sxs-lookup"><span data-stu-id="2404d-126">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span></span>

3. <span data-ttu-id="2404d-127">**Ierīce bija pareizi pievienota Hibrīdā AZURE AD, bet tā ir nejauši izdzēsta vai atspējota, vai nu sakarā ar sinhronizācijas izmaiņām AZURE ad Connect vai Azure portālā**: ja tā notiek, ierīces objekts vairs netiek atpazīts kā pilnībā pievienota ierīce, lai gan "AzureAdJoined", gan "PRT" statuss ierīcē tiek rādīts kā derīgs.</span><span class="sxs-lookup"><span data-stu-id="2404d-127">**The device was correctly hybrid Azure AD joined, but it was inadvertently deleted or disabled, either due to sync changes in Azure AD Connect or from the Azure portal**: If this happens, the device object is no longer recognized as a fully joined device even though the "AzureAdJoined" and "PRT" status show up as valid on the device.</span></span>

<span data-ttu-id="2404d-128">Lai novērstu šo problēmu, palaidiet `dsregcmd/leave` ietekmētās ierīces un atdodiet tās AZURE ad.</span><span class="sxs-lookup"><span data-stu-id="2404d-128">To fix this issue, run `dsregcmd/leave` on the affected devices and let them rejoin Azure AD.</span></span> <span data-ttu-id="2404d-129">Lai iegūtu papildinformāciju, skatiet šo [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span><span class="sxs-lookup"><span data-stu-id="2404d-129">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span></span>

> [!NOTE]
> <span data-ttu-id="2404d-130">Ja jūsu ierīces darbojas operētājsistēmā Windows 10, 1809 atjauninājums ar VPN/Cloud starpniekserveri un redzamas problēmas ar "AzureAdPrt" vai kādu programmu ar SSO problēmu (Outlook neveido savienojumu ar pastkasti pat tad, ja ir bijusi PRT), pārliecinieties, vai jums ir šis plāksteris [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) vai aprīļa kumulatīvās atjaunināšanas [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) , lai novērstu PRT nepilnības šajos datoros.</span><span class="sxs-lookup"><span data-stu-id="2404d-130">If your devices are on Windows 10, 1809 update, with VPN/Cloud Proxy and see issues with "AzureAdPrt" state or any app with SSO problem (outlook not connecting to mailbox even though you had PRT), ensure you have this patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) or April cumulative update [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) to prevent PRT failures on those machines.</span></span>

















