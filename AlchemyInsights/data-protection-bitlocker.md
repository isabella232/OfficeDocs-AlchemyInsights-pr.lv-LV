---
title: DataProtection — BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908716"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="81187-102">BitLocker šifrēšanas ar InTune iespējošana</span><span class="sxs-lookup"><span data-stu-id="81187-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="81187-103">InTune galapunkta aizsardzības politiku var izmantot, lai konfigurētu BitLocker šifrēšanas iestatījumus Windows ierīcēm.</span><span class="sxs-lookup"><span data-stu-id="81187-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="81187-104">Lai iegūtu papildinformāciju, skatiet [Windows 10 (un jaunākām versijām) iestatījumus, lai aizsargātu ierīces, izmantojot InTune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="81187-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="81187-105">Ņemiet vērā, ka daudzas jaunākas ierīces, kurās darbojas operētājsistēma Windows 10, atbalsta automātisku BitLocker šifrēšanu, kas tiek izraisīta bez MDM politikas lietojumprogrammas.</span><span class="sxs-lookup"><span data-stu-id="81187-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="81187-106">Tas var ietekmēt politikas piemērošanu, ja nav noklusējuma iestatījumi ir konfigurēti.</span><span class="sxs-lookup"><span data-stu-id="81187-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="81187-107">Detalizētu informāciju skatiet tālāk sadaļā BUJ.</span><span class="sxs-lookup"><span data-stu-id="81187-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="81187-108">Informāciju par BitLocker problēmu novēršanu skatiet [problēmu novēršana saistībā ar BitLocker politikām Microsoft InTune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="81187-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="81187-109">**Faq**</span><span class="sxs-lookup"><span data-stu-id="81187-109">**FAQ**</span></span>

 <span data-ttu-id="81187-110">Q: kādi izdevumi Windows atbalsta ierīču šifrēšana, izmantojot galapunktu aizsardzības politiku?</span><span class="sxs-lookup"><span data-stu-id="81187-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="81187-111">A: InTune galapunkta aizsardzības politikas iestatījumi tiek ieviesti, izmantojot [BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="81187-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="81187-112">Ne visi izdevumi vai būvējumi Windows atbalsta BitLocker CSP.</span><span class="sxs-lookup"><span data-stu-id="81187-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="81187-113">Šajā laikā tiek atbalstīti šādi Windows izdevumi: Enterprise, Education, Mobile, Mobile Enterprise un Professional (būvējums 1809 un jaunākas versijas).</span><span class="sxs-lookup"><span data-stu-id="81187-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="81187-114">Q: ja ierīce jau ir šifrēts ar BitLocker, izmantojot OS noklusējuma iestatījumus šifrēšanas metodi un šifra stiprums (XTS-AES-128), piemērojot politiku ar dažādiem iestatījumiem automātiski izraisīt atkārtotu šifrēšanu disku ar jaunajiem iestatījumiem?</span><span class="sxs-lookup"><span data-stu-id="81187-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="81187-115">A: Nē.</span><span class="sxs-lookup"><span data-stu-id="81187-115">A: No.</span></span> <span data-ttu-id="81187-116">Lai lietotu jaunos šifra iestatījumus, vispirms disks ir atšifrēts.</span><span class="sxs-lookup"><span data-stu-id="81187-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="81187-117">**Piezīme:** Ierīces tiek uzņemti ar Autopilot, automātiskā šifrēšana, kas varētu rasties OOBE laikā nav aktivizēta līdz InTune politika tiek novērtēta, kas ļauj izmantot politikas iestatījumus vietā OS noklusējumus.</span><span class="sxs-lookup"><span data-stu-id="81187-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="81187-118">Q: ja ierīce tiek šifrēta, kā lietojumprogrammas InTune politikas dēļ, tas tiks atšifrēts, tiek noņemta politika?</span><span class="sxs-lookup"><span data-stu-id="81187-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="81187-119">A: noņemšana šifrēšanas saistīto politiku nerada atšifrēšana diskus, kas tika konfigurēts.</span><span class="sxs-lookup"><span data-stu-id="81187-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="81187-120">Q: kāpēc InTune atbilstības politika parāda, ka mana ierīce nav iespējots BitLocker, pat ja tas ir?</span><span class="sxs-lookup"><span data-stu-id="81187-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="81187-121">: "BitLocker iespējots" iestatījums InTune atbilstības politika izmanto Windows Device Health apliecinājums (DHA) klientu.</span><span class="sxs-lookup"><span data-stu-id="81187-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="81187-122">Šis klients tikai mēra ierīces stāvokli sāknēšanas laikā.</span><span class="sxs-lookup"><span data-stu-id="81187-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="81187-123">Tāpēc, ja ierīce nav rebooted tā kā BitLocker šifrēšana ir pabeigta, DHA klienta pakalpojums neziņos BitLocker par aktīvu.</span><span class="sxs-lookup"><span data-stu-id="81187-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 