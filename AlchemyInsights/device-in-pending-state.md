---
title: Ierīce gaidīšanas režīmā
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
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/11/2020
ms.locfileid: "49678484"
---
# <a name="device-in-pending-state"></a><span data-ttu-id="e7118-102">Ierīce gaidīšanas režīmā</span><span class="sxs-lookup"><span data-stu-id="e7118-102">Device in pending state</span></span>

<span data-ttu-id="e7118-103">**Priekšnoteikumi**</span><span class="sxs-lookup"><span data-stu-id="e7118-103">**Prerequisites:**</span></span>

1. <span data-ttu-id="e7118-104">Ja iestatāt ierīču reģistrācijas pirmo reizi, lūdzu, pārliecinieties, ka esat pārskatījis [Azure Active Directory (AZURE AD) Ievads](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) par ierīču pārvaldību, kas palīdzēs iegūt ierīces, kas atrodas Azure AD vadībā.</span><span class="sxs-lookup"><span data-stu-id="e7118-104">If you are setting up device registrations for the first time, please ensure that you have reviewed [Introduction to device management in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) that will guide you on how to get devices under the control of Azure AD.</span></span>
2. <span data-ttu-id="e7118-105">Ja esat reģistrējis ierīces Azure AD tiešā veidā un reģistrējat to Intune, jums ir jāpārliecinās, vai esat [konfigurējis Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) un ir vispirms [jālicencē](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) .</span><span class="sxs-lookup"><span data-stu-id="e7118-105">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
3. <span data-ttu-id="e7118-106">Pārliecinieties, vai jums ir atļauts veikt darbības Azure AD un lokālajā REKLĀMā.</span><span class="sxs-lookup"><span data-stu-id="e7118-106">Ensure you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="e7118-107">Tikai globālais administrators Azure AD var pārvaldīt ierīces reģistrācijām paredzētos iestatījumus.</span><span class="sxs-lookup"><span data-stu-id="e7118-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="e7118-108">Turklāt, ja iestatāt automātiskas reģistrācijas savā lokālajā Active Directory, jums būs nepieciešams Active Directory un AD FS administrators (ja piemērojams).</span><span class="sxs-lookup"><span data-stu-id="e7118-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="e7118-109">Hibrīdā Azure AD pievienošanās reģistrācijas procesam ir nepieciešamas ierīces, lai tās būtu korporatīvajā tīklā.</span><span class="sxs-lookup"><span data-stu-id="e7118-109">The hybrid Azure AD join registration process requires devices to be on corporate network.</span></span> <span data-ttu-id="e7118-110">Tā darbojas arī uz VPN, bet tam ir daži brīdinājumi.</span><span class="sxs-lookup"><span data-stu-id="e7118-110">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="e7118-111">Mēs esam dzirdējuši, ka klientiem ir nepieciešama palīdzība saistībā ar Hibrīdā Azure AD pievienošanās reģistrācijas procesam attālā darba apstākļos.</span><span class="sxs-lookup"><span data-stu-id="e7118-111">We have heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote work circumstances.</span></span>

<span data-ttu-id="e7118-112">**Mākoņa autentifikācijas vide (izmantojot Azure AD Password hash Sync vai tranzīta autentifikāciju)**</span><span class="sxs-lookup"><span data-stu-id="e7118-112">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="e7118-113">Šo reģistrācijas plūsmu dēvē arī par sinhronizācijas savienojumu.</span><span class="sxs-lookup"><span data-stu-id="e7118-113">This registration flow is also known as “Sync Join”.</span></span>

<span data-ttu-id="e7118-114">Tālāk ir aprakstīts, kas notiek reģistrācijas procesa laikā.</span><span class="sxs-lookup"><span data-stu-id="e7118-114">Here is a breakdown of what happens during the registration process:</span></span>

1. <span data-ttu-id="e7118-115">Windows 10 atklāj pakalpojumu savienojuma punkta (SCP) ierakstu, kad lietotājs piesakās savā ierīcē.</span><span class="sxs-lookup"><span data-stu-id="e7118-115">Windows 10 discovers Service Connection Point (SCP) record when the user logs on to the device.</span></span>

    1. <span data-ttu-id="e7118-116">Ierīce vispirms mēģina izgūt nomnieka informāciju no klienta puses SCP reģistrā [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="e7118-116">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="e7118-117">Papildinformāciju skatiet rakstā [dokuments](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="e7118-117">For more information, see [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    1. <span data-ttu-id="e7118-118">Ja tas nelīdz, ierīce komunicē ar lokālo Active Directory, lai iegūtu nomnieka informāciju no SCP.</span><span class="sxs-lookup"><span data-stu-id="e7118-118">If it fails, the device communicates with on-premises Active Directory to get tenant information from SCP.</span></span> <span data-ttu-id="e7118-119">Lai verificētu SCP, skatiet šo [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="e7118-119">To verify SCP, refer this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span>

    > [!NOTE]
    > <span data-ttu-id="e7118-120">Ieteicams iespējot SCP Active Directory un izmantot tikai klienta puses SCP sākotnējai validācijai.</span><span class="sxs-lookup"><span data-stu-id="e7118-120">We recommend enabling SCP in the Active Directory and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="e7118-121">Windows 10 mēģina sazināties ar Azure AD, izmantojot sistēmas kontekstu, lai autentificētu sevi pret Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e7118-121">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span>

    <span data-ttu-id="e7118-122">Varat pārbaudīt, vai ierīce var piekļūt Microsoft resursiem sistēmas kontā, izmantojot [testa ierīces reģistrācijas savienojamības skriptu](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span><span class="sxs-lookup"><span data-stu-id="e7118-122">You can verify if the device can access Microsoft resources under the system account by using the [Test Device Registration Connectivity script](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span></span>

3. <span data-ttu-id="e7118-123">Windows 10 izveido pašparakstītu sertifikātu un saglabā to zem datora objekta lokālajā Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e7118-123">Windows 10 generates self-signed certificate and stores it under the computer object in on-premises Active Directory.</span></span> <span data-ttu-id="e7118-124">Lai to izdarītu, ir nepieciešams domēna kontrolleris.</span><span class="sxs-lookup"><span data-stu-id="e7118-124">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="e7118-125">Ierīces objekts, kura sertifikāts tiek sinhronizēts ar Azure AD, izmantojot Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="e7118-125">Device object that has certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="e7118-126">Sinhronizācijas cikls ik pēc noklusējuma ir 30 minūtes, tomēr tas ir atkarīgs no Azure AD Connect konfigurēšanas.</span><span class="sxs-lookup"><span data-stu-id="e7118-126">Sync cycle is every 30 minutes by default, but it depends on the configuration of Azure AD Connect.</span></span> <span data-ttu-id="e7118-127">Lai iegūtu papildinformāciju, skatiet šo [dokumentu](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="e7118-127">For more information, refer this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="e7118-128">Šajā posmā varat skatīt tēmas ierīci sadaļā "**gaida**", sadaļā ierīces disks Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="e7118-128">At this stage, you should be able to see the subject device in “**Pending**” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="e7118-129">Nākamajā lietotāja pierakstīšanās operētājsistēmā Windows 10 reģistrācija tiks pabeigta.</span><span class="sxs-lookup"><span data-stu-id="e7118-129">At the next user login to Windows 10, the registration will be completed.</span></span>

    > [!NOTE]
    > <span data-ttu-id="e7118-130">Ja esat VPN un atteikšanās/pierakstīšanās pārtrauc domēna savienojamību, varat manuāli aktivizēt reģistrāciju.</span><span class="sxs-lookup"><span data-stu-id="e7118-130">If you are on VPN and logoff/login terminates the domain connectivity, you can trigger registration manually.</span></span> <span data-ttu-id="e7118-131">Lai to izdarītu:</span><span class="sxs-lookup"><span data-stu-id="e7118-131">To do that:</span></span>
    >
    > <span data-ttu-id="e7118-132">`dsregcmd /join`Lokāli jautājiet savā datorā, izmantojot PSExec.</span><span class="sxs-lookup"><span data-stu-id="e7118-132">Issue a `dsregcmd /join` locally on admin prompt or remotely via PSExec to your PC.</span></span>
    >
    > <span data-ttu-id="e7118-133">Piemēram: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span><span class="sxs-lookup"><span data-stu-id="e7118-133">For example: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span></span>

<span data-ttu-id="e7118-134">Biežāk sastopamās problēmas ar Azure Active Directory ierīces reģistrēšanu skatiet rakstā [bieži uzdotie jautājumi par ierīcēm](https://docs.microsoft.com/azure/active-directory/devices/faq).</span><span class="sxs-lookup"><span data-stu-id="e7118-134">For common issues with Azure Active Directory device registration, see [Devices FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq).</span></span>
