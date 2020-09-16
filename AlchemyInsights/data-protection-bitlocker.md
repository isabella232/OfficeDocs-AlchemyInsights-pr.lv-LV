---
title: Aspektus-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731246"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="b6b36-102">BitLocker šifrēšanas iespējošana ar Intune</span><span class="sxs-lookup"><span data-stu-id="b6b36-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="b6b36-103">Intune galapunkta aizsardzības politika var tikt izmantota, lai konfigurētu BitLocker šifrēšanas iestatījumus Windows ierīcēm.</span><span class="sxs-lookup"><span data-stu-id="b6b36-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="b6b36-104">Papildinformāciju skatiet rakstā [Windows 10 (un jaunākas versijas) iestatījumi, lai aizsargātu ierīces, kas izmanto Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="b6b36-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="b6b36-105">Ņemiet vērā, ka daudzās jaunākās ierīcēs, kurās darbojas operētājsistēma Windows 10, tiek atbalstīta automātiskā BitLocker šifrēšana, kas tiek palaista, nelietojot MDM politiku.</span><span class="sxs-lookup"><span data-stu-id="b6b36-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="b6b36-106">Tas var ietekmēt politikas lietojumu, ja tiek konfigurēti noklusējuma iestatījumi.</span><span class="sxs-lookup"><span data-stu-id="b6b36-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="b6b36-107">Papildinformāciju skatiet tālāk norādītajos bieži uzdotajos jautājumos.</span><span class="sxs-lookup"><span data-stu-id="b6b36-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="b6b36-108">Informāciju par BitLocker problēmu novēršanu skatiet rakstā [BitLocker politikas problēmu novēršana pakalpojumā Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="b6b36-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="b6b36-109">**BUJ**</span><span class="sxs-lookup"><span data-stu-id="b6b36-109">**FAQ**</span></span>

 <span data-ttu-id="b6b36-110">J: kādi Windows izdevumi atbalsta ierīces šifrēšanu, izmantojot galapunktu aizsardzības politiku?</span><span class="sxs-lookup"><span data-stu-id="b6b36-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="b6b36-111">A: Intune Endpoint Protection politikas iestatījumi tiek ieviesti, izmantojot [BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="b6b36-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="b6b36-112">Ne visi Windows izdevumi un būvējumi neatbalsta BitLocker CSP.</span><span class="sxs-lookup"><span data-stu-id="b6b36-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="b6b36-113">Pašlaik tiek atbalstīti šādi Windows izdevumi: Enterprise, Education, Mobile, Mobile Enterprise un Professional (būvējums 1809 un jaunākas versijas).</span><span class="sxs-lookup"><span data-stu-id="b6b36-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="b6b36-114">J: ja ierīce jau ir šifrēta ar BitLocker, izmantojot OS noklusējuma iestatījumus šifrēšanas metodei un Cipher Strength (XTS-AES-128), vai tiek lietota politika ar atšķirīgiem iestatījumiem, kas automātiski aktivizē šī diska atkārtotu šifrēšanu ar jaunajiem iestatījumiem?</span><span class="sxs-lookup"><span data-stu-id="b6b36-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="b6b36-115">A: Nē.</span><span class="sxs-lookup"><span data-stu-id="b6b36-115">A: No.</span></span> <span data-ttu-id="b6b36-116">Lai lietotu jaunos Cipher iestatījumus, vispirms diskam ir jābūt atšifrētam.</span><span class="sxs-lookup"><span data-stu-id="b6b36-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="b6b36-117">**Piezīme:** Ierīcēm, kuras tiek reģistrētas ar Autopilot, automātiskā šifrēšana, kas notiek OOBE laikā, netiek aktivizēta, kamēr Intune politika tiek novērtēta, kas ļauj izmantot politikas iestatījumus OS noklusējumu vietā.</span><span class="sxs-lookup"><span data-stu-id="b6b36-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="b6b36-118">J: ja ierīce ir šifrēta atbilstoši Intune politikas lietojumprogrammai, tā tiks atšifrēta, kad šī politika tiks noņemta?</span><span class="sxs-lookup"><span data-stu-id="b6b36-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="b6b36-119">: Ar šifrēšanu saistītas politikas noņemšana neizraisa konfigurēto disku atšifrēšanu.</span><span class="sxs-lookup"><span data-stu-id="b6b36-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="b6b36-120">J: Kāpēc Intune atbilstības politika rāda, ka manā ierīcē nav iespējots līdzeklis BitLocker, kaut gan tas ir?</span><span class="sxs-lookup"><span data-stu-id="b6b36-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="b6b36-121">A: "BitLocker iespējotais" iestatījums Intune atbilstības politikā izmanto Windows ierīces darbspējas atestācijas (DHA) klientu.</span><span class="sxs-lookup"><span data-stu-id="b6b36-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="b6b36-122">Šis klients nosaka ierīces stāvokli tikai sāknēšanas laikā.</span><span class="sxs-lookup"><span data-stu-id="b6b36-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="b6b36-123">Tāpēc, ja ierīce nav atsāknēta, jo BitLocker šifrēšana ir pabeigta, DHA klienta pakalpojums neziņo par BitLocker aktīvu.</span><span class="sxs-lookup"><span data-stu-id="b6b36-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 