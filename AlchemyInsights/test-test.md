---
title: SharePoint Online terminu krātuvē trūkst terminu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750458"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="5baa3-102">BitLocker šifrēšanas iespējošana ar Intune</span><span class="sxs-lookup"><span data-stu-id="5baa3-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="5baa3-103">Intune Endpoint Protection politiku var izmantot, lai konfigurētu Boitlocker šifrēšanas iestatījumus Windows ierīcēm, kā aprakstīts: Windows 10 (un jaunākas versijas) iestatījumi, lai aizsargātu ierīces, kas izmanto Intune</span><span class="sxs-lookup"><span data-stu-id="5baa3-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="5baa3-104">Ņemiet vērā, ka daudzās jaunākās ierīcēs, kurās darbojas operētājsistēma Windows 10, tiek atbalstīta automātiskā BitLocker šifrēšana, kas tiek palaista, nelietojot MDM politiku.</span><span class="sxs-lookup"><span data-stu-id="5baa3-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="5baa3-105">Tas var ietekmēt politikas lietojumu, ja nav konfigurēti noklusējuma iestatījumi.</span><span class="sxs-lookup"><span data-stu-id="5baa3-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="5baa3-106">Detalizētāku informāciju skatiet rakstā bieži uzdotie jautājumi.</span><span class="sxs-lookup"><span data-stu-id="5baa3-106">See FAQ for more detail.</span></span>


<span data-ttu-id="5baa3-107">Bieži uzdotie jautājumi   : kādus Windows izdevumus atbalsta ierīces šifrēšana, izmantojot galapunktu aizsardzības politiku?</span><span class="sxs-lookup"><span data-stu-id="5baa3-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="5baa3-108"> A: Intune Endpoint Protection politikas iestatījumi tiek ieviesti, izmantojot BitLocker CSP.</span><span class="sxs-lookup"><span data-stu-id="5baa3-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="5baa3-109">Ne visi izdevumi un būvējumi Windows neatbalsta BitLocker CSP. 
     </span><span class="sxs-lookup"><span data-stu-id="5baa3-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="5baa3-110">Šajā laikā Windows izdevumi: Enterprise; Tiek atbalstītas Education, Mobile, Mobile Enterprise un Professional (no būvējuma 1809).</span><span class="sxs-lookup"><span data-stu-id="5baa3-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="5baa3-111">J: ja ierīce jau ir šifrēta ar BitLocker, izmantojot OS noklusējuma iestatījumus šifrēšanas metodei un Cipher Strength (XTS-AES-128), tiks lietota politika ar dažādiem iestatījumiem, kas automātiski aktivizēs ar jaunajiem iestatījumiem atkārtoti šifrētu disku.</span><span class="sxs-lookup"><span data-stu-id="5baa3-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="5baa3-112">A: Nē.</span><span class="sxs-lookup"><span data-stu-id="5baa3-112">A: No.</span></span> <span data-ttu-id="5baa3-113">Lai lietotu jaunos Cipher iestatījumus, vispirms diskam ir jābūt atšifrētam.</span><span class="sxs-lookup"><span data-stu-id="5baa3-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="5baa3-114">Piezīme ierīcēm, kas tiek reģistrētas, izmantojot automātisko testēšanu, automātiskā šifrēšana, kas rastos OOBE laikā, netiek aktivizēta, kamēr Intune politika tiek novērtēta, kas ļauj izmantot politikas iestatījumus, kas tiek izmantoti OS noklusējumu vietā</span><span class="sxs-lookup"><span data-stu-id="5baa3-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="5baa3-115">Ja ierīce ir šifrēta atbilstoši Intune politikas lietojumam, tā tiks atšifrēta, kad šī politika tiks noņemta?</span><span class="sxs-lookup"><span data-stu-id="5baa3-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="5baa3-116">: Šifrēšanas saistītās politikas noņemšana neizraisa to disku atšifrēšanu, kas ir konfigurēti.</span><span class="sxs-lookup"><span data-stu-id="5baa3-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="5baa3-117">J: Kāpēc Intune atbilstības politika rāda, ka manai ierīcei nav "BitLocker iespējots", bet tas ir?</span><span class="sxs-lookup"><span data-stu-id="5baa3-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="5baa3-118">A: "BitLocker iespējots" iestatījums Intune atbilstības politikā izmanto Windows ierīces Health atestācijas (DHA) klientu.</span><span class="sxs-lookup"><span data-stu-id="5baa3-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="5baa3-119">Šis klients nosaka ierīces stāvokli tikai sāknēšanas laikā.</span><span class="sxs-lookup"><span data-stu-id="5baa3-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="5baa3-120">Tāpēc, ja ierīce nav atsāknēta, jo ir pabeigta BitLocker šifrēšana, DHA klienta pakalpojums neziņo par BitLocker aktīvu.</span><span class="sxs-lookup"><span data-stu-id="5baa3-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>