---
title: Izmantojiet pirkstu nospiedumu atbloķēšanas opciju operētājsistēmā Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 8a5059c722c306ad79811140062cec7f52f31766
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588322"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="14568-102">Izmantojiet pirkstu nospiedumu atbloķēšanas opciju operētājsistēmā Windows 10</span><span class="sxs-lookup"><span data-stu-id="14568-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="14568-103">**Iespējot Windows Hello pirksta nospiedumu**</span><span class="sxs-lookup"><span data-stu-id="14568-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="14568-104">Lai atbloķētu operētājsistēmu Windows 10, izmantojot pirksta nospiedumu, ir jāiestata Windows Hello pirksta nospiedums, pievienojot (ļaujot Windows iemācīties atpazīt) vismaz vienu pirkstu.</span><span class="sxs-lookup"><span data-stu-id="14568-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="14568-105">Dodieties uz **iestatījumi > konti > pierakstīšanās opcijas** (vai noklikšķiniet [šeit](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="14568-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="14568-106">Tiks uzskaitītas pieejamās pierakstīšanās opcijas.</span><span class="sxs-lookup"><span data-stu-id="14568-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="14568-107">Piemērs:</span><span class="sxs-lookup"><span data-stu-id="14568-107">For example:</span></span>

    ![Pierakstīšanās opcijas.](media/sign-in-options.png)

2. <span data-ttu-id="14568-109">Noklikšķiniet uz vai pieskarieties **Windows Hello pirksta nospiedums**, pēc tam noklikšķiniet uz **Iestatīt**.</span><span class="sxs-lookup"><span data-stu-id="14568-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="14568-110">Windows Hello iestatīšanas logā noklikšķiniet uz **Sākt darbu**.</span><span class="sxs-lookup"><span data-stu-id="14568-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="14568-111">Pirkstu nospiedumu sensors aktivizēs, un jums tiks lūgts novietot pirkstu uz sensora:</span><span class="sxs-lookup"><span data-stu-id="14568-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Pirkstu nospiedumu sensors.](media/fingerprint-sensor.png)

3. <span data-ttu-id="14568-113">Izpildiet norādījumus, kas prasīs atkārtoti skenēt pirkstu.</span><span class="sxs-lookup"><span data-stu-id="14568-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="14568-114">Kad tas ir izdarīts, jums būs iespēja pievienot citus pirkstus, kurus jūs varētu vēlēties izmantot pierakstīšanās gadījumā.</span><span class="sxs-lookup"><span data-stu-id="14568-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="14568-115">Nākamreiz, kad pierakstīsies operētājsistēmā Windows 10, jums būs iespēja izmantot pirksta nospiedumu.</span><span class="sxs-lookup"><span data-stu-id="14568-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="14568-116">**Windows Hello pirksta nospiedums nav pieejams kā pierakstīšanās opcija**</span><span class="sxs-lookup"><span data-stu-id="14568-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="14568-117">Ja Windows Hello pirksta nospiedums nav redzams kā opcija **pierakstīšanās opcijas**, tas nozīmē, ka Windows nav informēts par jebkuru pirkstu nospiedumu lasītāju/skeneri, kas ir pievienots datoram, vai arī sistēmas politika liedz tās izmantošanu (piemēram, ja jūsu datoru pārvalda darbvieta).</span><span class="sxs-lookup"><span data-stu-id="14568-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="14568-118">Lai novērstu:</span><span class="sxs-lookup"><span data-stu-id="14568-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="14568-119">Uzdevumjoslā atlasiet pogu **Sākums** un meklējiet **ierīču pārvaldnieks**.</span><span class="sxs-lookup"><span data-stu-id="14568-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="14568-120">Noklikšķiniet uz vai pieskarieties, lai atvērtu **ierīču pārvaldnieku**.</span><span class="sxs-lookup"><span data-stu-id="14568-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="14568-121">Ierīču pārvaldniekā izvērsiet sadaļu biometrijas ierīces, noklikšķinot uz tās Chevron.</span><span class="sxs-lookup"><span data-stu-id="14568-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biometrijas ierīcēm.](media/biometric-devices.png)

4. <span data-ttu-id="14568-123">Jūsu pirkstu nospiedumu skeneris ir jānorāda kā biometriskā ierīce, piemēram, Synaptics WBDI Scanner:</span><span class="sxs-lookup"><span data-stu-id="14568-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biometrijas ierīcēm.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="14568-125">Ja pirkstu nospiedumu skeneris netiek rādīts un skeneris ir integrēts datorā, apmeklējiet datora ražotāja vietni.</span><span class="sxs-lookup"><span data-stu-id="14568-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="14568-126">DATORA modeļa sadaļā tehniskā palīdzība meklējiet skenera Windows 10 draiveri, ko varat instalēt.</span><span class="sxs-lookup"><span data-stu-id="14568-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="14568-127">Ja skeneris ir atdalīts no datora (pievienots, izmantojot USB), apmeklējiet skenera ražotāja vietni, lai atrastu un instalētu Windows 10 ierīces draivera programmatūru savam skenera modelim.</span><span class="sxs-lookup"><span data-stu-id="14568-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
