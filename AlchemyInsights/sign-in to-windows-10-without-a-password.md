---
title: Pierakstīšanās operētājsistēmā Windows 10, neizmantojot paroli
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1f325eb7afb1e88457296e8187f8ba6dff2ebfe0
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588287"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="27dd8-102">Pierakstīšanās operētājsistēmā Windows 10, neizmantojot paroli</span><span class="sxs-lookup"><span data-stu-id="27dd8-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="27dd8-103">Lai izvairītos no paroles rakstīšanas Windows startēšanas laikā, ieteicams izmantot kādu no Windows Hello drošās pierakstīšanās opcijām, piemēram, PIN, sejas atpazīšanas vai pirksta nospiedumu, ja tas ir pieejams.</span><span class="sxs-lookup"><span data-stu-id="27dd8-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="27dd8-104">Ja tiešām vēlaties atspējot drošo pierakstīšanos, skatiet tālāk sniegtos norādījumus "automātiski pierakstīties Windows 10".</span><span class="sxs-lookup"><span data-stu-id="27dd8-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="27dd8-105">**Secure Windows Hello alternatīvas konta paroli**</span><span class="sxs-lookup"><span data-stu-id="27dd8-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="27dd8-106">Dodieties uz **iestatījumi > konti > pierakstīšanās opcijas** (vai noklikšķiniet [šeit](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="27dd8-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="27dd8-107">Tiks uzskaitītas pieejamās pierakstīšanās opcijas.</span><span class="sxs-lookup"><span data-stu-id="27dd8-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="27dd8-108">Piemērs:</span><span class="sxs-lookup"><span data-stu-id="27dd8-108">For example:</span></span>

![Pierakstīšanās opcijas.](media/sign-in-options.png)

<span data-ttu-id="27dd8-110">Noklikšķiniet uz vai pieskarieties kādai no opcijām, lai to konfigurētu.</span><span class="sxs-lookup"><span data-stu-id="27dd8-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="27dd8-111">Nākamreiz startējot vai atbloķējot sistēmu Windows, paroles vietā varēs izmantot jauno opciju.</span><span class="sxs-lookup"><span data-stu-id="27dd8-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="27dd8-112">**Automātiski pierakstīties Windows 10**</span><span class="sxs-lookup"><span data-stu-id="27dd8-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="27dd8-113">**Piezīme**: automātiska pierakstīšanās ir ērta, bet ievieš drošības risku, it īpaši, ja jūsu dators ir pieejams vairākiem cilvēkiem.</span><span class="sxs-lookup"><span data-stu-id="27dd8-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="27dd8-114">Uzdevumjoslā noklikšķiniet uz pogas **Sākt** vai pieskarieties tai.</span><span class="sxs-lookup"><span data-stu-id="27dd8-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="27dd8-115">Ierakstiet **lodziņā netplwiz** un nospiediet taustiņu ENTER, lai atvērtu logu lietotāju konti.</span><span class="sxs-lookup"><span data-stu-id="27dd8-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="27dd8-116">**Lietotāju kontos**noklikšķiniet uz konta, kurā vēlaties automātiski pierakstīties, startējot sistēmu Windows.</span><span class="sxs-lookup"><span data-stu-id="27dd8-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="27dd8-117">Noņemiet atzīmi no izvēles rūtiņas "lietotājiem ir jāievada lietotājvārds un parole, lai izmantotu šo datoru".</span><span class="sxs-lookup"><span data-stu-id="27dd8-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Lietotājiem ir jāievada lietotājvārds un parole.](media/users-must-enter-username.png)

5. <span data-ttu-id="27dd8-119">Noklikšķiniet uz **Labi**.</span><span class="sxs-lookup"><span data-stu-id="27dd8-119">Click **OK**.</span></span> <span data-ttu-id="27dd8-120">Jums tiks lūgts ievadīt un apstiprināt paroli atlasītajam kontam.</span><span class="sxs-lookup"><span data-stu-id="27dd8-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="27dd8-121">Noklikšķiniet uz **Labi** , lai pabeigtu.</span><span class="sxs-lookup"><span data-stu-id="27dd8-121">Click **OK** to finish.</span></span> <span data-ttu-id="27dd8-122">Nākamreiz, kad tiks startēta operētājsistēma Windows 10, tā automātiski pierakstīsies atlasītajā kontā.</span><span class="sxs-lookup"><span data-stu-id="27dd8-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
