---
title: SharePoint Online terminu krātuvē trūkst terminu
ms.author: pebaum
author: pebaum
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 28913b8e57e39d51e8957b7408c19337a119c589
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053520"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="03499-102">BitLocker šifrēšanas ar InTune iespējošana</span><span class="sxs-lookup"><span data-stu-id="03499-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="03499-103">InTune galapunkta aizsardzības politiku var izmantot, lai konfigurētu Windows ierīču Boitlocker šifrēšanas iestatījumus, kā aprakstīts: Windows10 (un jaunākām versijām) iestatījumus, lai aizsargātu ierīces, izmantojot InTune</span><span class="sxs-lookup"><span data-stu-id="03499-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="03499-104">Ņemiet vērā, ka daudzas jaunākas ierīces, kurās darbojas operētājsistēma Windows 10, atbalsta automātisku BitLocker šifrēšanu, kas tiek izraisīta, nepiemērojot MDM politiku.</span><span class="sxs-lookup"><span data-stu-id="03499-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="03499-105">Tas var ietekmēt politikas piemērošanu, ja nav noklusējuma iestatījumi ir konfigurēti.</span><span class="sxs-lookup"><span data-stu-id="03499-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="03499-106">Detalizētāku informāciju skatiet sadaļā BUJ.</span><span class="sxs-lookup"><span data-stu-id="03499-106">See FAQ for more detail.</span></span>


<span data-ttu-id="03499-107">FAQ  Q: kādi Windows izdevumi atbalsta ierīču šifrēšanu, izmantojot galapunktu aizsardzības politiku?</span><span class="sxs-lookup"><span data-stu-id="03499-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="03499-108"> A: InTune galapunkta aizsardzības politikas iestatījumi tiek ieviesti, izmantojot BitLocker CSP.</span><span class="sxs-lookup"><span data-stu-id="03499-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="03499-109">Ne visi izdevumi, ne arī veido Windows atbalsta BitLocker CSP. 
     </span><span class="sxs-lookup"><span data-stu-id="03499-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="03499-110">Šajā laikā Windows izdevumi: Enterprise; Education, Mobile, Mobile Enterprise un Professional (no Build 1809 gada) tiek atbalstīti.</span><span class="sxs-lookup"><span data-stu-id="03499-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="03499-111">Q: ja ierīce jau ir šifrēts ar BitLocker, izmantojot OS noklusējuma iestatījumus šifrēšanas metodei un šifra stiprums (XTS-AES-128), piemērojot politiku ar atšķirīgiem iestatījumiem, automātiski aktivizēs diska atkārtotu šifrēšanu ar jaunajiem iestatījumiem?</span><span class="sxs-lookup"><span data-stu-id="03499-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="03499-112">A: Nē.</span><span class="sxs-lookup"><span data-stu-id="03499-112">A: No.</span></span> <span data-ttu-id="03499-113">Lai lietotu jaunos šifra iestatījumus, vispirms disks ir atšifrēts.</span><span class="sxs-lookup"><span data-stu-id="03499-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="03499-114">Piezīme ierīcēm, kas uzņemti ar Autopilot automātiskās šifrēšanas, kas varētu rasties OOBE laikā nav aktivizēta līdz InTune politika tiek novērtēta, kas ļauj politikas iestatījumus izmantot vietā OS noklusējumus</span><span class="sxs-lookup"><span data-stu-id="03499-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="03499-115">Q Ja ierīce tiek šifrēta, kā rezultātā lietojumprogrammas InTune politika tiks atšifrēti, šī politika tiek noņemta?</span><span class="sxs-lookup"><span data-stu-id="03499-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="03499-116">A: noņemšana šifrēšanas saistīto politiku nerada atšifrēšana diskus, kas tika konfigurēts.</span><span class="sxs-lookup"><span data-stu-id="03499-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="03499-117">Q: kāpēc InTune atbilstības politika parāda, ka mana ierīce nav "BitLocker iespējota", bet tas ir?</span><span class="sxs-lookup"><span data-stu-id="03499-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="03499-118">: "BitLocker iespējots" iestatījums InTune atbilstības politika izmanto Windows Device Health apliecinājums (DHA) klientu.</span><span class="sxs-lookup"><span data-stu-id="03499-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="03499-119">Šis klients tikai mēra ierīces stāvokli sāknēšanas laikā.</span><span class="sxs-lookup"><span data-stu-id="03499-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="03499-120">Tātad, ja ierīce nav rebooted tā kā BitLocker šifrēšana tika pabeigta, DHA klienta pakalpojums neziņos par BitLocker kā aktīvu.</span><span class="sxs-lookup"><span data-stu-id="03499-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>