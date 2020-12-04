---
title: Ar PRT problēmu saistītu problēmu novēršana
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573719"
---
# <a name="troubleshoot-prt-issue"></a><span data-ttu-id="ff496-102">Ar PRT problēmu saistītu problēmu novēršana</span><span class="sxs-lookup"><span data-stu-id="ff496-102">Troubleshoot PRT issue</span></span>

<span data-ttu-id="ff496-103">Lai jebkura ierīce pabeigtu autentificēšanu, tai ir jābūt pilnībā reģistrētai un labā stāvoklī, kā arī var iegūt primāru atsvaidzināšanas marķieri (PRT).</span><span class="sxs-lookup"><span data-stu-id="ff496-103">For any device to complete getting authenticated, it must be fully registered and in good state and able to acquire a Primary Refresh Token (PRT).</span></span>

<span data-ttu-id="ff496-104">Hibrīdā Azure AD pievienoties reģistrācijas procesam ir nepieciešamas ierīces, lai tās būtu korporatīvajā tīklā.</span><span class="sxs-lookup"><span data-stu-id="ff496-104">The hybrid Azure AD join registration process requires devices to be on a corporate network.</span></span> <span data-ttu-id="ff496-105">Tā darbojas arī uz VPN, bet tam ir daži brīdinājumi.</span><span class="sxs-lookup"><span data-stu-id="ff496-105">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="ff496-106">Mēs esam dzirdējuši, ka klientiem ir jāsniedz palīdzība saistībā ar Hibrīdā Azure AD Join reģistrācijas procesu attālā darba apstākļos.</span><span class="sxs-lookup"><span data-stu-id="ff496-106">We’ve heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote-work circumstances.</span></span> <span data-ttu-id="ff496-107">Tālāk ir sniegts to darbību sadalījums, kas notiek ar kapuci reģistrācijas procesa laikā.</span><span class="sxs-lookup"><span data-stu-id="ff496-107">Here’s a breakdown of what’s happening ‘under the hood’ during the registration process.</span></span>

<span data-ttu-id="ff496-108">**Mākoņa autentifikācijas vide (izmantojot Azure AD Password hash Sync vai tranzīta autentifikāciju)**</span><span class="sxs-lookup"><span data-stu-id="ff496-108">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="ff496-109">Šo reģistrācijas plūsmu dēvē arī par sinhronizācijas savienojumu.</span><span class="sxs-lookup"><span data-stu-id="ff496-109">This registration flow is also known as “Sync Join”.</span></span>

1. <span data-ttu-id="ff496-110">Windows 10 atklāj SCP ierakstu, kad lietotājs pierakstās ierīcē.</span><span class="sxs-lookup"><span data-stu-id="ff496-110">Windows 10 discovers an SCP record upon user logging on to the device.</span></span>
    1. <span data-ttu-id="ff496-111">Ierīce vispirms mēģina izgūt nomnieka informāciju no klienta puses SCP reģistrā [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="ff496-111">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="ff496-112">Lai iegūtu papildinformāciju, skatiet šo [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="ff496-112">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    2. <span data-ttu-id="ff496-113">Ja tas nelīdz, ierīce komunicē ar lokālo Active Directory (AD), lai iegūtu nomnieka informāciju no pakalpojumu savienojuma punkta (SCP).</span><span class="sxs-lookup"><span data-stu-id="ff496-113">If it fails, the device communicates with on-premises Active Directory (AD) to get tenant information from Service Connection Point (SCP).</span></span> <span data-ttu-id="ff496-114">Lai verificētu SCP, lūdzu, skatiet šo [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="ff496-114">To verify SCP, please refer to this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span> 

> [!NOTE]
> <span data-ttu-id="ff496-115">Iesakām iespējot SCP reklāmas un tikai tad, izmantojot klienta puses SCP sākotnējai validācijai.</span><span class="sxs-lookup"><span data-stu-id="ff496-115">We recommend enabling SCP in the AD and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="ff496-116">Windows 10 mēģina sazināties ar Azure AD, izmantojot sistēmas kontekstu, lai autentificētu sevi pret Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ff496-116">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span> <span data-ttu-id="ff496-117">Varat pārbaudīt, vai ierīce var piekļūt Microsoft resursiem sistēmas kontā, izmantojot testa ierīces reģistrācijas savienojamības skriptu.</span><span class="sxs-lookup"><span data-stu-id="ff496-117">You can verify if the device can access Microsoft resources under the system account by using the Test Device Registration Connectivity script.</span></span>

3. <span data-ttu-id="ff496-118">Windows 10 izveido pašparakstītu sertifikātu un saglabā to zem datora objekta lokālajā REKLĀMā.</span><span class="sxs-lookup"><span data-stu-id="ff496-118">Windows 10 generates a self-signed certificate and stores it under the computer object in on-premises AD.</span></span> <span data-ttu-id="ff496-119">Lai to izdarītu, ir nepieciešams domēna kontrolleris.</span><span class="sxs-lookup"><span data-stu-id="ff496-119">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="ff496-120">Ierīces objekts, kura sertifikāts tiek sinhronizēts ar Azure AD, izmantojot Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="ff496-120">A device object that has a certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="ff496-121">Sinhronizācijas cikls ik pēc noklusējuma ir 30 minūtes, tomēr tas ir atkarīgs no Azure AD Connect konfigurēšanas.</span><span class="sxs-lookup"><span data-stu-id="ff496-121">Sync cycle is every 30 minutes by default, but it depends on configuration of Azure AD Connect.</span></span> <span data-ttu-id="ff496-122">Lai iegūtu papildinformāciju, lūdzu, skatiet šo [dokumentu](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="ff496-122">For more information, please refer to this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="ff496-123">Šajā posmā varat skatīt tēmas ierīci sadaļā "gaida", sadaļā ierīces disks Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="ff496-123">At this stage, you should be able to see the subject device in “Pending” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="ff496-124">Nākamajā lietotāja pierakstīšanās operētājsistēmā Windows 10 reģistrācija tiks pabeigta.</span><span class="sxs-lookup"><span data-stu-id="ff496-124">At the next user login to Windows 10, the registration will be completed.</span></span> 

> [!NOTE]
> <span data-ttu-id="ff496-125">Ja esat pieslēdzies VPN, bet atteikšanās process pārtrauc domēna savienojamību, varat manuāli aktivizēt reģistrāciju:</span><span class="sxs-lookup"><span data-stu-id="ff496-125">If you're on VPN and a logoff-login process terminates the domain connectivity, you can trigger registration manually:</span></span>
 1. <span data-ttu-id="ff496-126">Dsregcmd/Join lokāli uz administratora uzaicinājuma vai attālināti, izmantojot PSExec savā datorā.</span><span class="sxs-lookup"><span data-stu-id="ff496-126">Issue a dsregcmd /join locally on admin prompt or remotely via PSExec to your PC.</span></span> <span data-ttu-id="ff496-127">Piemēram, PsExec-s \\ win10client01 cmd, dsregcmd/Join</span><span class="sxs-lookup"><span data-stu-id="ff496-127">For example, PsExec -s \\win10client01 cmd, dsregcmd /join</span></span>

 2. <span data-ttu-id="ff496-128">Detalizētu informāciju par Hibrīdajām problēmām skatiet rakstā [ierīču problēmu novēršana](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span><span class="sxs-lookup"><span data-stu-id="ff496-128">For more details on Hybrid Join issues, see [Troubleshoot devices Issue](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span></span>
