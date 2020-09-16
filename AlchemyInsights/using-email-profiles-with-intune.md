---
title: E-pasta profilu izmantošana ar Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653295"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="d9fc1-102">E-pasta profilu izmantošana ar Intune</span><span class="sxs-lookup"><span data-stu-id="d9fc1-102">Using email profiles with Intune</span></span>

<span data-ttu-id="d9fc1-103">Intune var izmantot, lai izveidotu un izvietotu e-pasta profilus vietējā (iebūvētā) e-pasta klientam vairāku ierīču platformās.</span><span class="sxs-lookup"><span data-stu-id="d9fc1-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="d9fc1-104">Lai iegūtu informāciju par dažiem ierobežojumiem, kas saistīti ar e-pasta profiliem, tostarp to, kā tiek apstrādāti esošie profili un kā noņemt e-pasta profilus, skatiet rakstu [e-pasta iestatījumu pievienošana ierīcēs, izmantojot Intune](https://docs.microsoft.com/intune/email-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="d9fc1-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="d9fc1-105">Lai iegūtu papildinformāciju par to, kā izveidot e-pasta profilus katrai ierīču platformai, skatiet:</span><span class="sxs-lookup"><span data-stu-id="d9fc1-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="d9fc1-106">Android ierīces iestatījumi, lai pakalpojumā Intune konfigurētu e-pastu, autentifikāciju un sinhronizāciju</span><span class="sxs-lookup"><span data-stu-id="d9fc1-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="d9fc1-107">E-pasta iestatījumu pievienošana operētājsistēmā iOS un iPadOS ierīcēs programmā Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="d9fc1-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="d9fc1-108">E-pasta profila iestatījumi pakalpojumā Microsoft Intune ierīcēs, kurās darbojas operētājsistēma Windows Phone 8,1</span><span class="sxs-lookup"><span data-stu-id="d9fc1-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="d9fc1-109">E-pasta profila iestatījumi ierīcēm, kurās darbojas Windows 10 programmā Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="d9fc1-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="d9fc1-110">**Kopējā sinhronizācijas problēma**</span><span class="sxs-lookup"><span data-stu-id="d9fc1-110">**Common syncing issue**</span></span>

<span data-ttu-id="d9fc1-111">**KNOX Android e-pasta profils neļauj sinhronizēt lietotāju kontaktpersonas, kalendārus un uzdevumus.**</span><span class="sxs-lookup"><span data-stu-id="d9fc1-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="d9fc1-112">KNOX tehnoloģiju KNOX e-pasta profils piedāvā administratoram iespēju izlemt, kuri satura tipi ir sinhronizēti ar ierīci, iestatot katru iespējoto.</span><span class="sxs-lookup"><span data-stu-id="d9fc1-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="d9fc1-113">Ja iestatījums jebkuram satura tipam ir iestatīts uz **nav konfigurēts** (noklusējums), šis satura tips netiek sinhronizēts automātiski.</span><span class="sxs-lookup"><span data-stu-id="d9fc1-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="d9fc1-114">Lietotājs var iespējot satura tipu, ko tie vēlas veikt tieši ierīcē manuāli, taču šī konfigurācija tiek pārrakstīta, izmantojot Intune politikas iestatījumu, un šī satura tipa sinhronizācijas pieturas.</span><span class="sxs-lookup"><span data-stu-id="d9fc1-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

