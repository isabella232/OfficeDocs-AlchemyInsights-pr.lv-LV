---
title: Paroļu arī atpakaļrakstīšanas nedarbojas
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
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243515"
---
# <a name="password-writeback-is-not-working"></a><span data-ttu-id="37220-102">Paroļu arī atpakaļrakstīšanas nedarbojas</span><span class="sxs-lookup"><span data-stu-id="37220-102">Password Writeback is not working</span></span>

<span data-ttu-id="37220-103">**Man rodas problēmas, konfigurējot paroļu arī atpakaļrakstīšanas**</span><span class="sxs-lookup"><span data-stu-id="37220-103">**I'm having problems configuring password writeback**</span></span>

- <span data-ttu-id="37220-104">Paroļu arī atpakaļrakstīšanas ir Premium līdzeklis.</span><span class="sxs-lookup"><span data-stu-id="37220-104">Password writeback is a premium feature.</span></span>
- <span data-ttu-id="37220-105">Pārliecinieties, vai jums ir izpratne par licencēšanas prasībām:</span><span class="sxs-lookup"><span data-stu-id="37220-105">Make sure that you understand the licensing requirements:</span></span>
  - <span data-ttu-id="37220-106">Jums ir nepieciešama vismaz viena licence, kas piešķirta jūsu organizācijā</span><span class="sxs-lookup"><span data-stu-id="37220-106">You must have at least one license assigned in your organization</span></span>
  - <span data-ttu-id="37220-107">**Tikai mākoņi** — visi Office 365 (O365) apmaksātie SKU vai Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="37220-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
  - <span data-ttu-id="37220-108">**Mākoņa un/vai Lokālie lietotāji** — Azure AD Premium P1 vai P2, Enterprise Mobility + Security (EMS) vai Secure ražīgs uzņēmums (SPE)</span><span class="sxs-lookup"><span data-stu-id="37220-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="37220-109">Papildinformāciju par licencēšanas prasībām skatiet rakstā Azure AD pašapkalpošanās [paroles atiestatīšanas licencēšanas prasības](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="37220-109">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span></span>
- <span data-ttu-id="37220-110">Jums ir vismaz viens administratora konts un viens testa lietotāja konts ar vienu no attiecīgās licences.</span><span class="sxs-lookup"><span data-stu-id="37220-110">You have at least one administrator account and one test user account with one of the appropriate license.</span></span>
- <span data-ttu-id="37220-111">Lai strādātu ar paroļu arī atpakaļrakstīšanas, ir jāizveido savienojums ar Azure AD savienojumu ar primāro domēna kontrollera administratoru.</span><span class="sxs-lookup"><span data-stu-id="37220-111">You must connect Azure AD Connect to the Primary Domain Controller Emulator for password writeback to work.</span></span> <span data-ttu-id="37220-112">Azure AD Connect varat konfigurēt, lai izmantotu primāro domēna kontrolleri, ar peles labo pogu noklikšķinot uz Active Directory sinhronizācijas savienotāja **rekvizītiem** un pēc tam atlasot **konfigurēt direktoriju nodalījumus**.</span><span class="sxs-lookup"><span data-stu-id="37220-112">You can configure Azure AD Connect to use a Primary Domain Controller by right clicking on the **properties** of the Active Directory synchronization connector, then selecting **configure directory partitions**.</span></span> <span data-ttu-id="37220-113">Šeit meklējiet sadaļu **domēna kontrollera savienojuma iestatījumi** un atzīmējiet izvēles rūtiņu **izmantot tikai vēlamos domēna kontrollerus**.</span><span class="sxs-lookup"><span data-stu-id="37220-113">From there, look for the **domain controller connection settings** section and check the box titled **only use preferred domain controllers**.</span></span>
  > [!NOTE]
  > <span data-ttu-id="37220-114">Ja vēlamais DC nav PDC emulators, Azure AD Connect joprojām sasniedz PDC paroļu arī atpakaļrakstīšanas.</span><span class="sxs-lookup"><span data-stu-id="37220-114">If the preferred DC is not a PDC emulator, Azure AD Connect will still reach out to the PDC for password writeback.</span></span>
- <span data-ttu-id="37220-115">Paroles atiestatīšana ir konfigurēta un iespējota jūsu nomniekā.</span><span class="sxs-lookup"><span data-stu-id="37220-115">Password reset has been configured and enabled in your tenant.</span></span> <span data-ttu-id="37220-116">Lai iegūtu papildinformāciju, skatiet rakstu [kā atļaut lietotājiem atiestatīt savas AZURE ad paroles](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span><span class="sxs-lookup"><span data-stu-id="37220-116">For more information, see [Enable users to reset their Azure AD passwords](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span></span>
- <span data-ttu-id="37220-117">Pārliecinieties, vai administratora konts, kas tiek izmantots, lai iespējotu paroļu arī atpakaļrakstīšanas, ir mākoņa administratora konts (izveidots Azure AD nav lokālās reklāmas)</span><span class="sxs-lookup"><span data-stu-id="37220-117">Make sure that the administrator account being used to enable Password Writeback is a cloud administrator account (created in Azure AD not on-premises AD)</span></span>
- <span data-ttu-id="37220-118">Jums ir viena vai vairāku mežu reklāma lokālajā izvietojumā, kurā darbojas sistēma Windows Server 2008 R2, Windows Server 2012 vai Windows Server 2012 R2 ar pēdējām instalētajām servisa pakotnēm</span><span class="sxs-lookup"><span data-stu-id="37220-118">You have a single or multi-forest AD on-premises deployment running Windows Server 2008 R2, Windows Server 2012, or Windows Server 2012 R2 with the latest service packs installed</span></span>
- <span data-ttu-id="37220-119">Jūs esat instalējis Azure AD Connect instrumentu un esat sagatavojis savu reklāmas vidi, lai sinhronizētu mākonī.</span><span class="sxs-lookup"><span data-stu-id="37220-119">You have the Azure AD Connect tool installed and you have prepared your AD environment for synchronization to the cloud.</span></span> <span data-ttu-id="37220-120">Pirms paroļu arī atpakaļrakstīšanas pārbaudes vispirms pārliecinieties, vai esat pabeidzis pilnu importēšanu un pilnīgu sinhronizāciju no AD un Azure AD Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="37220-120">Before testing password writeback, make sure that you first complete a full import and full sync from both AD and Azure AD in Azure AD Connect.</span></span>
- <span data-ttu-id="37220-121">Lai uzzinātu vairāk, skatiet rakstu kā veikt [pilno sinhronizāciju un pilnīgu importēšanu AZURE ad Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span><span class="sxs-lookup"><span data-stu-id="37220-121">To learn more, see how to do a [full sync and full import in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span></span>

<span data-ttu-id="37220-122">**Man radās problēma ar paroļu arī atpakaļrakstīšanas savienojumu**</span><span class="sxs-lookup"><span data-stu-id="37220-122">**I'm having a problem with password writeback connectivity**</span></span>

1. <span data-ttu-id="37220-123">Jaunākās [AZURE ad Connect](https://www.microsoft.com/download/details.aspx?id=47594) versijas lejupielāde un iespējošana</span><span class="sxs-lookup"><span data-stu-id="37220-123">Download and enable the latest version of [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span></span>
2. <span data-ttu-id="37220-124">Ugunsmūra konfigurācija: Azure AD Connect rīkam (1.1.443 un augstāk) vajadzēs **izejošo https** piekļuvi:</span><span class="sxs-lookup"><span data-stu-id="37220-124">Firewall configuration: The Azure AD Connect tool (1.1.443 and above) will need **outbound HTTPS** access to:</span></span>
    - <span data-ttu-id="37220-125">passwordreset.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="37220-125">passwordreset.microsoftonline.com</span></span>
    - <span data-ttu-id="37220-126">servicebus. Windows. Networks</span><span class="sxs-lookup"><span data-stu-id="37220-126">servicebus.windows.networks</span></span>
3. <span data-ttu-id="37220-127">Atļaut saglabāt dīkstāvi vismaz 2-3 minūtes</span><span class="sxs-lookup"><span data-stu-id="37220-127">Allow idle connections to persist for at least 2-3 minutes</span></span>

<span data-ttu-id="37220-128">**Joprojām pastāv problēmas ar paroļu arī atpakaļrakstīšanas**</span><span class="sxs-lookup"><span data-stu-id="37220-128">**I'm still having problems with password writeback**</span></span>

- <span data-ttu-id="37220-129">Ja joprojām rodas problēmas, mēģiniet atspējot un atkārtoti iespējot paroļu arī atpakaļrakstīšanas pakalpojumu Azure AD Connect rīkā</span><span class="sxs-lookup"><span data-stu-id="37220-129">If you are still having difficulty, try disabling and re-enabling the password writeback service in the Azure AD Connect tool</span></span>
- <span data-ttu-id="37220-130">Lai uzzinātu vairāk, skatiet rakstu kā [Atspējot un atkārtoti iespējot paroļu arī atpakaļrakstīšanas](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="37220-130">To learn more, see how to [disable and re-enable password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span></span>
