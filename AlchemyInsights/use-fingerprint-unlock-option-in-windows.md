---
title: Pirksta nospiedumu atbloķēšanas opcijas izmantošana operētājsistēmā Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796684"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="3035c-102">Pirksta nospiedumu atbloķēšanas opcijas izmantošana operētājsistēmā Windows 10</span><span class="sxs-lookup"><span data-stu-id="3035c-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="3035c-103">**Iespējot Windows Hello pirkstu nospiedumu**</span><span class="sxs-lookup"><span data-stu-id="3035c-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="3035c-104">Lai atbloķētu windows 10, izmantojot pirksta nospiedumu, ir jāiestata Windows Hello pirksta nospiedums, pievienojot (ļaujot Windows uzzināt, kā to atpazīt) vismaz vienu pirkstu.</span><span class="sxs-lookup"><span data-stu-id="3035c-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="3035c-105">Dodieties **uz > konti > Pierakstīšanās opcijas** (vai noklikšķiniet [šeit).](ms-settings:signinoptions?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="3035c-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="3035c-106">Tiks uzskaitītas pieejamās pierakstīšanās opcijas.</span><span class="sxs-lookup"><span data-stu-id="3035c-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="3035c-107">Piemēram:</span><span class="sxs-lookup"><span data-stu-id="3035c-107">For example:</span></span>

    ![Pierakstīšanās opcijas.](media/sign-in-options.png)

2. <span data-ttu-id="3035c-109">Noklikšķiniet uz vai pieskarieties pie **Windows Hello pirksta nospiedumu** un pēc tam **noklikšķiniet uz Iestatīt**.</span><span class="sxs-lookup"><span data-stu-id="3035c-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="3035c-110">Windows Hello iestatīšanas logā noklikšķiniet uz **Sākt darbu.**</span><span class="sxs-lookup"><span data-stu-id="3035c-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="3035c-111">Tiks aktivizēts pirkstu nospiedumu sensors, un jums tiks lūgts novietot pirkstu uz sensora:</span><span class="sxs-lookup"><span data-stu-id="3035c-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Pirkstu nospiedumu sensors.](media/fingerprint-sensor.png)

3. <span data-ttu-id="3035c-113">Izpildiet norādījumus, kas lūgs atkārtoti skenēt pirkstu.</span><span class="sxs-lookup"><span data-stu-id="3035c-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="3035c-114">Kad tas ir izdarīts, varat pievienot citus pirkstus, kurus, iespējams, vēlēsities izmantot, lai pierakstītos.</span><span class="sxs-lookup"><span data-stu-id="3035c-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="3035c-115">Nākamreiz, kad pierakstīsties operētājsistēmā Windows 10, jums būs iespēja izmantot pirksta nospiedumu, lai to izdarītu.</span><span class="sxs-lookup"><span data-stu-id="3035c-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="3035c-116">**Windows Hello pirkstu nospiedumu nav pieejama kā pierakstīšanās opcija**</span><span class="sxs-lookup"><span data-stu-id="3035c-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="3035c-117">Ja opcija Pierakstīšanās opcijas netiek rādīta, izmantojot Windows Hello pirkstu nospiedumu, sistēma Windows neizmanto jūsu datoram pievienoto pirkstu nospiedumu lasītāju/skeneri vai arī sistēmas politika neļauj to izmantot (ja, piemēram, jūsu datoru pārvalda jūsu darbvieta). </span><span class="sxs-lookup"><span data-stu-id="3035c-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="3035c-118">Lai novērstu problēmas,</span><span class="sxs-lookup"><span data-stu-id="3035c-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="3035c-119">**Uzdevumjoslā** atlasiet pogu Sākums un meklējiet **Ierīču pārvaldnieks**.</span><span class="sxs-lookup"><span data-stu-id="3035c-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="3035c-120">Noklikšķiniet uz vai pieskarieties, lai **atvērtu ierīču pārvaldnieku**.</span><span class="sxs-lookup"><span data-stu-id="3035c-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="3035c-121">Ierīču pārvaldniekā izvērsiet biometriskās ierīces, noklikšķinot uz tās skujiņas.</span><span class="sxs-lookup"><span data-stu-id="3035c-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biometriskas ierīces.](media/biometric-devices.png)

4. <span data-ttu-id="3035c-123">Jūsu pirkstu nospiedumu skenerim ir jābūt norādītam kā biometriskai ierīcei, piemēram, sinaptikas WBDI skenerim:</span><span class="sxs-lookup"><span data-stu-id="3035c-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biometriskas ierīces.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="3035c-125">Ja jūsu pirkstu nospiedumu skeneris nav redzams un skeneris ir integrēts jūsu datorā, dodieties uz datora ražotāja tīmekļa vietni.</span><span class="sxs-lookup"><span data-stu-id="3035c-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="3035c-126">Datora modeļa tehniskā atbalsta sadaļā meklējiet Windows 10 draiveri, ko instalēt.</span><span class="sxs-lookup"><span data-stu-id="3035c-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="3035c-127">Ja skeneris nav dators (pievienots, izmantojot USB), dodieties uz skenera ražotāja tīmekļa vietni, lai atrastu un instalētu Windows 10 ierīces draivera programmatūru jūsu skenera modelim.</span><span class="sxs-lookup"><span data-stu-id="3035c-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
