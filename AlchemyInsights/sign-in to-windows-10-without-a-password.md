---
title: Pierakstīšanās operētājsistēmā Windows 10, neizmantojot paroli
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
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719960"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="ea737-102">Pierakstīšanās operētājsistēmā Windows 10, neizmantojot paroli</span><span class="sxs-lookup"><span data-stu-id="ea737-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="ea737-103">Lai izvairītos no paroles ievadīšanas Windows startēšanas laikā, iesakām izmantot kādu no Windows Hello drošās pierakstīšanās opcijām, piemēram, PIN, sejiņas atpazīšanu vai pirksta nospiedumu, ja tas ir pieejams.</span><span class="sxs-lookup"><span data-stu-id="ea737-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="ea737-104">Ja tiešām vēlaties atspējot drošu pierakstīšanos, skatiet tālāk sniegtos norādījumus "automātiska pierakstīšanās Windows 10".</span><span class="sxs-lookup"><span data-stu-id="ea737-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="ea737-105">**Drošas Windows Hello alternatīvas konta parolei**</span><span class="sxs-lookup"><span data-stu-id="ea737-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="ea737-106">Dodieties uz **sadaļu iestatījumi > konti > pierakstīšanās opcijas** (vai noklikšķiniet [šeit](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="ea737-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="ea737-107">Būs norādītas pieejamās pierakstīšanās opcijas.</span><span class="sxs-lookup"><span data-stu-id="ea737-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="ea737-108">Piemērs:</span><span class="sxs-lookup"><span data-stu-id="ea737-108">For example:</span></span>

![Pierakstīšanās opcijas.](media/sign-in-options.png)

<span data-ttu-id="ea737-110">Noklikšķiniet uz vai pieskarieties vienai no opcijām, lai to konfigurētu.</span><span class="sxs-lookup"><span data-stu-id="ea737-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="ea737-111">Nākamreiz, kad startējat vai atbloķējat Windows, paroles vietā varēsit izmantot jauno opciju.</span><span class="sxs-lookup"><span data-stu-id="ea737-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="ea737-112">**Automātiska pierakstīšanās operētājsistēmā Windows 10**</span><span class="sxs-lookup"><span data-stu-id="ea737-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="ea737-113">**Piezīme**: automātiska pierakstīšanās ir ērta, taču ir ieviesti drošības riski, it īpaši tad, ja jūsu dators ir pieejams vairākām personām.</span><span class="sxs-lookup"><span data-stu-id="ea737-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="ea737-114">Noklikšķiniet uz vai pieskarieties pie pogas **Sākt** uzdevumjoslā.</span><span class="sxs-lookup"><span data-stu-id="ea737-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="ea737-115">Ierakstiet **netplwiz** un nospiediet taustiņu ENTER, lai atvērtu lietotāju kontu logu.</span><span class="sxs-lookup"><span data-stu-id="ea737-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="ea737-116">**Lietotāju kontos**noklikšķiniet uz konta, kuram vēlaties automātiski pierakstīties, startējot sistēmu Windows.</span><span class="sxs-lookup"><span data-stu-id="ea737-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="ea737-117">Atzīmējiet izvēles rūtiņu "lietotājiem ir jāievada lietotājvārds un parole, lai izmantotu šo datoru".</span><span class="sxs-lookup"><span data-stu-id="ea737-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Lietotājiem ir jāievada lietotājvārds un parole.](media/users-must-enter-username.png)

5. <span data-ttu-id="ea737-119">Noklikšķiniet uz **Labi**.</span><span class="sxs-lookup"><span data-stu-id="ea737-119">Click **OK**.</span></span> <span data-ttu-id="ea737-120">Jums būs jāievada un jāapstiprina atlasītā konta parole.</span><span class="sxs-lookup"><span data-stu-id="ea737-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="ea737-121">Noklikšķiniet uz **Labi** , lai pabeigtu.</span><span class="sxs-lookup"><span data-stu-id="ea737-121">Click **OK** to finish.</span></span> <span data-ttu-id="ea737-122">Nākamreiz, kad tiks palaista operētājsistēma Windows 10, tā automātiski pierakstīsies atlasītajā kontā.</span><span class="sxs-lookup"><span data-stu-id="ea737-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
