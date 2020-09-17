---
title: Pirkstu nospiedumu atbloķēšanas opcijas lietošana operētājsistēmā Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795251"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="e21a3-102">Pirkstu nospiedumu atbloķēšanas opcijas lietošana operētājsistēmā Windows 10</span><span class="sxs-lookup"><span data-stu-id="e21a3-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="e21a3-103">**Windows Hello Fingerprint iespējošana**</span><span class="sxs-lookup"><span data-stu-id="e21a3-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="e21a3-104">Lai atbloķētu Windows 10, izmantojot pirkstu nospiedumu, ir jāiestata Windows Hello Fingerprint, pievienojot (ļaujot Windows uzzināt atpazīst) vismaz vienu pirkstu.</span><span class="sxs-lookup"><span data-stu-id="e21a3-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="e21a3-105">Dodieties uz **sadaļu iestatījumi > konti > pierakstīšanās opcijas** (vai noklikšķiniet [šeit](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="e21a3-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="e21a3-106">Būs norādītas pieejamās pierakstīšanās opcijas.</span><span class="sxs-lookup"><span data-stu-id="e21a3-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="e21a3-107">Piemērs:</span><span class="sxs-lookup"><span data-stu-id="e21a3-107">For example:</span></span>

    ![Pierakstīšanās opcijas.](media/sign-in-options.png)

2. <span data-ttu-id="e21a3-109">Noklikšķiniet uz vai pieskarieties pie **Windows Hello Fingerprint**, pēc tam noklikšķiniet uz **Iestatīt**.</span><span class="sxs-lookup"><span data-stu-id="e21a3-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="e21a3-110">Windows Hello uzstādīšanas logā noklikšķiniet uz **Sākt darbu**.</span><span class="sxs-lookup"><span data-stu-id="e21a3-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="e21a3-111">Pirkstu nospiedumu sensors tiks aktivizēts, un jums tiks lūgts novietot pirkstu uz sensora:</span><span class="sxs-lookup"><span data-stu-id="e21a3-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Pirkstu nospiedumu sensors.](media/fingerprint-sensor.png)

3. <span data-ttu-id="e21a3-113">Izpildiet norādījumus, kas lūgs atkārtoti skenēt pirkstu.</span><span class="sxs-lookup"><span data-stu-id="e21a3-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="e21a3-114">Kad tas ir izdarīts, jums būs iespēja pievienot citus pirkstus, kurus varat izmantot, lai pierakstītos.</span><span class="sxs-lookup"><span data-stu-id="e21a3-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="e21a3-115">Nākamreiz, kad pierakstīsities operētājsistēmā Windows 10, jums būs iespēja izmantot savu pirksta nospiedumu.</span><span class="sxs-lookup"><span data-stu-id="e21a3-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="e21a3-116">**Windows Hello Fingerprint nav pieejama kā pierakstīšanās opcija**</span><span class="sxs-lookup"><span data-stu-id="e21a3-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="e21a3-117">Ja Windows Hello pirksta nospiedums netiek rādīts kā opcija **pierakstīšanās opcijās**, tas nozīmē, ka Windows nezina nevienu pirkstu nospiedumu lasītāju/skeneri, kas pievienots datoram, vai sistēmas politika neļauj to izmantot (ja, piemēram, jūsu datoru pārvalda jūsu darbvieta).</span><span class="sxs-lookup"><span data-stu-id="e21a3-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="e21a3-118">Lai novērstu problēmu:</span><span class="sxs-lookup"><span data-stu-id="e21a3-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="e21a3-119">Uzdevumjoslā atlasiet pogu **Sākums** un meklējiet **ierīču pārvaldnieks**.</span><span class="sxs-lookup"><span data-stu-id="e21a3-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="e21a3-120">Noklikšķiniet vai pieskarieties, lai atvērtu **ierīču pārvaldnieku**.</span><span class="sxs-lookup"><span data-stu-id="e21a3-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="e21a3-121">Ierīču pārvaldniekā izvērsiet biometrijas ierīces, noklikšķinot uz tās v veida.</span><span class="sxs-lookup"><span data-stu-id="e21a3-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biometrijas ierīces.](media/biometric-devices.png)

4. <span data-ttu-id="e21a3-123">Jūsu pirkstu nospiedumu skenerim ir jābūt norādītam kā biometriskai ierīcei, piemēram, Synaptics WBDI skenerim:</span><span class="sxs-lookup"><span data-stu-id="e21a3-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biometrijas ierīces.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="e21a3-125">Ja netiek parādīts jūsu pirkstu nospiedumu skeneris un skeneris ir iebūvēts datorā, atveriet datora ražotāja tīmekļa vietni.</span><span class="sxs-lookup"><span data-stu-id="e21a3-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="e21a3-126">Datora modeļa sadaļā tehniskais atbalsts meklējiet Windows 10 draiveri rīkam, ko varat instalēt.</span><span class="sxs-lookup"><span data-stu-id="e21a3-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="e21a3-127">Ja skeneris ir atdalīts no datora (pievienots, izmantojot USB), dodieties uz skenera ražotāja tīmekļa vietni, lai atrastu un instalētu Windows 10 ierīču draiveru programmatūru jūsu skenera modelim.</span><span class="sxs-lookup"><span data-stu-id="e21a3-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
