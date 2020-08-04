---
title: Ar VPN saistītās problēmas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555234"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="d9042-102">Ar VPN saistītās problēmas</span><span class="sxs-lookup"><span data-stu-id="d9042-102">VPN related issues</span></span>

<span data-ttu-id="d9042-103">Veiksmīga VPN savienojamības implementēšana attiecībā uz MDM klientiem ir atkarīga no izvietotā profila, kas pareizi atbilst VPN infrastruktūras prasībām.</span><span class="sxs-lookup"><span data-stu-id="d9042-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="d9042-104">Atbilstošos iestatījumus klientu platformām, kuras izmeklējat, skatiet:</span><span class="sxs-lookup"><span data-stu-id="d9042-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="d9042-105">Windows 10 un Windows Hologrāfiskās ierīces iestatījumi, lai pievienotu VPN savienojumus, izmantojot Intune</span><span class="sxs-lookup"><span data-stu-id="d9042-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="d9042-106">VPN iestatījumu pievienošana iOS un iPadOS ierīcēs programmā Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="d9042-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="d9042-107">Android ierīces iestatījumi VPN konfigurēšanai Intune</span><span class="sxs-lookup"><span data-stu-id="d9042-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="d9042-108">VPN iestatījumu pievienošana macOS ierīcēs programmā Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="d9042-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="d9042-109">Ja jūsu VPN profils izmanto autentifikāciju, kuras pamatā ir sertifikāts, pārliecinieties, vai saknes sertifikāts un klienta autentifikācijas sertifikātu profili, kas saistīti ar VPN profilu, ir sekmīgi izvietoti.</span><span class="sxs-lookup"><span data-stu-id="d9042-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="d9042-110">**Biežāk sastopamās problēmas**</span><span class="sxs-lookup"><span data-stu-id="d9042-110">**Common Issues**</span></span>

<span data-ttu-id="d9042-111">**Esmu izvietojis VPN profilu ierīcē. Intune rāda, ka tas ir izdevies, taču ierīce neveido savienojumu ar VPN.**</span><span class="sxs-lookup"><span data-stu-id="d9042-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="d9042-112">Veiksmīgs statuss nozīmē, ka Intune ir sekmīgi izvietojusi profilu kā konfigurētu.</span><span class="sxs-lookup"><span data-stu-id="d9042-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="d9042-113">Tomēr šīs konfigurācijas var nesaskanēt ar jūsu tīkla un/vai autentifikācijas prasībām.</span><span class="sxs-lookup"><span data-stu-id="d9042-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="d9042-114">Pārskatiet žurnālus infrastruktūras un autentifikācijas pakalpojumā (VPN serverī un NPS/rādiusa serverī), lai iegūtu papildinformāciju par mēģinājumu savienojumu.</span><span class="sxs-lookup"><span data-stu-id="d9042-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="d9042-115">Lai apkopotu un pārskatītu žurnālus, jums, iespējams, būs jāstrādā ar tīkla infrastruktūras grupu vai trešās puses VPN piegādātāju.</span><span class="sxs-lookup"><span data-stu-id="d9042-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="d9042-116">**Konfigurējot pielāgoto VPN for iOS, programmas VPN līdzeklis nav pieejams.**</span><span class="sxs-lookup"><span data-stu-id="d9042-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="d9042-117">Katras lietojumprogrammas VPN iOS ierīcēm sistēmā Intune pašlaik ir pieejama konkrētam pakalpojumu sniedzēju un partneru sarakstam, kam ir jāatbilst sertifikāta priekšnosacījumiem, pirms konfigurējot vienu lietojumprogrammu VPN.</span><span class="sxs-lookup"><span data-stu-id="d9042-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="d9042-118">Lai iegūtu papildinformāciju, skatiet rakstu [programmas Virtual Private Network (VPN) iestatīšana darbam ar iOS/iPadOS ierīcēm pakalpojumā Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span><span class="sxs-lookup"><span data-stu-id="d9042-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="d9042-119">Lai iegūtu papildinformāciju par visiem VPN savienojumu veidiem sistēmā Intune, skatiet rakstu [VPN profilu izveide, lai izveidotu savienojumu ar VPN serveriem Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="d9042-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="d9042-120">**pēc tam, kad tiek atvērts konfigurēts domēns, iOS pēc pieprasījuma VPN netiek aktivizēta**</span><span class="sxs-lookup"><span data-stu-id="d9042-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="d9042-121">Lai pārbaudītu automātiskos VPN iestatījumus, iestatiet tālāk norādītās vērtības.</span><span class="sxs-lookup"><span data-stu-id="d9042-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="d9042-122">Vēlos veikt šādas darbības: **katra savienojuma izveides mēģinājuma novērtēšana**</span><span class="sxs-lookup"><span data-stu-id="d9042-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="d9042-123">Izvēlieties, vai veidot savienojumu: **nepieciešamības gadījumā izveidot** savienojumu</span><span class="sxs-lookup"><span data-stu-id="d9042-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="d9042-124">Kad lietotāji piekļūst šiem domēniem: **mērķis** *domēna nosaukums*</span><span class="sxs-lookup"><span data-stu-id="d9042-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="d9042-125">Ja iepriekš norādītā konfigurācija nav sekmīga, pievienojiet šādu elementu:</span><span class="sxs-lookup"><span data-stu-id="d9042-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="d9042-126">Ja šis vietrādis URL nav sasniedzams, pievienojiet VPN: **BADURL**</span><span class="sxs-lookup"><span data-stu-id="d9042-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>