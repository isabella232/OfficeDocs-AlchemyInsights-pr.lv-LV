---
title: Intune Wi-Fi profili
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
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555313"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="60a13-102">Intune Wi-Fi profili</span><span class="sxs-lookup"><span data-stu-id="60a13-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="60a13-103">Veiksmīga Wi-Fi savienojamības ar MDM klientiem ieviešana ir atkarīga no pareiza izvietošanas profila, kas atbilst korporatīvās Wi-Fi infrastruktūras prasībām.</span><span class="sxs-lookup"><span data-stu-id="60a13-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="60a13-104">Lai pārskatītu atbilstošos iestatījumus klientu platformām, kuras izmeklējat, skatiet:</span><span class="sxs-lookup"><span data-stu-id="60a13-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="60a13-105">Wi-Fi iestatījumu pievienošana ierīcēs, kurās darbojas Android programmā Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="60a13-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="60a13-106">Wi-Fi iestatījumu pievienošana Android Enterprise atvēlētajām un pilnībā pārvaldītajām ierīcēm pakalpojumā Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="60a13-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="60a13-107">Wi-Fi iestatījumu pievienošana operētājsistēmā iOS un iPadOS ierīcēs programmā Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="60a13-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="60a13-108">Wi-Fi iestatījumu pievienošana sistēmai Windows 10 un jaunākām ierīcēm pakalpojumā Intune</span><span class="sxs-lookup"><span data-stu-id="60a13-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="60a13-109">Wi-Fi iestatījumu importēšana Windows ierīcēs Intune</span><span class="sxs-lookup"><span data-stu-id="60a13-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="60a13-110">**Biežāk sastopamās problēmas**</span><span class="sxs-lookup"><span data-stu-id="60a13-110">**Common Issues**</span></span>

<span data-ttu-id="60a13-111">**Esmu izvietojis Wi-Fi profilu, kas ir atkarīgs no Wi-Fi profilā norādītā izvietotā sertifikāta. Taču konfigurācijas profiliem tiek rādīts kļūdas statuss.**</span><span class="sxs-lookup"><span data-stu-id="60a13-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="60a13-112">Pārbaudiet, vai jūsu ierīce saņēma sertifikātu.</span><span class="sxs-lookup"><span data-stu-id="60a13-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="60a13-113">Sistēmā Intune dodieties uz **visas ierīces** un atlasiet ierīci, > **ierīces konfigurāciju**.</span><span class="sxs-lookup"><span data-stu-id="60a13-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="60a13-114">Pārbaudiet, vai visi gaidītie profili ir uzskaitīti un darbojas veiksmīgi.</span><span class="sxs-lookup"><span data-stu-id="60a13-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="60a13-115">Android profilam, ja jums ir starpposma sertifikāti jūsu sertifikātu ķēdē, pārliecinieties, vai tie ir izvietoti Android ierīcēs.</span><span class="sxs-lookup"><span data-stu-id="60a13-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="60a13-116">Lai pārbaudītu sertifikāta statusu, dodieties uz **ierīču konfigurācijas**  >  **profili**  >  **Android Intermediate CA**  >  **Rekvizīti**  >  **uzticams sertifikāts**.</span><span class="sxs-lookup"><span data-stu-id="60a13-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="60a13-117">Ja joprojām redzat kļūdas, pārskatiet sadaļu procedūras un problēmu novēršanas darbības.</span><span class="sxs-lookup"><span data-stu-id="60a13-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="60a13-118">Papildinformāciju skatiet rakstā [pārskats par problēmu novēršanas SCEP sertifikātu profiliem ar Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="60a13-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="60a13-119">**Es Izvietoju Wi-Fi profilu ierīcē. Intune rāda, ka tas ir izdevies, taču ierīce neveido savienojumu ar Wi-Fi.**</span><span class="sxs-lookup"><span data-stu-id="60a13-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="60a13-120">Veiksmīgs statuss nozīmē, ka Intune ir sekmīgi izvietojusi profilu kā konfigurētu.</span><span class="sxs-lookup"><span data-stu-id="60a13-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="60a13-121">Tomēr šīs konfigurācijas var nesaskanēt ar jūsu tīkla un/vai autentifikācijas prasībām.</span><span class="sxs-lookup"><span data-stu-id="60a13-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="60a13-122">Lai iegūtu detalizētu informāciju par mēģinājumu savienojumu, pārskatiet žurnālus infrastruktūras un autentifikācijas pakalpojumos (Wi-Fi piekļuves punkta kontrollerī un NPS/rādiusa serverī).</span><span class="sxs-lookup"><span data-stu-id="60a13-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="60a13-123">Lai apkopotu un pārskatītu žurnālus, jums, iespējams, būs jāstrādā ar tīkla infrastruktūras grupu vai trešās puses Wi-Fi piegādātāju.</span><span class="sxs-lookup"><span data-stu-id="60a13-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>