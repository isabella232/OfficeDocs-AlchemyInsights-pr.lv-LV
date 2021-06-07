---
title: Drošības Microsoft Intune bāzes datu izmantošana, lai konfigurētu Windows 10 ierīces
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793897"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="1d2ec-102">Drošības Microsoft Intune bāzes datu izmantošana, lai konfigurētu Windows 10 ierīces</span><span class="sxs-lookup"><span data-stu-id="1d2ec-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="1d2ec-103">Intune drošības bāzes datus, kas palīdz aizsargāt lietotājus un ierīces.</span><span class="sxs-lookup"><span data-stu-id="1d2ec-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="1d2ec-104">Drošības bāzes datu bāzes Windows ar iestatījumiem iepriekš konfigurētām grupām, ko izmanto, lai lietotu zināmu iestatījumu grupu un noklusējuma vērtības, ko iesaka attiecīgās drošības grupas.</span><span class="sxs-lookup"><span data-stu-id="1d2ec-104">Security baselines are Windows settings pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="1d2ec-105">Izveidojot drošības bāzes datu profilu intune, jūs izveidojat veidni, kas sastāv no vairākiem ierīču konfigurācijas profiliem.</span><span class="sxs-lookup"><span data-stu-id="1d2ec-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="1d2ec-106">Izvietojot drošības bāzlīnijus lietotāju grupām vai ierīcēm, iestatījumi tiek lietoti ierīcēm, kuras darbojas Windows 10 versijā.</span><span class="sxs-lookup"><span data-stu-id="1d2ec-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="1d2ec-107">Piemēram, Microsoft mobilo ierīču pārvaldības (Mobile Device Management — MDM) drošības bāzlīnija automātiski BitLocker iespējo datu iespējošanu noņemamiem diskiem, pieprasa ierīces atbloķēšanu ar paroli un atspējo pamata autentifikāciju.</span><span class="sxs-lookup"><span data-stu-id="1d2ec-107">For example, the Microsoft mobile device management (MDM) security baseline automatically enables BitLocker for removable drives, requires the password for unlocking a device, and disables basic authentication.</span></span> <span data-ttu-id="1d2ec-108">Ja noklusējuma vērtība jūsu vidē nedarbojas, varat pielāgot bāzes datu bāzes informāciju, lai lietotu iestatījumus.</span><span class="sxs-lookup"><span data-stu-id="1d2ec-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="1d2ec-109">Drošības bāzes datu bāzes arī palīdz izveidot drošu darbplūsmu programmā Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1d2ec-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="1d2ec-110">Drošības bāzlīnija ietver labāko praksi un ieteikumus iestatījumiem, kas ietekmē drošību.</span><span class="sxs-lookup"><span data-stu-id="1d2ec-110">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="1d2ec-111">InTune partneri ar Windows grupu, kas izveido bāzes datu bāzes kodus grupas politikām, tāpēc šie ieteikumi ir balstīti uz nepārtrauktām vadlīnijām un plašas pieredzes.</span><span class="sxs-lookup"><span data-stu-id="1d2ec-111">Intune partners with the Windows security team that creates baselines for group policies, so these recommendations are based on solid guidance and extensive experience.</span></span>

<span data-ttu-id="1d2ec-112">Ja esat jauns Intune lietotājam un neesat pārliecināts par to, ar ko sākt, drošības bāzes rādītāji palīdz ātri izveidot un izvietot drošu profilu.</span><span class="sxs-lookup"><span data-stu-id="1d2ec-112">If you're new to Intune and unsure of where to start, security baselines help you quickly create and deploy a secure profile.</span></span> <span data-ttu-id="1d2ec-113">Ja pašlaik izmantojat grupas politiku, migrēšana uz Intune pārvaldības nolūkiem ir daudz vienkāršāka, izmantojot drošības bāzes datus, jo tie ir iebūvēti intune un ietver modernas pārvaldības iespējas.</span><span class="sxs-lookup"><span data-stu-id="1d2ec-113">If you currently use a group policy, migrating to Intune for management purposes is much easier with security baselines because they are built into Intune and include cutting-edge management capabilities.</span></span>

<span data-ttu-id="1d2ec-114">Papildinformāciju skatiet rakstā [Drošības Windows un Mobilo](/windows/security/threat-protection/windows-security-baselines) ierīču [pārvaldība.](/windows/client-management/mdm/)</span><span class="sxs-lookup"><span data-stu-id="1d2ec-114">To learn more, see [Windows security baselines](/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](/windows/client-management/mdm/).</span></span>

