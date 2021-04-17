---
title: Pierakstīšanās operētājsistēmā Windows 10, neizmantojot paroli
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
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830553"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="c5b5e-102">Pierakstīšanās operētājsistēmā Windows 10, neizmantojot paroli</span><span class="sxs-lookup"><span data-stu-id="c5b5e-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="c5b5e-103">Lai izvairītos no nepieciešamības ievadīt paroli Windows startēšanas laikā, ieteicams izmantot kādu no Windows Hello drošās pierakstīšanās opcijām, piemēram, PIN, sejas atpazīšanu vai pirksta nospiedumu, ja tāda ir pieejama.</span><span class="sxs-lookup"><span data-stu-id="c5b5e-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="c5b5e-104">Ja tiešām vēlaties atspējot drošo pierakstīšanu, skatiet tālāk esošos norādījumus "Automātiska pierakstīšanās sistēmā Windows 10".</span><span class="sxs-lookup"><span data-stu-id="c5b5e-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="c5b5e-105">**Kā aizsargāt Windows Hello alternatīvas konta parolei**</span><span class="sxs-lookup"><span data-stu-id="c5b5e-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="c5b5e-106">Dodieties **uz > konti > Pierakstīšanās opcijas** (vai noklikšķiniet [šeit).](ms-settings:signinoptions?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="c5b5e-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="c5b5e-107">Tiks uzskaitītas pieejamās pierakstīšanās opcijas.</span><span class="sxs-lookup"><span data-stu-id="c5b5e-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="c5b5e-108">Piemēram:</span><span class="sxs-lookup"><span data-stu-id="c5b5e-108">For example:</span></span>

![Pierakstīšanās opcijas.](media/sign-in-options.png)

<span data-ttu-id="c5b5e-110">Noklikšķiniet uz vai pieskarieties pie vienas no opcijām, lai to konfigurētu.</span><span class="sxs-lookup"><span data-stu-id="c5b5e-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="c5b5e-111">Nākamreiz, kad startēsit vai atbloķēsit sistēmu Windows, varēsit izmantot jauno opciju, nevis paroli.</span><span class="sxs-lookup"><span data-stu-id="c5b5e-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="c5b5e-112">**Automātiska pierakstīšanās operētājsistēmā Windows 10**</span><span class="sxs-lookup"><span data-stu-id="c5b5e-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="c5b5e-113">**Piezīme.** Automātiskā pierakstīšanās ir ērta, taču rada drošības risku, īpaši, ja jūsu dators ir pieejams vairākiem cilvēkiem.</span><span class="sxs-lookup"><span data-stu-id="c5b5e-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="c5b5e-114">Uzdevumjoslā **noklikšķiniet uz** vai pieskarieties pie pogas Sākt.</span><span class="sxs-lookup"><span data-stu-id="c5b5e-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="c5b5e-115">Ierakstiet **netplwiz** un nospiediet taustiņu Enter, lai atvērtu logu Lietotāju konti.</span><span class="sxs-lookup"><span data-stu-id="c5b5e-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="c5b5e-116">Izvēlnē **Lietotāju konti** noklikšķiniet uz konta, kurā vēlaties automātiski pierakstīties sistēmas Windows startēšanas laikā.</span><span class="sxs-lookup"><span data-stu-id="c5b5e-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="c5b5e-117">Notīriet izvēles rūtiņu Lai izmantotu šo datoru, lietotājiem ir jāievada lietotājvārds un parole.</span><span class="sxs-lookup"><span data-stu-id="c5b5e-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Lietotājiem ir jāievada lietotājvārda un paroles opcija.](media/users-must-enter-username.png)

5. <span data-ttu-id="c5b5e-119">Noklikšķiniet uz **Labi**.</span><span class="sxs-lookup"><span data-stu-id="c5b5e-119">Click **OK**.</span></span> <span data-ttu-id="c5b5e-120">Jums tiks lūgts ievadīt un apstiprināt atlasītā konta paroli.</span><span class="sxs-lookup"><span data-stu-id="c5b5e-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="c5b5e-121">Noklikšķiniet **uz Labi,** lai pabeigtu.</span><span class="sxs-lookup"><span data-stu-id="c5b5e-121">Click **OK** to finish.</span></span> <span data-ttu-id="c5b5e-122">Nākamajā Windows 10 startēšanas reizē tā automātiski pierakstīsies atlasītajā kontā.</span><span class="sxs-lookup"><span data-stu-id="c5b5e-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
